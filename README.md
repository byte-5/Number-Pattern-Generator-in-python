# Number-Pattern-Generator-in-python

def number_pattern(n):
    """
    Creates a space-separated string of numbers from 1 to n.
    """
    # 1. Check if the argument is an integer
    if not isinstance(n, int):
        return "Argument must be an integer value."
    
    # 2. Check if the integer is greater than 0
    if n < 1:
        return "Argument must be an integer greater than 0."
    
    # 3. Use a for loop to build the string
    pattern = ""
    for i in range(1, n + 1):
        pattern += str(i) + " "
    
    # 4. Return the string (using strip() to remove the trailing space)
    return pattern.strip()

# Examples of usage:
# print(number_pattern(4))  # Output: "1 2 3 4"
# print(number_pattern(1))  # Output: "1"
# print(number_pattern(0))  # Output: "Argument must be an integer greater than 0."
# print(number_pattern("a"))# Output: "Argument must be an integer value."
