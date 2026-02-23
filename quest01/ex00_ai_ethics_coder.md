Part A: The Critical Distinction

1. Write down your honest answers:

- How have you used AI for coding so far?
    I have used AI in building a marriage site.

- Do you ask AI for solutions before trying yourself?
    Yes, but sometimes i try things myself. Most time I just want to do things
    fast and easy myself of stress so i use AI.

- Can you explain code you've submitted without AI's help?
    Yes, I can explain it.

- What would happen if AI was suddenly unavailable during an exam or interview?
    I would try using my head and writing all I know.

2. Identify your current pattern: Which learner are you now? Learner A: "AI is my answer generator

- "Write a function that does X"

    def function_name(parameter1, parameter2):
    """
    Docstring: Describe what the function does here.
        """
        # Function body: Actionable code to do X
        result = parameter1 + parameter2
    return result

# Calling the function
output = function_name(5, 3)
print(output)

3. Write a brief paragraph: Where are you now, and where do you want to be?

    I am currently a learner A that usese AI as an answer generator and I want to be a learner B to use AI as a learning amplifier in order to really 
    understand any new concept and knowledge. AI as an amplifier help to solidifies knowledge and make the knowledge sticks better.



Part B: The Wrong Way vs. The Right Way

Challenge: Implement a simple function to check if a string is a palindrome.

Track A — The Wrong Way (observe but DO NOT do this):

    def is_palindrome(s):
    # Returns True if the string is equal to its reverse
        return s == s[::-1]

    # Quick test
    print(is_palindrome("radar"))  # True
    print(is_palindrome("python")) # False



Track B — The Right Way (DO THIS): Step 1: Attempt independently

def is_palindrome(input_string): 
    # Pre-process: Remove spaces and standardize to lowercase for accurate comparison
    input_string = input_string.replace(" ","").lower()

    # Initialize two pointers at opposite ends of the string
    left = 0
    right = len(input_string) - 1

    # Compare characters moving inward from both ends
    while left < right:
        # If a mismatch is found, it's not a palindrome
        if input_string[left] != input_string[right]:
            return False
        
        # Move pointers closer to the center
        left += 1
        right -= 1
    
    # If the loop finishes without returning False, all pairs matched
    return True


    Step 2: Strategic AI use After you have a working solution, ask AI:
    
    - What's the time complexity?

     Time Complexity: O(n). You only visit each character at most once. Even though the string might be "dirty" (lots of symbols), the pointers never backtrack.

     Space Complexity: O(1). This is the "Gold Medal." Since you are comparing characters directly within the original string, you aren't creating a cleaned_version or a reversed_version in your RAM.


     - What edge cases am I missing?

        Non-English Characters: s[left].lower() works for standard Latin characters, but some languages have unique rules for lowercase (like the Turkish "I"). For a global app, you’d use s[left].casefold().

        Empty or Single-Character Strings: Technically, "" and "a" are palindromes. Your code handles these correctly (returning True), but it's good to define this behavior for your specific project.

        Numeric Palindromes: Your code handles "12321" because .isalnum() includes numbers. If you only want letters, you'd use .isalpha().

        Accented Characters: "á" and "a" are seen as different characters. If "Áva" should be a palindrome, you would need to "normalize" the string first.
       
       
     - Alternatives and trade-offs?

        def is_palindrome(s):
            clean = "".join(c.lower() for c in s if c.isalnum())
            return clean == clean[::-1]

     - How does it perform on very long strings?"

        Imagine you are checking a 1GB text file to see if it’s a palindrome:

    The Slicing Method would try to load the file, create a 1GB "cleaned" string, and then a 1GB "reversed" string. You would likely crash your computer with an OutOfMemory error.

    Your Two-Pointer Method only needs the original string and two integers (left and right). It is the most stable approach for high-performance systems.

Step 3: Reflection

   - What did you learn by struggling first?

        I learnt how the two pointers move from the ends of a string to the 
        middle of the string at the While loop. I also learnt how the
         variables of the two pointers move.

   - How is your understanding different than if you'd just asked for the solution?

        I now know how to create a function that uses pointers to loop through
        a string.I also has the perception now that one can actually solve a problem 
        independently of AI
         

    - Can you now implement similar functions (reverse a string, find duplicates) without AI?

        yes, i can use a slice method to solve the problem.

        def is_palindrome (input_string):
            word = input_string.replace(" ","").lower()
            reversed_word=word [::-1]
            if word == reversed_word:
                return True
            else:
                return False


    - What mental model did you build?

      I built a mental picture of the movement of two keys from both ends of a row in a keyword
      as the movement of two pointers along a string while comparing the characters.                     
    


