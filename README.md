# ConcurrentModificationException in Kotlin MutableList Iteration

This repository demonstrates a common error encountered when modifying a mutable list while iterating over it using a standard for loop in Kotlin. The code showcases how the `ConcurrentModificationException` arises and provides a solution using iterators or other safer approaches.

## Problem

Directly removing elements from a mutable list while iterating through it with a `for` loop in Kotlin leads to a `ConcurrentModificationException`. This is because the loop's internal iterator gets out of sync with the list's structure after a removal.

## Solution

The solution involves using an iterator to safely remove elements from the list.  The iterator maintains consistency with changes made to the list.