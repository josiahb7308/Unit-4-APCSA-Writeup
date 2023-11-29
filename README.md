# Process Writeup

## Name: Josiah Benitez
## Course: SEP12
## Period: 7
## Concept: Unit 4

### Overview

In this Unit we learned about things similar to things we already knew from javascript such as conditionals, using if and else statements, and we also learned some new things like De Morgans law and comparing objects. We also added on to the boolean information we already knew and used and/or more often.
## First Challenge
### Conditional functionality

On the Unit 3 test I had a pretty hard time with the conditional questions and in some of those questions it required me to choose what conditionals would be able to replace other conditionals. For example, in the exam on question 5 it asked me what conditional sequence would be able to replace the following code:
  
```java
    if (low < amount  && amount < high)
{
  System.out.println("Amount of customers could be better.");
}
else
{
  System.out.println("Amount of customers is great!");
}
```
I answered with the wrong choice because I missed the point that something is supposed to print when the amount is = to the high and it should say "Amount of customers is great!" but in the code that I picked it didnt do that. I made my mistake when I went throught the conditional in my head and I missed a very important detail causing me to get the answer wrong. The test tells me that the right answer to this question was this: 

```java
    if (amount > low)
{
  if (amount < high)
  {
    System.out.println("Amount of customers could be better.");
  }
  else
  {
  System.out.println("Amount of customers is great!");
  }
}
else
{
  System.out.println("Amount of customers is great!");
}
```

 This code can replace the code displayed earlier correctly and this mistake was due to my mistake I made when evaluating the decisions available to me. I can fix this by going over questions similar to this on a time limit and continuously doing this until I get a better grade.
 
## Second Challenge
### Finding output of conditionals

On the exam I found myself also getting a lot of questions where I had to find the output of code including mainly conditionals. For example on question 20 which looks like this:

    
 ```java 
     Car Honda = new Car(4, 2);
Car Mercedes = new Car(4, 2);

if (Honda == Mercedes) 
{
    System.out.print("equal ");
} 
else 
{
    System.out.print("not equal ");
}
   ```

I chose the answer that says it will print equal because I forgot that when comparing objects even if they are the same value if they arent pointing to the same data then they arent diplayed as equal. The actual answer would be not equal because Honda == Mercedes would give you a false value and then the code would drop to the else which prints "not equal". All in all I need to study these questions and get better at taking these type of tests and using less time on each question.
## Third Challenge
### Nested if statements 

On the exam there were questions including code with if statements inside another if statement and with these type of questions you must pay attention to the brackets very well because one bracker in one place can change the whole flow of the code. I messed up on a lot of these nested if statement questions so here is an example: 

```java
if (low < amount  && amount < high)
{
  System.out.println("Amount of customers could be better.");
}
else
{
  System.out.println("Amount of customers is great!");
}
```
The objective was to replace this code with another set of conditionals that did the same thing out of the options 1,2, and 3. The answer I picked was number 2 which is:

```java
if (amount > low) 
{
  if (amount < high)
  {
    System.out.println("Amount of customers could be better.");
  }
}
  else
  {
    System.out.println("Amount of customers is great!");
  }
```
The reason why this one was wrong was because if amount > low and amount >= high, the code would just drop to the bottom and not print anything. I did not go through all the possibilities of what the amount could be when I evaluated this decision and this same mistake cost me a lot of points. The correct answer was this: 

```java
if (amount > low)
{
  if (amount < high)
  {
    System.out.println("Amount of customers could be better.");
  }
  else
  {
  System.out.println("Amount of customers is great!");
  }
}
else
{
  System.out.println("Amount of customers is great!");
}
```
This code had all the functionalities of the code that needed to be replaced and the reason I missed this was because I attributed the first else statement I saw to the first if statement when I needed to look at the indentations and the brackets to see which else was for which if.
### Takeaways

* Always ask for help when you are stuck, whether that be a peer or teacher. For example, I asked my neighbor who sits next to me in class about the question shown in question 1 and he walked me through it step by step because he got it right. 
* Trying code you dont understand in a sandbox lets you understand what each batch of code gives you and why one is right and the other isnt. After the quiz when I got home I did this for a good amount of the questions that I didnt understand and this let me physically see why one is right and one is wrong instead of just seeing the red and green marks.
* Take better notes and more notes if you want to bring your quiz and test grades up. This comes down to me reminding myself to write things down when I have a "woah" moment or I need to remember some code or syntax and what they do such as "!", "||", "&".
* Look over every part of conditionals when you are trying to find the value of it or its ability to replace other code because one different or/and statement or "!" can change the whole codes purpose and ability to replace another conditional.
