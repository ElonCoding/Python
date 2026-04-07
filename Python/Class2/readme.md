### Class Summary: Loops in Python

This class focuses on loops in Python, covering their types, usage, and related programming questions. Below is a detailed explanation of all major loop constructs in Python.

#### 1. **For Loops**
    - Used to iterate over a sequence (like a list, tuple, string, or range).
    - Syntax: `for item in iterable:`
    - Example:
      ```python
      for i in range(5):
            print(i)  # Outputs: 0, 1, 2, 3, 4
      ```

#### 2. **While Loops**
    - Executes as long as a condition is true.
    - Syntax: `while condition:`
    - Example:
      ```python
      count = 0
      while count < 5:
            print(count)
            count += 1  # Outputs: 0, 1, 2, 3, 4
      ```

#### 3. **Nested Loops**
    - Loops inside loops, useful for multi-dimensional data.
    - Example:
      ```python
      for i in range(3):
            for j in range(2):
                 print(f"({i}, {j})")  # Outputs pairs like (0,0), (0,1), etc.
      ```

#### 4. **Loop Control Statements**
    - `break`: Exits the loop prematurely.
    - `continue`: Skips the current iteration.
    - `else`: Executes after the loop completes (if no break).
    - Example:
      ```python
      for i in range(5):
            if i == 3:
                 break
            print(i)  # Outputs: 0, 1, 2
      ```

#### 5. **List Comprehensions** (Loop-like for concise lists)
    - A compact way to create lists using loops.
    - Syntax: `[expression for item in iterable if condition]`
    - Example:
      ```python
      squares = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]
      ```

This class includes exercises and questions to practice these concepts. Read the full documentation for in-depth examples and best practices.