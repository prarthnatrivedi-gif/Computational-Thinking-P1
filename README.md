# Computational-Thinking-P1

 Task 1: Identity Investigation

 Objective:
To analyze how memory locations change when different data types are modified.

 Action:
A Python file `identity_prarthna.py` was created. The `id()` function was used to print memory addresses before and after modifying variables.

 Observation:
- Integer, String, Tuple → Memory ID changes  
- List → Memory ID remains the same  

 Conclusion:
Immutable data types (int, string, tuple) create new memory when modified, while mutable data types (list) update the same memory location.


 Task 2: Nature of Commit History

 Action:
A Git repository was created and multiple commits were made with messages such as "Version 1" and "Version 2".

 Question:
Does "Version 2" still exist in the folder?

 Answer:
Yes, Version 2 still exists, along with Version 1, in the commit history.

 Explanation:
Git follows an immutable model where commits cannot be changed. Instead of modifying existing commits, Git creates new ones for every update.

 Conclusion:
All versions are preserved in Git, ensuring complete history and data safety.
 Task 3: Shallow Copy Behavior

Action:
A nested list was created and copied using `list()`. An element in the copied list was modified.

 Observation:
Changes in the copied list also affected the original list.
 Explanation:
This happens because a shallow copy only copies the outer structure, while inner elements still reference the same memory.
 Conclusion:
Deep copy should be used to create independent copies of nested data.

 Task 4: Commit Immutability

 Action:
A commit was created and its hash was recorded. The commit message was then changed using `git commit --amend`, and the new hash was noted.

 Observation:
The commit hash changed after modifying the message.

 Explanation:
Commit hashes depend on content, message, and metadata. Any change results in a new commit with a new hash.

 Conclusion:
Git commits are immutable, and any modification creates a new commit instead of changing the original.