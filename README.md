# React Native FlatList: Key Extraction Issues

This repository demonstrates a common error in React Native's FlatList component: using inconsistent or non-unique keys for data items. This can lead to incorrect rendering, unexpected behavior, and crashes.

## Problem

The `keyExtractor` prop in FlatList is critical for efficient rendering and data updates. If keys are not unique or change unexpectedly, FlatList might struggle to identify and update items correctly. This often results in incorrect item positions, duplicate items, or performance problems.  The example provided shows a scenario with duplicate keys, which can cause FlatList to produce unpredictable outputs.

## Solution

The solution involves ensuring unique and immutable keys for each item in your data array.  Generating unique IDs (like using UUIDs) is a common practice to address this problem. The corrected code example uses a different approach to generate unique keys, thereby fixing the issues.