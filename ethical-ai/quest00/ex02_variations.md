1. Modify your palindrome function to:

    Ignore spaces and punctuation.

    Be case-insensitive.

    Return the position where the string stops being a palindrome (if not one).

def is_palindrome(s):
    cleaned_str = ""
    for char in s:
        if char.isalnum():
            cleaned_str += char.lower()
    
    left = 0
    right = len(cleaned_str) - 1
  
    while left < right:
        if cleaned_str[left] != cleaned_str[right]:
            return {
                "is_palindrome": False,
                "mismatch_index": left,
                "left_char": cleaned_str[left],
                "right_char": cleaned_str[right]
            }
        left += 1
        right -= 1

    return {
        "is_palindrome": True,
        "mismatch_index": None,
        "left_char": None,
        "right_char": None
    }


print(is_palindrome("A man, a plan, a canal, Panama"))  
print(is_palindrome("Mr. Owl ate my metal worm")) 
print(is_palindrome("No 'x' in Nixon"))

2.  Did I miss anything? Can it be more efficient?"

Modified version has the following:
- Uses O(1) extra space
- Still O(n) time
- Doesn't create any new string



def is_palindrome(s: str) -> dict:
    left = 0
    right = len(s) - 1
    
    while left < right:
        # 1. Skip non-alphanumeric from the left
        if not s[left].isalnum():
            left += 1
            continue # Restart the loop to check the new s[left]
            
        # 2. Skip non-alphanumeric from the right
        if not s[right].isalnum():
            right -= 1
            continue # Restart the loop to check the new s[right]
            
        # 3. Compare characters (case-insensitive)
        if s[left].lower() != s[right].lower():
            return {
                "is_palindrome": False,
                "mismatch_left_index": left,
                "mismatch_right_index": right,
                "left_char": s[left],
                "right_char": s[right]
            }
        
        # 4. Only move both if a valid comparison was made
        left += 1
        right -= 1
        
    return {
        "is_palindrome": True,
        "mismatch_index": None
    }

    
    Reflect on what AI added that you didn't consider initially.
Modified version has the following:
- Uses O(1) extra space
- Still O(n) time
- Doesn't create any new string

    