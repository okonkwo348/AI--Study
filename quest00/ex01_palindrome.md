Step 1 - Do it yourself

1. #Write pseudocode for a function that checks if a string is a palindrome.

 FUNCTION is_Palindrome(input_string)
     SET input_string to input_stringe with all spaces removed
     SET input_string to lowercase

     SET left to 0
     SET right to length of input_string minus 1

     WHILE left less than right
         IF input_string at position left is not equal to input_string at position right:
             RETURN False

         INCREMENT left 1
         DECREMENT right 1

         ENDIF

     RETURN True
     ENDWHILE

 INPUT input_string
 PRINT is_Palindrome(input_string)
 END FUNCTION

2. #Implement your solution in Python.


def is_palindrome(input_string):
    input_string = input_string.replace(" ","").lower()
    
    left = 0
    right = len(input_string) - 1
    while left < right:
        if input_string[left]!= input_string[right]:
            return False
            
        left +=  1
        right -= 1
        
    return True

3.#Test with examples like "racecar", "hello", and "A man a plan a canal Panama".

print(is_palindrome("racar"))
print(is_palindrome("hello"))
print(is_palindrome("A man a plan a canal Panama"))


4. #Add comments explaining your reasoning.

# Create a python function "is_palindrome" with argument "input_string"

#Remove empty spaces and change the input_string to lower case.

# Set a variable "left" to 0
# Set a Variable "right" to length of "case" minus ine
# These variables are pointers to help run through the input_string


# Create a while loop of left less than right to run through the input_string
# If condition is created to help check if the left index and right index of the input_string are not equal returning False while the loop still runs by moving to the next line
#As long the if condition is not met the loop continues to the increase the point from left by 1 and decrease the point from right by 1
# The increament and drecreament of both pointers moves towards themselves while the WHILE loop is still met.
# The loop dies when the pointers meet at the same index when left == right and return True. This implies that the input_string is a palindrome.
# Whenever the fuction is call it returns either True or False depending whether the WHILE loop is met.



Step 2 - Use AI to learn

1. What's the time complexity?

Time complexity: O(n)
Space complexity: O(n) (because new strings are created)

2. What edge cases might I miss?

Punctuation: "A man, a plan, a canal: Panama"

Tabs/newlines (only spaces removed): "a\tb\na"

Mixed whitespace types

Numbers in strings: "1a2a1"

Empty string ""

Single character "a"

Only spaces " "

Unicode/accents: "Àbba"

Emojis/symbols: "😊a😊"

None / non-string input (will crash)


3. Are there better approaches?"

Yes — Pythonic reverse check

`def is_palindrome(s: str) -> bool:
    cleaned = ''.join(c.lower() for c in s if c.isalnum())
    return cleaned == cleaned[::-1]



Step 3 - Reflection

# What did you learn from solving it before asking AI?

I learnt how to use while loop in solving the problem rather than using only if condition.
I also learnt to handle the spaces and case in a phrase string using replace and lowercase methods.
I learnt a lot about pseudocode like putting keywords in capital letter eg FUNCTION, WHILE, IF e.t.c.
Also, that the pseudocode focuses on logic rather than syntax.
I learnt what is a palindrome and how to create a python function.

# How is your understanding different now?

Initially, it's impossible to solve a question entirely without first going to ChatGPT.
But my perception is changed now because I did the pseudocode of a Palindrome python function without using AI.
I can now approach any question without going first to AI.
I am confidence of my code and can defend it.

# Could you now write similar functions (e.g., reverse a string) without help?

Yes, I can. I was able to learn another approach of solving the problem.
