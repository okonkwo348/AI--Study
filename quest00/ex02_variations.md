def is_palindrome(s):
   # Clean the string: remove any characters that are not alphabets
   cleaned_str = ""
   for char in s:
       if char.isalnum():
           cleaned_str += char.lower() # add up lower case to cleaned
          
   # Check for palindrome
   left = 0
   right = len(cleaned_str)-1
  
   while left < right:
       if cleaned_str[left] != cleaned_str[right]:
           return {
               "is_palindrome":False,
               "index_number":left,
               "palindrome_rightchar":cleaned_str[right],
               "palindrome_leftchar":cleaned_str[left]
           }
       left = left + 1
       right  = right - 1
   return {
       "is_palindrome":True,
       "Index valu":None
   }

print(is_palindrome("A man a plan a canal Panam"))  # Expected: True
print(is_palindrome("Mr. Owl ate my metal worm"))  # Expected: True
print(is_palindrome("No 'x' in Nixon"))
