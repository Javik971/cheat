---
title: diff
category: CLI
layout: 2017/sheet
tags: [Featured]
updated: 2023-10-23
keywords:
  - diff
---

### The diff command compares two files and outputs the lines that are unique to each file
diff file1 file2 | grep '^<' | cut -c 3-

### Entries marked with ‘<‘ represent lines that would have to be removed from file1 so that it resembles file2. Therefore, these are lines unique to file1. We use cut -c 3- to remove the first two characters because these are added by diff and are not part of the original file.
### To find lines unique to file2 instead, we only need to change the pattern used with grep to ‘^>‘:

$ diff file1 file2 | grep '^>' | cut -c 3-

### Entries that begin with ‘>‘ represent lines that would have to be added to file1 so that it resembles file2. Therefore, these are lines unique to file2 which are missing in file1.
