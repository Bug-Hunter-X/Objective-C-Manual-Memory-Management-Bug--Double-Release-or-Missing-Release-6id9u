# Objective-C Manual Memory Management Bug: Double Release or Missing Release

This repository demonstrates a subtle bug that can occur in Objective-C when using manual reference counting (MRC) for memory management. The bug involves incorrect handling of `retain` and `release`, leading to either double-releasing objects (causing crashes) or failing to release them (resulting in memory leaks).

## The Bug
The `bug.m` file contains code that showcases the problem.  It improperly manages the lifetime of an NSString object, potentially leading to either a double release or a memory leak depending on the execution path. 

## The Solution
The `bugSolution.m` file presents a corrected version of the code. It addresses the memory management issue by ensuring that `retain` and `release` are used correctly, preventing both double releases and memory leaks.