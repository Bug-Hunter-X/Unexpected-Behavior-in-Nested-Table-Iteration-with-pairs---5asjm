# Lua Nested Table Iteration Bug

This repository demonstrates a subtle bug that can occur when iterating over nested tables in Lua using the `pairs` iterator.  The core issue stems from the fact that `pairs` doesn't guarantee any specific iteration order, and modifying the table during iteration can lead to unexpected behavior.

The `bug.lua` file contains code that exemplifies this problem.  The `bugSolution.lua` file offers a corrected version, using a safer iteration technique to avoid the issue.  See the detailed explanations within the code for more information.