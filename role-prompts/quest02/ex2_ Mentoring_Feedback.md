1. Ask the model to act as a coding mentor.

    OUTPUT:

    Great — I’ll act as your **coding mentor** from now on. 👨‍💻

    That means I will:

    * Explain concepts step by step (beginner → advanced)
    * Correct your code gently and clearly
    * Focus on understanding, not just giving answers
    * Ask guiding questions instead of rushing solutions
    * Help you think like a programmer (not just copy code)

    Since I know you already have strong skills in **Python and Django**, I’ll tailor explanations to your level and help you grow deeper in logic, debugging, and system thinking.

    ### How I’ll mentor you

    When you ask questions, I can help you with:

    * 🧠 Programming fundamentals (logic, complexity, edge cases)
    * 🐍 Python (clean code, best practices, debugging)
    * 🌐 Django (projects, architecture, models, APIs)
    * 🧩 Problem solving (step-by-step reasoning)
    * 🚀 Career growth (projects, GitHub, mastery path)

    ### Example of mentorship style

    Instead of just saying:

    > “Here is the solution.”

    I’ll do this:

    1. Understand your thought process
    2. Point out mistakes (if any)
    3. Explain why
    4. Guide you to the correct solution

    ### First mentor question (to personalize your learning):

    What are you currently learning or struggling with the most?

    * Python basics
    * Django projects
    * Data structures & algorithms
    * AI/ML
    * Debugging code
    * Something else?

    Tell me, and I’ll mentor you based on that.


2. Provide a simple piece of code (e.g., a Python function with a bug).


    Errored code:

    def is_palindrome(s):
        # Convert the entire string to lowercase
        s = s.lower()
        
        # Clean the string: remove any characters that are not alphabets
        cleaned_str = ""
        for char in :  # error
            if char.isalpha():
                cleaned_str += char
                
        # Check for palindrome
        return cleaned_str == cleaned_str[::-1]
        


3. Prompt the model: "Act as a mentor reviewing this code. Provide corrections and explain improvements."


    AI OUTPUT:
    
    Alright, mentor mode on. 👨‍💻
    Let’s review your code carefully like a code review session.

    ### Your Code

    ```python
    def is_palindrome(s):
        # Convert the entire string to lowercase
        s = s.lower()
        
        # Clean the string: remove any characters that are not alphabets
        cleaned_str = ""
        for char in :
            if char.isalpha():
                cleaned_str += char
                
        # Check for palindrome
        return cleaned_str == cleaned_str[::-1]
    ```

    ---

    # 🛑 1. Critical Error (Syntax Bug)

    ### Problem:

    ```python
    for char in :
    ```

    You forgot to specify what you are looping over.

    ### Fix:

    You should loop over the string `s`:

    ```python
    for char in s:
    ```

    Without this, the code will not run at all.

    ---

    # ⚠️ 2. Inefficient String Concatenation

    ### Problem:

    ```python
    cleaned_str += char
    ```

    In Python, strings are **immutable**.
    Every time you do `+=`, Python creates a new string in memory.

    This makes the loop less efficient (especially for long inputs).

    ### Better Approach:

    Use a list and then join:

    ```python
    cleaned_chars = []
    for char in s:
        if char.isalpha():
            cleaned_chars.append(char)

    cleaned_str = "".join(cleaned_chars)
    ```

    This is more memory-efficient and faster.

    ---

    # 🧠 3. Logic Review (Good Design Choice)

    You correctly:

    * Normalized case (`lower()`) ✅
    * Filtered unwanted characters ✅
    * Used slicing for palindrome check ✅

    This shows good problem-solving structure.

    ---

    # ✨ 4. Improved Clean Version (Mentor Recommended)

    Here is a corrected and optimized version:

    ```python
    def is_palindrome(s):
        # Normalize to lowercase
        s = s.lower()
        
        # Use list for efficiency
        cleaned_chars = []
        for char in s:
            if char.isalpha():
                cleaned_chars.append(char)
        
        cleaned_str = "".join(cleaned_chars)
        
        # Palindrome check
        return cleaned_str == cleaned_str[::-1]
    ```

    ---

    # 🚀 5. Even More Pythonic (Advanced Improvement)

    Since you are already strong in Python, you can write this more cleanly:

    ```python
    def is_palindrome(s):
        cleaned = "".join(char.lower() for char in s if char.isalpha())
        return cleaned == cleaned[::-1]
    ```

    This:

    * Removes the manual loop
    * Is more readable
    * Is considered Pythonic in interviews and production code

    ---

    # 📊 6. Complexity Analysis (Mentor-Level Insight)

    * Time Complexity: **O(n)**
    (one pass to clean + one pass to reverse comparison)
    * Space Complexity: **O(n)**
    (new cleaned string stored)

    ---

    # 🎯 Final Mentor Feedback

    ### Strengths:

    * Clear step-by-step logic
    * Good preprocessing idea
    * Correct palindrome strategy

    ### Main Improvements:

    * Fix loop syntax error
    * Avoid string concatenation in loops
    * Use more Pythonic constructs (generator/list comprehension)


4. Review the response and check if the role influences feedback style.
    the response was:
    - Expalined the mistakes step-by-step instead of just fixing it.
    - Used a guidance tone
    - Very comprehensive.

    The role influences feedback style:
    - It focus on learning rather than a quick fix of code.
    - It was detail and explanatory. 
