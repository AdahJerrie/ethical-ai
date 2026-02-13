#### Pseudocode that checks if a string is a palindrome

``Receive a string as input from the user``

``store the input received from the user``

``Reverse the input string and compare with the stored input``

``Display the result if the reverse equals the original stored input``

``note that any string of length 1 is always a palindrome``

##### My solution in python

#modified version of the above palindrome function that
#1. removes spaces and punctuation
#2. converts all uppercases to lowercase.

def pal_checker(x):
    # create and empty string, this will allow us build a new string that contains only valid xters(letters & numbers)
    empty = ""

    #now loop through each character in the given string
    for char in x:
        #using a special "string method" in python to check for numbers and letters
        #alternative to .isalnum() string method
        if ('0' <= char <= '9') or ('a' <= char <= 'z') or ('A' <= char <= 'Z'):
        #if char.isalnum(): #this string method returns true - if the character is a letter or number and false - if its a space or punctuation
        #ALTERNATIVELY ALSO, u can separate the number and number check
        #if char.isalpha() or char.isnum():
            empty += char.lower() #converts uppercase to lowercase
            #so now spaces has been removed, uppercase converted to lowercase, and the new string now appended to the old empty string that was created
    
    length = len(empty) #getting the current length of xters.

    #iterating through half of the string(algorithm optimisation) and comparing with the reverse
    for i in range(length // 2):
        #now symmetric character comparison
        if empty[i] != empty[length - i - 1]:
            return "not pal" #Early exit (efficiency): the function stops immediately a mismatch is found
            #For time complexity sake, this saves time instead of checking the entire string.
    
    return "palindrome" #It returns successful completion once all the boxes are checked!
#code walk through:
#1. Input string received
#2. spaces and punctuation removed
#3. converted to lowercase
#4. compared front and back
#5. all characters match


print(pal_checker("racecar"))
print(pal_checker("hello"))
print(pal_checker("A man a plan a canal Panama"))


**What I learnt from solving it before asking AI**

Firstly I saw that my confidence increased, and then I had a firm grasp on the understanding of what I am meant to do. Such that I can explain exactly what is happening in my code. 


## How my understanding is different now

Now I am able to use AI more profitably. In general my understanding of AI's function in writing code or programming is now different, I don't depepnd on it to generate my codes for me. I write my code if it works I ask for modifications and edge cases suggestions from AI.

I can now write similar functions e.g reverse a string without help.
