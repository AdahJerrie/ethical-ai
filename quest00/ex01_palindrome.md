#### Pseudocode that checks if a string is a palindrome

``Receive a string as input from the user``

``store the input received from the user``

``Reverse the input string and compare with the stored input``

``Display the result if the reverse equals the original stored input``

``note that any string of length 1 is always a palindrome``

##### My solution in Javascript

    function palindrome_check(x) {
    
        let len = s.length;

    //Iterate over the first half of the string
    for (let i = 0; i < len /2; i++) {
        
        //If the xters at symmetric positions are not equal
        if (x[i] != x[len -i -1]) {

            //return not pal

            return "not a palindrome";
        } else {

        }

    }
    //if all symmetric xters are equal then its a pal
    return "This is a palindrome";
}


**What I learnt from solving it before asking AI**

Firstly I saw that my confidence increased, and then I had a firm grasp on the understanding of what I am meant to do. Such that I can explain exactly what is happening in my code. 


## How my understanding is different now

Now I am able to use AI more profitably. In general my understanding of AI's function in writing code or programming is now different, I don't depepnd on it to generate my codes for me. I write my code if it works I ask for modifications and edge cases suggestions from AI.

I can now write similar functions e.g reverse a string without help.
