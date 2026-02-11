def is_palindrome(s):
   
   cleaned_str = ""
   for char in s:
       if char.isalnum():
           cleaned_str += char.lower()
          
   
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
       left  += 1
       right -= 1
   return {
       "is_palindrome":True,
       "Index valu":None
   }

print(is_palindrome("A man a plan a canal Panam"))  
print(is_palindrome("Mr. Owl ate my metal worm")) 
print(is_palindrome("No 'x' in Nixon"))



Did I miss anything? Can it be more efficient?"

Modified version has the following:
- Uses O(1) extra space
- Still O(n) time
- Doesn't create any new string
- Very common in coding interviews


def is_palindrome(s: str) -> dict:
    cleaned = ''.join(c.lower() for c in s if c.isalnum())
    
    left = 0
    right = len(cleaned) - 1
    
    while left < right:
        if cleaned[left] != cleaned[right]:
            return {
                "is_palindrome": False,
                "mismatch_left_index": left,
                "mismatch_right_index": right,
                "left_char": cleaned[left],
                "right_char": cleaned[right]
            }
        left += 1
        right -= 1
        
    return {
        "is_palindrome": True,
        "mismatch_index": None
    }