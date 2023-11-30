# Process Writeup

## Name: Josiah Benitez
## Course: SEP12
## Period: 7
## Concept: Unit 4

### Overview

In this Unit we learned about concepts similar to the ones we already knew from javascript such as while loops and for loops. We also learned about loops inside of a loop which is a nested loop. I had gotten two questions wrong on the exam for this unit and in this writeup I will be going over the mistakes I made and why I did.
## First Challenge
### For Loops Blunder

On question 18 I made the mistake of missing the fact that the characters are being appended in reverse order, my answer was correct except for that one part of the characters having to be in reverse order. This is the prompt:
  
```java
    String str = "result";
String result = "";
for (int i = 0; i < str.length(); i++) 
{
  int index = (i + 3) % str.length();
  result = str.substring(index, index + 1) + result;
}
```
What is stored by the string result after this code segment has been executed?

I selected the answer "ultres" but the actual answer was "sertlu" which is my answer but reversed. This was an easily avoidable mistake that couldve been averted by reading the code closer instead of jumping to conclusions and on impulse. One thing I also picked up is my lack of speed with determining outcomes when mod is involved. I am good with the other common things like multiplication, division, addition, subtraction. Mod always seems to take me more time to get the value after using it.


 
## Second Challenge
### Short Circuit Evaluation 

On question 6 it mainly came down to not having enough time and panicking to getting an answer down. Looking at this question now it definitely was one of the easier ones on the exam for me but I didnt have enough time so I messed up. This was the code:

    
 ```java 
    if (a < b && c != d)
{
  System.out.print("True");
}
   ```

I know already that booleans evaluate left to right and if a < b is false then automatically it makes the boolean false because it is using "&&" so if one is wrong then automatically both of them cant be right making it false. Another example would be:

```java
  if(chickens == cows || chickens == dogs)
{
System.out.print("True");
}
```
This example would automatically be true if chickens == cows and it would be false if chickens and cows werent equivalent as well as chickens and dogs not being equal. This is because it uses an "or" type of boolean so if one of the two booleans are true then the output is true and the condition is met.
### Takeaways

* Read keywords of questions on an exam so you can evaluate if you have the knowledge and time to fully and correctly complete the question or if it would be best to go to another question, this takeaway comes from my loss of a point on question 6 because I didnt have enough time.
* Short circuit evaluation is a great way to see the outcome of booleans without having to go through each outcome of the boolean.
* Look over every part of loops when you are trying to find the value of it or its ability to replace other code because one different "-" symbol or anything can make it wrong. I saw this on my mistake with the result string on question 18 and the for loop.
