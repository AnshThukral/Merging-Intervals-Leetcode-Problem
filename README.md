# Merging-Intervals-Leetcode-Problem

Problem Description: Merge Overlapping Intervals
Objective:
You are given a collection of intervals represented as a 2D array intervals, where each interval is defined by a start and an end point [start, end]. The task is to merge all overlapping intervals and return an array of the merged intervals.

Input:
intervals: A 2D array where each element is an interval [start, end]. The start and end points are integers, and the intervals may or may not be sorted.
Output:
A 2D array containing the merged intervals, sorted in ascending order by their start points.
Constraints:
1 <= intervals.length <= 10^4
intervals[i][0] <= intervals[i][1]

Input
[[1,3],[2,6],[8,10],[15,18]]

Output
[[1,6],[8,10],[15,18]]
Solution Outline:
Initial Check: If the list of intervals is empty or contains only one interval, return the intervals as they are.
Sorting: Sort the intervals by their starting points to ensure that any overlapping intervals are adjacent.
Merging Intervals: Traverse the sorted list, merging overlapping intervals by updating the end point of the current interval.
Output the Merged Intervals: Return the merged intervals in a new list.