Part C: Testing Your Understanding

Without using AI, complete these variations:

    Ignore spaces and punctuation

    Make it case-insensitive

    Return the position where the string stops being a palindrome (if not a palindrome)


    def is_palindrome(input_string):
        clean_string = ""
        for char in input_string:
            if char.isalnum():
                clean_string= clean_string + char.lower()
    
        left = 0 
        right = len(clean_string) - 1

        while left < right:
            if clean_string[left] != clean_string[right]:
                return {
           "is_palindrome":False,
           "index_number":left,
           "palindrome_rightchar":cleaned_str[right],
           "palindrome_leftchar":cleaned_str[left]
                }

            left += 1
            right -= 1

        return {
    "is_palindrome":True,
    "Index valu":None
}


AI modification


    def is_palindrome(input_string):
        clean_string = "".join(c.lower() for c in input_string if c.isalnum())
        
        left = 0 
        right = len(clean_string) - 1

        while left < right:
            if clean_string[left] != clean_string[right]:
                return {
           "is_palindrome":False,
           "index_number":left,
           "palindrome_rightchar":cleaned_str[right],
           "palindrome_leftchar":cleaned_str[left]
                }

            left += 1
            right -= 1

        return {
            "is_palindrome":True,
            "Index valu":None
        }


    Part D: The Fairness Contract

    Here is a well-rounded and academically strong completion you can use:



1. I will use AI when:

* After I've attempted a problem for at least 20 minutes
* To understand why my solution works/doesn't
* To explore alternatives after I have a working solution
* To check for edge cases I may have missed
* To learn new concepts or clarity confusing topics
* T review best practices and improve code quality
* To get explanations, and improve code quality.
* To check for edge cases may have missed




2.  I will NOT use AI when:

* I haven't tried the problem myself
* I'm taking an assessment or test
* I need to build fundamentals
* The task is meant to test my independent problem-solving ability
* I cannot explain the solution in my own words afterward
* I am expected to create original work without assistance
* I am coping solution without understanding them
* I am using AI as a shortcut instead of learning



3. I know I'm using AI fairly when:

*I can explain my code without looking at AI's response
* I could solve similar problems without AI
* I feel more confident in my abilities
* I use AI as a tutor, not a replacement for effort
* I can identify mistakes in AI generated answer
* I will try to understand every solution provided
* I modify and adapt AI answers instead of copying them directly



    **[sign]**: Okonkwo Emmanuel Chisom     
    **[date]** : 15/02/2026



Part E: Real-World Scenario Analysis

    - Interview: "Explain how you'd implement a caching system." If you always relied on AI, can you answer?

        I sincerely do not know how to implement a caching system. 

    - Production bug at 2 AM: AI is unavailable. Can you debug code you don't fully understand?
        I can't debug the code because I didn't write it myself nor do I understand it.

    - New tech with little documentation: If you never learned to read docs and experiment, what happens?
        I wouldn't be able to know or understand the new tech.

    - Write a paragraph: How does using AI fairly now prepare you for these scenarios?
       AI fairly prepares me for real-world challenges like interview, production bug and learning a new learning 
       by giving me an depth knowledge, understanding and confidence of any programming language and program before 
       meeting the real-world challenges.

Part F: Building Irreplaceable Skills

Rate yourself 1–5 and write an improvement plan for your lowest area:

Skill                         Rating       Improvement Plan

Problem Decomposition           4           Spending time to understand the problem and the logic flow
Systems Thinking                4           Understand the how the logic flow and how each block of code affect the whole program
Critical Evaluation             2           know the logic and concepts of a programming languagem or project or program
Debugging Mindset               3           Reading the error message carefully and exercise patience in fixing it
Conceptual Understanding        3           Exercise patience in reading, studying and understanding the logic flow, concept and the issue a program is trying to solve
sfdyfdghyufuy                   


skill                           rated          

Choose your lowest-rated skill and write 3 specific actions you'll take this week to improve it without relying on AI.

Critcal Evaluation
Goal: Strengthen my ability to deeply understand concepts instead of just applying solutions.
    - Understand the concept and basic of a programming language.
    - Understand logic flow of a program.
    - Pay attention to indentation.