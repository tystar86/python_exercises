#Determine the longest word in a sequence
>Write a program that will take a list of words as input and will return back
the longest word and its length in one tuple.

**Example:**
```
Input: ['Python', 'is', 'a', 'widely', 'used', 'high-level', 'programming',
        'language', 'for', 'general-purpose', 'programming,', 'created',
        'by', 'Guido', 'van', 'Rossum', 'and', 'first', 'released', 'in', '1991.']

Output: ('general-purpose', 15)
```

**Task:**
```
word_list = ['Python', 'is', 'a', 'widely', 'used', 'high-level', 'programming',
        'language', 'for', 'general-purpose', 'programming,', 'created',
        'by', 'Guido', 'van', 'Rossum', 'and', 'first', 'released', 'in', '1991.']

def main(word_list):
    # create a list where you will store the currently longest word and the
    # number of occurence in the word_list
    max_word = ['',0]

    # iterate over the list and check whether each word is the longest one


    # return the result as as a tuple
    return result

if __name__=='__main__':
    main(word_list)
```










#Get the filename extension
>Write a Python program that will accept a filenames input return
the extension of that file.

**Example:**
```
Sample filename : test.txt
Output : txt
```
**Task:**
```
filename = 'super.test.txt'
def main(filename):
    # how can we divide strings based on a character? Find the method

    return result

if __name__=='__main__':
    main(filename)
```








#Calculate the difference between the highest even and highest odd value in a sequence
>Write a Python program that will collect all the even numbers and odd numbers
separately. Then return the absolute difference between the highest even and
highest odd value.

**Example:**
```
Input:
nums = [
    386, 462, 47, 418, 907, 344, 236, 375, 823, 566, 597, 978, 328, 615, 953, 345,
    399, 162, 758, 219, 918, 237, 412, 566, 826, 248, 866, 950, 626, 949, 687, 217,
    815, 67, 104, 58, 512, 24, 892, 894, 767, 553, 81, 379, 843, 831, 445, 742, 717,
    958,743, 527
    ]

Output: 25
```

**Task:**
```
nums = [
    386, 462, 47, 418, 907, 344, 236, 375, 823, 566, 597, 978, 328, 615, 953, 345,
    399, 162, 758, 219, 918, 237, 412, 566, 826, 248, 866, 950, 626, 949, 687, 217,
    815, 67, 104, 58, 512, 24, 892, 894, 767, 553, 81, 379, 843, 831, 445, 742, 717,
    958,743, 527
    ]


def main(nums):
    # prepare 2 variables that will collect even and odd numbers separately


    # collect the odd resp. even numbers using loop


    # calculate the absolute difference between the highest even and  highest odd value.

    # return the result
    return result

if __name__=='__main__':
    main(nums)
```








#Calculate the distance between two points in 2D space
>Write a Python program, that will accept two tuples of 2 numbers
each representing coordinates (position) of a point and calculate
the distance between those 2 points. The output should be a float,
therefore let's round the result to 2 decimal places.

>The distance should be straight line between the two points.
The coordinates cannot be negative numbers.


**Example:**
```
Input:
The point A is situated at coords [234, 34]
The point B is situated at coords [27, 114]

Output:
# input points A,B between which is the distance we have to calculate
A=[234, 34]
B=[27, 114]
```
**Task:**
```
from math import sqrt

def main(A,B):
    # your program should use knowledge from basic school about
    # calculating the length of the 3rd side in a triangle
    # you will also need to use the function sqrt which is used as follows:
    # sqrt(25) -> result is 5
    a = round(A[0]-B[0],2)
    b = round(A[1] - B[1],2)
    result = round(sqrt(a**2 + b**2),2)

    print(result)
    return result

if __name__ == '__main__':
    dist = main(A,B)
```








#Return all numbers divisible by the given number in a sequence from start to stop
>Write a program that will return a list of numbers divisible by given number
in interval from a to b. The program should take 3 inputs, divisor, start and
stop points of the interval.

**Example:**
```
Input: divisor = 3, start = 3, stop = 9

Output: [3,6,9]


If divisor is 0, the result should be a string 'Cannot divide by zero'
```
**Task:**
```
divisor = 1
start = 1
stop = 10

def main(divisor, start, stop):

    # create the variable, where you will store the result

    # check that the divisor is not zero
    # if not then iterate over the numbers between start and stop (including)
    # use modulo operator to check whether each of those numbers is divisible
    # by divisor


    return result

if __name__ == '__main__':
    main()
```









#Count vowels and consonants in a given text.
>Write a Python program that will count how many vowels and consonants are in
a given string.

>The program should take as input a string and output a dictionary in form:
{'consonants':count_c, 'vowels':count_v}
count_c should be count of consonants
count_v - count of vowels

**Example:**
```
input sentence: 'a speech sound that is produced by comparatively open configuration of the vocal tract'
output: {'consonants':43, 'vowels':30}
```
**Task:**
```
sentence ='''
Pandas is excellent at manipulating large amounts of data and summarizing
it in multiple text and visual representations. Without much effort, pandas
supports output to CSV, Excel, HTML, json and more.
'''


# function takes only one input - the sentence is a string
def main(sentence):
    # create two variables - one that will store a sequence of vowels and
    # the other to store the sequence of all the consonants

    # prepare the variable that will store dictionary where the counts of
    # vowels and consonants will be stored
    counts = {'vowels':0, 'consonants':0}

    # loop over the sentence and determine, whether a letter belongs to
    # the group of vowels or consonants



    return counts


if __name__=='__main__':

    main(sentence)
```









#Create echo like sentences
>Write a Python program that will create "echo sentences". Each word in
the sentence we will feed in, should be repeated n number of times. The number
of repetitions and the sentence to be manipulated are inputs into our function

**Example:**
```
If supplied the sentence:

    'I do not want to work today'

The output should be:

    'I I I do do do not not not want want want to to to work work work today today today'
```
>You can also use the print() function to see the resulting string.

>The resulting sentence cannot begin with space, unless the input sentence contained it

**Task:**
```
sentence = 'I do not want to work today'
num_repeat = 3

def main(sentence,num_repeat):
    # get words using split method

    # create variable in this you will store the resulting string

    # iterate over the list of words you got in the previous step and repeat
    # each word num_repeat times

    # return result and strip spaces at its beginning and end



if __name__ == '__main__':
    main(sentence,num_repeat)
```











#task #8: Create nice basic pivot table counting the number of elements in a sequence
>Create a program that will print out how many times does every object occur inside
any list, tuple or string (counts of individual characters).
The program output should be a dictionary with counts associated with each value.

**Example:**
```
Input: [1,21,5,3,5,8,321,1,2,2,32,6,9,1,4,6,3,1,2]
Output value: {'1': 4, '8': 1, '321': 1, '4': 1, '3': 2, '6': 2, '21': 1, '32': 1, '5': 2, '2': 3, '9': 1}
```
* Bonus 1 (not tested):
Make a program to recognize, whether the input is list, tuple or a string. If it is
a string, then return the counts for each word.

* Bonus 2 (not tested):
Print the result also as a table with nicely aligned numbers ordered from the
most frequent occurence to the least frequent occurence.

**Example:**
```
The above example printed to the screen - see the useful string methods section.
Printed to the screen:

 Item |Count
=============
 1    |  4
 2    |  3
 3    |  2
 5    |  2
 6    |  2
 32   |  1
 4    |  1
 321  |  1
 8    |  1
 9    |  1
 21   |  1
```
**Task:**
```
seq = [1,21,5,3,5,8,321,1,2,2,32,6,9,1,4,6,3,1,2]

def main(seq):
    # check if the input sequence is empty - if so then the result should be
    # empty string


    # create a dictionary that will collect counts of each item in the sequence
    counts = {}
    
if __name__=='__main__':
    main(seq)
```
**Bonus 1**
```
If you want to count entire words, now it is time to split the string to words

Iterate over the sequence and increase the count of the item found

You can now return the result or you can continue trying to print the results nicely
```
**Bonus 2**
```
Find out, what column widths will need each column of the table - use the len(), max(), 
and str() (if the item is a number) functions to find the length of the longest item in
the column - beware, maybe the column headers will be the longest items in the column 
column to the left will be made of dictionary keys (items), the right occurence will be
associated values

Now it is time to print each row on new line

First print the header - center the 'Item' and 'Count' words inside the string (str.center() method)

Now print each row with item and associated value - use the center() method and the width of each column

Return counts
```








#Primenumber
>Even though everybody knows, what prime numbers are, and how to identify them, it is little 
bit more complicated with teaching this to a computer. Sometimes we would like to know, wheter 
a huge number is a prime number. Average human is able to recognize prime numbers only for smaller 
values. For the bigger ones, we will need computer's help. Prime numbers are heavily used in cryptography 
or generation of pseudo random numbers and if we searched more, we would found more more examples of their 
usefulness. So the first step for determining, whether a number is prime is the ability of their generation. 
Your program should be therefore able not only to determine whether a number is a prime number, but also 
to generate all the prime numbers up to the number being examined.

**Example:**
```
Input: Please enter the number: 421321
Output: Number 421321 is not a prime number.
```









#Bulls and Cows
>First of all, the computer will generate a 4-digit secret number. The digits must be all different. 
Then, in turn, the user tries to guess their computer's number. The user inputs a number and the 
computer responds with the number of matching digits. If the matching digits are in their right 
positions, they are "bulls", if in different positions, they are "cows".

**Example:**
```
For example, let's say the number is 2017. A sample interaction might look like this:

Hi there!
I've generated a random 4 digit number for you.
Let's play a bulls and cows game.
Enter a number
>>> 1234
0 bulls, 2 cows
>>> 6147
1 bull, 1 cow
>>> 2417
3 bulls, 0 cows
>>> 2017
Correct, you've guessed the right number in 4 guesses!
That's {amazing, average, not so good, ...}
```









#Birthnumber
>Program birthnumber.py bude pracovať v 2 módoch - buď bude generovať nové rodné číslo (žiaden argument) 
alebo bude verifikovať poskytnuté číslo z príkazového riadku (1 argument).

* Podmienky na generovanie a overenie rodného čísla sú nasledovné:

    * číslo musí obsahovať 10 čisel (pre ľudí, ktorí sa narodili po roku 1954) alebo musí osahovať 9 čisel (pre ľudí, ktorí sa narodili do roku 1953)
    * číslo má 2 časti - dátum narodenia a kontrolný súčet (CCCC) v tvare YYMMDD/CCCC
    * celé číslo musí byť delitelné číslom 11
    * ženy majú v mesiaci narodenia pridanú hodnotu 50

**Example**
```
861107/2239 je validné rodné číslo pre muža, ktorý sa narodil 7.11.1986. 
025226/1306 je validné rodné číslo ženy narodenej 26.02.2002.
```

>Pre spustenie overenia rodného čísla použijeme príkaz:
```
 $ birthnumber.py YYMMDD/CCCC
``` 
 >kde YYMMDD/CCCC je konkrétne rodné číslo, ktoré chceme overiť.

>Očakávaný výstup v prípade nesprávneho rodného čísla je hláška s chybami, ktoré počas validácie nastali. 

**Example**
```
 Provided birth number is INVALID.
 <reason>
 <another-reason>
```
>Pre generovanie to bude interaktívny proces:
```
 $ birthnumber.py
```
**Output**
```
Day of the birth [YYYY-MM-DD]: <user input>
Sex [M/F]: <user input>
Generated birth number: YYMMDD/CCCC
```


#Date and Time
##Skeleton: weekday.py
> This program should take in date representation as tuple of format (year,month,day) and return 
the number of the day of the week on which the given date falls.

* 1 = Monday
* 2 = Tuesday
* 3 = Wednesday
* 4 = Thursday
* 5 = Friday
* 6 = Saturday
* 7 = Sunday

>The program should also handle case, when non-existent date is supplied (2015,2,29). If such date is 
supplied, the program should print out: 'Non-existent date' And return value should be 0. Examples in 
the examples section.
In order to be able to determine what weekday falls on specific date, we need to have a point of 
reference - we need to know at least one match between a date and and weekday. This reference day will 
be the beginning of Unix epoch: 1.1.1970 which corresponds to weekday: Thursday, therefore it a date earlier 
than 1.1.1970 is supplied, the program should return value -1.
**Example**
```
weekday.py (2017,4,7)
6
```
```
weekday.py (1969,12,31)
-1
```
```
weekday.py (2015,2,29)
Non-existent date
0
```








#Caesar cipher
>Now we will dive into the world of cryptography. Our goal is to use the old Caesar cipher technique 
to encode our messages. But how the Caesar cipher works? Caesar cipher encryption technique is named 
after Julius Caesar, who used it in his private correspondce. It is based on the notion of encoding each 
letter by shifting arbitrary number of positions in alphabet. Alphabet is ordered and so letter 'A' can 
be thought of as being at position 1, 'B' at position 2 etc. If we decided to encrypt our message with shift 
value of 3, for example for a message 'ABBA', we would get string 'DEED'. The encryption offset stays the same 
for each encoded character. We have replaced 'D' for 'A', becayse it was 3 places away from 'A' and the same 
is valid for the substitution of 'E' for 'B'.
Now it is your task to make a program that will perform encoding and decoding of messages using Caesar cipher. 
The program should read a plain text file on your disk, encrypt its content and write this encrypted content into a new file. 
The program should take inputs from the command line.

**Example**
```
caesar.py my_file.txt 6
The content has been successfully encrypted
```
**Bonus**
```
ARGUMENT PARSING
You can make your program even better by implementing command line argument parsing. Try to find out, what library 
could help you here. The resulting program could be ran as follows: $ python caesar.py --file "my_file.txt" --offset 6 
The content has been successfully encrypted And it should provide user with help if 
called using "-h" or "--help" flag: $ python caesar.py --help BRUTE FORCE DECRYPTION You could also create a program 
that will decrypt the Caesar cipher without knowing the offset constant.
```









#Dragon Curve
>Dragon curve is a fractal that is naturally created when folding a paper for example. Create a program that will draw 
so called dragon curve of any size. Example of dragon curve after 12 iterations: Dragon curve gets twice longer each 
iteration. We can color the line, that is created during single iteration: You can also try to create combined dragon 
curves, which lines will have different coloures.







#Combinatorics
>Without Repetition:

>Represents the act of arranging all the members of a set into some sequence or order. To get all the permutations of a sequence means to find all the possible orderings of elements in a set. The elements cannot repeat.

>There can be permutations with and without repetition:
- Number of permutations without repetition of n elements is n!
- Number of permutations with repetition of n elements is nn
>And if we are just selecting a subset of length k from a set, then:
- Number of permutations without repetition of n elements is n!/(n-k)!
- Number of permutations with repetition of n elements is nk

**Links**
https://www.mathsisfun.com/combinatorics/combinations-permutations.html
https://betterexplained.com/articles/easy-permutations-and-combinations/

**Task**
```
Create a program that will return all permutations of a given sequence.

```
**Example**
```Please enter the list: ['A', 'B', 'C', 'D']
With repetition?[y/n]: n
Subset lengths (press enter for the length of the input list):

There are 24 permutations without repetition:
[['A', 'B', 'C', 'D'], 
['A', 'B', 'D', 'C'], 
['A', 'C', 'B', 'D'], 
['A', 'C', 'D', 'B'], 
['A', 'D', 'B', 'C'], 
['A', 'D', 'C', 'B'], 
['B', 'A', 'C', 'D'], 
['B', 'A', 'D', 'C'], 
['B', 'C', 'A', 'D'], 
['B', 'C', 'D', 'A'], 
['B', 'D', 'A', 'C'], 
['B', 'D', 'C', 'A'], 
['C', 'A', 'B', 'D'], 
['C', 'A', 'D', 'B'], 
['C', 'B', 'A', 'D'], 
['C', 'B', 'D', 'A'], 
['C', 'D', 'A', 'B'], 
['C', 'D', 'B', 'A'], 
['D', 'A', 'B', 'C'], 
['D', 'A', 'C', 'B'], 
['D', 'B', 'A', 'C'], 
['D', 'B', 'C', 'A'], 
['D', 'C', 'A', 'B'], 
['D', 'C', 'B', 'A']]
```
>USED FOR

- sorting
- anagrams
- brute force password cracking
>COMBINATIONS

Selecting k elements from a set of length n, where the order does not matter. That means that (1,2,3) is the same as any of the tuples (3,2,1), (2,3,1), (3,1,2),(2,1,3),(1,3,2).

The program, that will list all combinations for us, should answer the questions, what are the ways of selecting items from a collection, such that (unlike permutations) the order of selection does not matter.
There can be combinations with and without repetition, when selecting k elements from the set:
- Number of combinations without repetition of k elements is n!/((n-k)!k!)
- Number of combinations with repetition of k elements is (n-1+k)!/((n-1)!k!)

**Task**
```
Create a program that will return all combinations of k items selected from a given sequence.

```
**Example**
```
Please enter the list: ['A', 'B', 'C', 'D']
With repetition?[y/n]: n
Number of items selected (press enter for the length of the input list):

There are 4 combinations without repetition:

[['A', 'B', 'C'], 
['A', 'B', 'D'], 
['A', 'C', 'D'], 
['B', 'C', 'D']]
```
>USED FOR

Probability calculation








#Anagram
>In many natural languages we can find some pairs of words which could be transformed to each other by changing 
the order of letters. I.e. they consist of the same set of letters, for example: act - cat, ate - eat - tea.
Such words are called anagrams and as we see in the third example sometimes there are more than two words.
Your task is to find out the amount of anagrams for given word by the dictionary.

**Source of the words:**
http://hack.engeto.com/words.txt

**Example**
```
Start the program and prompt the user for a word. You can specify options to extend the funcitonality of the program, but it's up to you how you'll implement it and what options you'll decide to use. In general, the program should be able to run with:
[test@test ]$ ./anagrams.py
Provide the word to find anagrams for: slot 
The output should be:

There are 2 anagrams we've been able to find for the word slot:
 * lots
 * lost
 ```
 
 ```
* define a function to load the dictionary to internal structure we will load it from external file
 
def load_dict():
    pass

* process the input word we're working with

* logic behind the anagram program
* ideal case - work with the internal structure (array) with all
words from the dictionary and try to find proper letters in those words
* it is up to you how you'll handle this area, try to figure this out

* print the requested anagrams
```
**Bonus**
```
Process multiple words
Text file as source of words
Optimize the algorithm to be most efficient
```






#Hangman
>Hangman is a simple game for one player. The computer will choose a word, 
phrase or sentence and the player tries to guess it by suggesting letters 
or numbers, within a certain number of guesses.

**Bonus**
```
Graphical interface
Text file as source of words
Stopwatch
Ending the game after 6 unsuccessfull attempts
```
**Example**
```
Just run the game and start guessing. You can specify options to extend 
the funcitonality of the program, but it's up to you how you'll implement it 
and what options you'll decide to use. In general, the program should be able to run with:
```
```
hangman.py
Let's guess the word: _ _ _ _ _ _ _
```
```
define a function for generating a random word
def choose_word():
    pass

word = choose_word()

# main loop
while True:
    # print out current state of the game
    # for example - We're guessing the word: _ _ _ _ _ _ _ _ _ _

    # let's get a letter from the user
    letter = input("Guess the letter: ")

    # make sure the letter is only one character

    # print the letter to see if everything is ok by now
    print("You guessed", letter)

    # determine if the letter is in the word

    # check if the word is not guessed in its entirety
```





#Labyrinth
>Labyrinths are part of many games. Creating them can be tricky as well as finding the way out. 
Finding a route from place A to place B has many other use cases (or better the shortest one), 
like navigations, self-driven cars and more. This task will provide you an introduction to the 
topic of finding paths. First you will be given few labyrinths - mazes in which your program 
will have to find the path from point A to point B. You will need to implement algorithms as 
breadth first search of depth first search (or you can use any other you prefer).

**Task**
* Download the file mazes.py. The file contains mazes, your future script should be able to traverse
* Implement function that will take maze as argument and will return a string representing the sequence of steps (example: 'SSSSEEENEESS'- S = South, N = North etc.) leading from the starting point to the goal. Permitted are only moves up - 'S', down - 'N', left - 'W', right - 'E'.
* Implement the function that will generate randomly distributed maze
* Implement a function that will depict the maze in ASCII art
* Put it all together into one program that will generate random maze, determine the starting point and end point, then find the shortest path and lastly print it all to the command line in ASCII art
* Prepared mazes are represented by lists of lists of zeros and ones. Ones represent walls and zeros are paths which you can use to move on

```
[[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
 [1, 0, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1],
 [1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1],
 [1, 0, 1, 0, 1, 1, 1, 1, 1, 1, 0, 1],
 [1, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 1],
 [1, 0, 0, 0, 1, 1, 0, 1, 1, 1, 0, 1],
 [1, 0, 1, 0, 0, 0, 0, 1, 0, 1, 1, 1],
 [1, 0, 1, 1, 0, 1, 0, 0, 0, 0, 0, 1],
 [1, 0, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1],
 [1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
```


**Example**
>Program returning the path from point A to B

```
[test@test ]$ ./find_path.py
'SSSSEEEENNNNWNNEEEESSS'
```
>Program to generate maze in ASCII art

```
[test@test ]$ ./generate_maze.py
+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+
|     |              |     |        |  |        |
+  +  +  +--+--+  +  +  +  +  +--+  +  +  +--+  +
|  |     |  |     |     |  |  |     |        |  |
+  +--+--+  +  +--+--+--+  +  +  +--+--+--+--+  +
|        |  |  |           |  |  |        |     |
+--+--+  +  +  +--+  +--+--+  +  +  +--+  +  +--+
|     |  |  |     |        |  |  |  |     |     |
+  +  +  +  +--+  +--+--+  +  +  +  +  +--+--+  +
|  |  |     |     |     |     |     |  |     |  |
+  +  +--+  +  +--+  +  +--+--+--+--+  +  +  +  +
|  |     |  |  |     |  |           |     |     |
+  +--+--+--+  +  +--+  +  +  +--+--+--+--+--+  +
|     |     |     |     |  |                 |  |
+--+  +  +  +--+--+  +--+  +--+--+--+--+--+  +  +
|        |           |                    |     |
+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+
```
>Progam to generate maze in ASCII art

```
[test@test ]$ ./solve_maze.py
+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+
|xxxxx|xxxxxxxxxxxxx |xxxxx|xxxxxxxx|  |        |
+  +  +x +--+--+  +x + x+ x+x +--+ x+  +  +--+  +
|  | x x |  |     |xxxxx| x|x |xxxxx|        |  |
+  +--+--+  +  +--+--+--+ x+x +x +--+--+--+--+  +
|        |  |  |   xxxxxxxx|x |x |xxxxxxxx|     |
+--+--+  +  +  +--+x +--+--+x +x +x +--+ x+  +--+
|     |  |  |     |xxxxxxxx|x |x |x |xxxxx|     |
+  +  +  +  +--+  +--+--+ x+x +x +x +x +--+--+  +
|  |  |     |     |     | x x |xxxxx|x | x x |  |
+  +  +--+  +  +--+  +  +--+--+--+--+x + x+x +  +
|  |     |  |  |     |  |           |xxxxx|xxxxx|
+  +--+--+--+  +  +--+  +  +  +--+--+--+--+--+ x+
|     |     |     |     |  |                 | x|
+--+  +  +  +--+--+  +--+  +--+--+--+--+--+  + x+
|        |           |                    |    x|
+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+--+

```
**Bonus**
* Create a pygame GUI maze generator

* Create a pygame GUI maze traversal

>maze.py:
```
#in the following mazes, 0 represent path, 1 walls
maze1=[
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1],
        [1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 0, 1, 1, 1, 1, 1, 1, 0, 1],
        [1, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 1, 1, 0, 1, 1, 1, 0, 1],
        [1, 0, 1, 0, 0, 0, 0, 1, 0, 1, 1, 1],
        [1, 0, 1, 1, 0, 1, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1],
        [1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
maze2=[
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]),
maze3 [
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 1, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 1, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 1, 1],
        [1, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 1, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]),
maze4 = [
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1],
        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 1],
        [1, 0, 1, 0, 0, 0, 1, 0, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]),
maze5 = [
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 1, 0, 1, 0, 1, 1, 1, 0, 1],
        [1, 0, 1, 1, 0, 1, 0, 1, 0, 1, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 1],
        [1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 0, 1],
        [1, 0, 0, 0, 0, 1, 1, 1, 0, 1, 1, 1],
        [1, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 1, 0, 1, 1, 1, 1, 1, 0, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1],
        [1, 0, 1, 0, 1, 0, 1, 1, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]),
maze6 =[
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 1, 1, 0, 1, 1, 1, 1, 0, 1, 1, 1],
        [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 0, 1, 1, 1, 0, 1, 1, 1, 1, 1, 1],
        [1, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 1],
        [1, 1, 0, 1, 1, 1, 1, 1, 1, 0, 1, 1],
        [1, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 0, 1, 0, 0, 1, 0, 1],
        [1, 0, 0, 0, 0, 0, 1, 1, 1, 1, 1, 1],
        [1, 0, 1, 1, 1, 0, 0, 0, 0, 0, 0, 1],
        [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]
```






#Game Of Life
>For those, who would like to extend their knowledge in Python data structures and put some life 
into their computer in the process. Game of Life is a program, that simulates cellular life 
on a two dimensional grid with simple rules. Every cell in the grid sumulates a cell, that can be 
either dead or alive. In every step of the simulation, the cell might be revived, die or maintain 
its state (alive, dead) based on circumstances around the cell. With its simple rules, 
the Game of Life created patterns that are constantly alive and evolving, moving on the grid and 
creating new life.
In this assignment, you'll create ground for smokers, oscillators, cannons, mathusalems and other 
forms of organism created in the Game of Life. You'll test your skill in conditions, loops, lists, 
indexing and strings. It is avised to use some graphical library as well.

>graphics.py:
```
"""Simple object oriented graphics library  

The library is designed to make it very easy for novice programmers to
experiment with computer graphics in an object oriented fashion. It is
written by John Zelle for use with the book "Python Programming: An
Introduction to Computer Science" (Franklin, Beedle & Associates).

LICENSE: This is open-source software released under the terms of the
GPL (http://www.gnu.org/licenses/gpl.html).

PLATFORMS: The package is a wrapper around Tkinter and should run on
any platform where Tkinter is available.

INSTALLATION: Put this file somewhere where Python can see it.

OVERVIEW: There are two kinds of objects in the library. The GraphWin
class implements a window where drawing can be done and various
GraphicsObjects are provided that can be drawn into a GraphWin. As a
simple example, here is a complete program to draw a circle of radius
10 centered in a 100x100 window:

--------------------------------------------------------------------
from graphics import *

def main():
    win = GraphWin("My Circle", 100, 100)
    c = Circle(Point(50,50), 10)
    c.draw(win)
    win.getMouse() # Pause to view result
    win.close()    # Close window when done

main()
--------------------------------------------------------------------
GraphWin objects support coordinate transformation through the
setCoords method and mouse and keyboard interaction methods.

The library provides the following graphical objects:
    Point
    Line
    Circle
    Oval
    Rectangle
    Polygon
    Text
    Entry (for text-based input)
    Image

Various attributes of graphical objects can be set such as
outline-color, fill-color and line-width. Graphical objects also
support moving and hiding for animation effects.

The library also provides a very simple class for pixel-based image
manipulation, Pixmap. A pixmap can be loaded from a file and displayed
using an Image object. Both getPixel and setPixel methods are provided
for manipulating the image.

DOCUMENTATION: For complete documentation, see Chapter 4 of "Python
Programming: An Introduction to Computer Science" by John Zelle,
published by Franklin, Beedle & Associates.  Also see
http://mcsp.wartburg.edu/zelle/python for a quick reference"""

__version__ = "5.0"

# Version 5 8/26/2016
#     * update at bottom to fix MacOS issue causing askopenfile() to hang
#     * update takes an optional parameter specifying update rate
#     * Entry objects get focus when drawn
#     * __repr_ for all objects
#     * fixed offset problem in window, made canvas borderless

# Version 4.3 4/25/2014
#     * Fixed Image getPixel to work with Python 3.4, TK 8.6 (tuple type handling)
#     * Added interactive keyboard input (getKey and checkKey) to GraphWin
#     * Modified setCoords to cause redraw of current objects, thus
#       changing the view. This supports scrolling around via setCoords.
#
# Version 4.2 5/26/2011
#     * Modified Image to allow multiple undraws like other GraphicsObjects
# Version 4.1 12/29/2009
#     * Merged Pixmap and Image class. Old Pixmap removed, use Image.
# Version 4.0.1 10/08/2009
#     * Modified the autoflush on GraphWin to default to True
#     * Autoflush check on close, setBackground
#     * Fixed getMouse to flush pending clicks at entry
# Version 4.0 08/2009
#     * Reverted to non-threaded version. The advantages (robustness,
#         efficiency, ability to use with other Tk code, etc.) outweigh
#         the disadvantage that interactive use with IDLE is slightly more
#         cumbersome.
#     * Modified to run in either Python 2.x or 3.x (same file).
#     * Added Image.getPixmap()
#     * Added update() -- stand alone function to cause any pending
#           graphics changes to display.
#
# Version 3.4 10/16/07
#     Fixed GraphicsError to avoid "exploded" error messages.
# Version 3.3 8/8/06
#     Added checkMouse method to GraphWin
# Version 3.2.3
#     Fixed error in Polygon init spotted by Andrew Harrington
#     Fixed improper threading in Image constructor
# Version 3.2.2 5/30/05
#     Cleaned up handling of exceptions in Tk thread. The graphics package
#     now raises an exception if attempt is made to communicate with
#     a dead Tk thread.
# Version 3.2.1 5/22/05
#     Added shutdown function for tk thread to eliminate race-condition
#        error "chatter" when main thread terminates
#     Renamed various private globals with _
# Version 3.2 5/4/05
#     Added Pixmap object for simple image manipulation.
# Version 3.1 4/13/05
#     Improved the Tk thread communication so that most Tk calls
#        do not have to wait for synchonization with the Tk thread.
#        (see _tkCall and _tkExec)
# Version 3.0 12/30/04
#     Implemented Tk event loop in separate thread. Should now work
#        interactively with IDLE. Undocumented autoflush feature is
#        no longer necessary. Its default is now False (off). It may
#        be removed in a future version.
#     Better handling of errors regarding operations on windows that
#       have been closed.
#     Addition of an isClosed method to GraphWindow class.

# Version 2.2 8/26/04
#     Fixed cloning bug reported by Joseph Oldham.
#     Now implements deep copy of config info.
# Version 2.1 1/15/04
#     Added autoflush option to GraphWin. When True (default) updates on
#        the window are done after each action. This makes some graphics
#        intensive programs sluggish. Turning off autoflush causes updates
#        to happen during idle periods or when flush is called.
# Version 2.0
#     Updated Documentation
#     Made Polygon accept a list of Points in constructor
#     Made all drawing functions call TK update for easier animations
#          and to make the overall package work better with
#          Python 2.3 and IDLE 1.0 under Windows (still some issues).
#     Removed vestigial turtle graphics.
#     Added ability to configure font for Entry objects (analogous to Text)
#     Added setTextColor for Text as an alias of setFill
#     Changed to class-style exceptions
#     Fixed cloning of Text objects

# Version 1.6
#     Fixed Entry so StringVar uses _root as master, solves weird
#            interaction with shell in Idle
#     Fixed bug in setCoords. X and Y coordinates can increase in
#           "non-intuitive" direction.
#     Tweaked wm_protocol so window is not resizable and kill box closes.

# Version 1.5
#     Fixed bug in Entry. Can now define entry before creating a
#     GraphWin. All GraphWins are now toplevel windows and share
#     a fixed root (called _root).

# Version 1.4
#     Fixed Garbage collection of Tkinter images bug.
#     Added ability to set text atttributes.
#     Added Entry boxes.

import time, os, sys

try:  # import as appropriate for 2.x vs. 3.x
   import tkinter as tk
except:
   import Tkinter as tk


##########################################################################
# Module Exceptions

class GraphicsError(Exception):
    """Generic error class for graphics module exceptions."""
    pass

OBJ_ALREADY_DRAWN = "Object currently drawn"
UNSUPPORTED_METHOD = "Object doesn't support operation"
BAD_OPTION = "Illegal option value"

##########################################################################
# global variables and funtions

_root = tk.Tk()
_root.withdraw()

_update_lasttime = time.time()

def update(rate=None):
    global _update_lasttime
    if rate:
        now = time.time()
        pauseLength = 1/rate-(now-_update_lasttime)
        if pauseLength > 0:
            time.sleep(pauseLength)
            _update_lasttime = now + pauseLength
        else:
            _update_lasttime = now

    _root.update()

############################################################################
# Graphics classes start here
        
class GraphWin(tk.Canvas):

    """A GraphWin is a toplevel window for displaying graphics."""

    def __init__(self, title="Graphics Window",
                 width=200, height=200, autoflush=True):
        assert type(title) == type(""), "Title must be a string"
        master = tk.Toplevel(_root)
        master.protocol("WM_DELETE_WINDOW", self.close)
        tk.Canvas.__init__(self, master, width=width, height=height,
                           highlightthickness=0, bd=0)
        self.master.title(title)
        self.pack()
        master.resizable(0,0)
        self.foreground = "black"
        self.items = []
        self.mouseX = None
        self.mouseY = None
        self.bind("<Button-1>", self._onClick)
        self.bind_all("<Key>", self._onKey)
        self.height = int(height)
        self.width = int(width)
        self.autoflush = autoflush
        self._mouseCallback = None
        self.trans = None
        self.closed = False
        master.lift()
        self.lastKey = ""
        if autoflush: _root.update()

    def __repr__(self):
        if self.isClosed():
            return "<Closed GraphWin>"
        else:
            return "GraphWin('{}', {}, {})".format(self.master.title(),
                                             self.getWidth(),
                                             self.getHeight())

    def __str__(self):
        return repr(self)
     
    def __checkOpen(self):
        if self.closed:
            raise GraphicsError("window is closed")

    def _onKey(self, evnt):
        self.lastKey = evnt.keysym


    def setBackground(self, color):
        """Set background color of the window"""
        self.__checkOpen()
        self.config(bg=color)
        self.__autoflush()
        
    def setCoords(self, x1, y1, x2, y2):
        """Set coordinates of window to run from (x1,y1) in the
        lower-left corner to (x2,y2) in the upper-right corner."""
        self.trans = Transform(self.width, self.height, x1, y1, x2, y2)
        self.redraw()

    def close(self):
        """Close the window"""

        if self.closed: return
        self.closed = True
        self.master.destroy()
        self.__autoflush()


    def isClosed(self):
        return self.closed


    def isOpen(self):
        return not self.closed


    def __autoflush(self):
        if self.autoflush:
            _root.update()

    
    def plot(self, x, y, color="black"):
        """Set pixel (x,y) to the given color"""
        self.__checkOpen()
        xs,ys = self.toScreen(x,y)
        self.create_line(xs,ys,xs+1,ys, fill=color)
        self.__autoflush()
        
    def plotPixel(self, x, y, color="black"):
        """Set pixel raw (independent of window coordinates) pixel
        (x,y) to color"""
        self.__checkOpen()
        self.create_line(x,y,x+1,y, fill=color)
        self.__autoflush()
      
    def flush(self):
        """Update drawing to the window"""
        self.__checkOpen()
        self.update_idletasks()
        
    def getMouse(self):
        """Wait for mouse click and return Point object representing
        the click"""
        self.update()      # flush any prior clicks
        self.mouseX = None
        self.mouseY = None
        while self.mouseX == None or self.mouseY == None:
            self.update()
            if self.isClosed(): raise GraphicsError("getMouse in closed window")
            time.sleep(.1) # give up thread
        x,y = self.toWorld(self.mouseX, self.mouseY)
        self.mouseX = None
        self.mouseY = None
        return Point(x,y)

    def checkMouse(self):
        """Return last mouse click or None if mouse has
        not been clicked since last call"""
        if self.isClosed():
            raise GraphicsError("checkMouse in closed window")
        self.update()
        if self.mouseX != None and self.mouseY != None:
            x,y = self.toWorld(self.mouseX, self.mouseY)
            self.mouseX = None
            self.mouseY = None
            return Point(x,y)
        else:
            return None

    def getKey(self):
        """Wait for user to press a key and return it as a string."""
        self.lastKey = ""
        while self.lastKey == "":
            self.update()
            if self.isClosed(): raise GraphicsError("getKey in closed window")
            time.sleep(.1) # give up thread

        key = self.lastKey
        self.lastKey = ""
        return key

    def checkKey(self):
        """Return last key pressed or None if no key pressed since last call"""
        if self.isClosed():
            raise GraphicsError("checkKey in closed window")
        self.update()
        key = self.lastKey
        self.lastKey = ""
        return key
            
    def getHeight(self):
        """Return the height of the window"""
        return self.height
        
    def getWidth(self):
        """Return the width of the window"""
        return self.width
    
    def toScreen(self, x, y):
        trans = self.trans
        if trans:
            return self.trans.screen(x,y)
        else:
            return x,y
                      
    def toWorld(self, x, y):
        trans = self.trans
        if trans:
            return self.trans.world(x,y)
        else:
            return x,y
        
    def setMouseHandler(self, func):
        self._mouseCallback = func
        
    def _onClick(self, e):
        self.mouseX = e.x
        self.mouseY = e.y
        if self._mouseCallback:
            self._mouseCallback(Point(e.x, e.y))

    def addItem(self, item):
        self.items.append(item)

    def delItem(self, item):
        self.items.remove(item)

    def redraw(self):
        for item in self.items[:]:
            item.undraw()
            item.draw(self)
        self.update()
        
                      
class Transform:

    """Internal class for 2-D coordinate transformations"""
    
    def __init__(self, w, h, xlow, ylow, xhigh, yhigh):
        # w, h are width and height of window
        # (xlow,ylow) coordinates of lower-left [raw (0,h-1)]
        # (xhigh,yhigh) coordinates of upper-right [raw (w-1,0)]
        xspan = (xhigh-xlow)
        yspan = (yhigh-ylow)
        self.xbase = xlow
        self.ybase = yhigh
        self.xscale = xspan/float(w-1)
        self.yscale = yspan/float(h-1)
        
    def screen(self,x,y):
        # Returns x,y in screen (actually window) coordinates
        xs = (x-self.xbase) / self.xscale
        ys = (self.ybase-y) / self.yscale
        return int(xs+0.5),int(ys+0.5)
        
    def world(self,xs,ys):
        # Returns xs,ys in world coordinates
        x = xs*self.xscale + self.xbase
        y = self.ybase - ys*self.yscale
        return x,y


# Default values for various item configuration options. Only a subset of
#   keys may be present in the configuration dictionary for a given item
DEFAULT_CONFIG = {"fill":"",
      "outline":"black",
      "width":"1",
      "arrow":"none",
      "text":"",
      "justify":"center",
                  "font": ("helvetica", 12, "normal")}

class GraphicsObject:

    """Generic base class for all of the drawable objects"""
    # A subclass of GraphicsObject should override _draw and
    #   and _move methods.
    
    def __init__(self, options):
        # options is a list of strings indicating which options are
        # legal for this object.
        
        # When an object is drawn, canvas is set to the GraphWin(canvas)
        #    object where it is drawn and id is the TK identifier of the
        #    drawn shape.
        self.canvas = None
        self.id = None

        # config is the dictionary of configuration options for the widget.
        config = {}
        for option in options:
            config[option] = DEFAULT_CONFIG[option]
        self.config = config
        
    def setFill(self, color):
        """Set interior color to color"""
        self._reconfig("fill", color)
        
    def setOutline(self, color):
        """Set outline color to color"""
        self._reconfig("outline", color)
        
    def setWidth(self, width):
        """Set line weight to width"""
        self._reconfig("width", width)

    def draw(self, graphwin):

        """Draw the object in graphwin, which should be a GraphWin
        object.  A GraphicsObject may only be drawn into one
        window. Raises an error if attempt made to draw an object that
        is already visible."""

        if self.canvas and not self.canvas.isClosed(): raise GraphicsError(OBJ_ALREADY_DRAWN)
        if graphwin.isClosed(): raise GraphicsError("Can't draw to closed window")
        self.canvas = graphwin
        self.id = self._draw(graphwin, self.config)
        graphwin.addItem(self)
        if graphwin.autoflush:
            _root.update()
        return self

            
    def undraw(self):

        """Undraw the object (i.e. hide it). Returns silently if the
        object is not currently drawn."""
        
        if not self.canvas: return
        if not self.canvas.isClosed():
            self.canvas.delete(self.id)
            self.canvas.delItem(self)
            if self.canvas.autoflush:
                _root.update()
        self.canvas = None
        self.id = None


    def move(self, dx, dy):

        """move object dx units in x direction and dy units in y
        direction"""
        
        self._move(dx,dy)
        canvas = self.canvas
        if canvas and not canvas.isClosed():
            trans = canvas.trans
            if trans:
                x = dx/ trans.xscale 
                y = -dy / trans.yscale
            else:
                x = dx
                y = dy
            self.canvas.move(self.id, x, y)
            if canvas.autoflush:
                _root.update()
           
    def _reconfig(self, option, setting):
        # Internal method for changing configuration of the object
        # Raises an error if the option does not exist in the config
        #    dictionary for this object
        if option not in self.config:
            raise GraphicsError(UNSUPPORTED_METHOD)
        options = self.config
        options[option] = setting
        if self.canvas and not self.canvas.isClosed():
            self.canvas.itemconfig(self.id, options)
            if self.canvas.autoflush:
                _root.update()


    def _draw(self, canvas, options):
        """draws appropriate figure on canvas with options provided
        Returns Tk id of item drawn"""
        pass # must override in subclass


    def _move(self, dx, dy):
        """updates internal state of object to move it dx,dy units"""
        pass # must override in subclass

         
class Point(GraphicsObject):
    def __init__(self, x, y):
        GraphicsObject.__init__(self, ["outline", "fill"])
        self.setFill = self.setOutline
        self.x = float(x)
        self.y = float(y)

    def __repr__(self):
        return "Point({}, {})".format(self.x, self.y)
        
    def _draw(self, canvas, options):
        x,y = canvas.toScreen(self.x,self.y)
        return canvas.create_rectangle(x,y,x+1,y+1,options)
        
    def _move(self, dx, dy):
        self.x = self.x + dx
        self.y = self.y + dy
        
    def clone(self):
        other = Point(self.x,self.y)
        other.config = self.config.copy()
        return other
                
    def getX(self): return self.x
    def getY(self): return self.y

class _BBox(GraphicsObject):
    # Internal base class for objects represented by bounding box
    # (opposite corners) Line segment is a degenerate case.
    
    def __init__(self, p1, p2, options=["outline","width","fill"]):
        GraphicsObject.__init__(self, options)
        self.p1 = p1.clone()
        self.p2 = p2.clone()

    def _move(self, dx, dy):
        self.p1.x = self.p1.x + dx
        self.p1.y = self.p1.y + dy
        self.p2.x = self.p2.x + dx
        self.p2.y = self.p2.y  + dy
                
    def getP1(self): return self.p1.clone()

    def getP2(self): return self.p2.clone()
    
    def getCenter(self):
        p1 = self.p1
        p2 = self.p2
        return Point((p1.x+p2.x)/2.0, (p1.y+p2.y)/2.0)

    
class Rectangle(_BBox):
    
    def __init__(self, p1, p2):
        _BBox.__init__(self, p1, p2)

    def __repr__(self):
        return "Rectangle({}, {})".format(str(self.p1), str(self.p2))
    
    def _draw(self, canvas, options):
        p1 = self.p1
        p2 = self.p2
        x1,y1 = canvas.toScreen(p1.x,p1.y)
        x2,y2 = canvas.toScreen(p2.x,p2.y)
        return canvas.create_rectangle(x1,y1,x2,y2,options)
        
    def clone(self):
        other = Rectangle(self.p1, self.p2)
        other.config = self.config.copy()
        return other


class Oval(_BBox):
    
    def __init__(self, p1, p2):
        _BBox.__init__(self, p1, p2)

    def __repr__(self):
        return "Oval({}, {})".format(str(self.p1), str(self.p2))

        
    def clone(self):
        other = Oval(self.p1, self.p2)
        other.config = self.config.copy()
        return other
   
    def _draw(self, canvas, options):
        p1 = self.p1
        p2 = self.p2
        x1,y1 = canvas.toScreen(p1.x,p1.y)
        x2,y2 = canvas.toScreen(p2.x,p2.y)
        return canvas.create_oval(x1,y1,x2,y2,options)
    
class Circle(Oval):
    
    def __init__(self, center, radius):
        p1 = Point(center.x-radius, center.y-radius)
        p2 = Point(center.x+radius, center.y+radius)
        Oval.__init__(self, p1, p2)
        self.radius = radius

    def __repr__(self):
        return "Circle({}, {})".format(str(self.getCenter()), str(self.radius))
        
    def clone(self):
        other = Circle(self.getCenter(), self.radius)
        other.config = self.config.copy()
        return other
        
    def getRadius(self):
        return self.radius

                  
class Line(_BBox):
    
    def __init__(self, p1, p2):
        _BBox.__init__(self, p1, p2, ["arrow","fill","width"])
        self.setFill(DEFAULT_CONFIG['outline'])
        self.setOutline = self.setFill

    def __repr__(self):
        return "Line({}, {})".format(str(self.p1), str(self.p2))

    def clone(self):
        other = Line(self.p1, self.p2)
        other.config = self.config.copy()
        return other
  
    def _draw(self, canvas, options):
        p1 = self.p1
        p2 = self.p2
        x1,y1 = canvas.toScreen(p1.x,p1.y)
        x2,y2 = canvas.toScreen(p2.x,p2.y)
        return canvas.create_line(x1,y1,x2,y2,options)
        
    def setArrow(self, option):
        if not option in ["first","last","both","none"]:
            raise GraphicsError(BAD_OPTION)
        self._reconfig("arrow", option)
        

class Polygon(GraphicsObject):
    
    def __init__(self, *points):
        # if points passed as a list, extract it
        if len(points) == 1 and type(points[0]) == type([]):
            points = points[0]
        self.points = list(map(Point.clone, points))
        GraphicsObject.__init__(self, ["outline", "width", "fill"])

    def __repr__(self):
        return "Polygon"+str(tuple(p for p in self.points))
        
    def clone(self):
        other = Polygon(*self.points)
        other.config = self.config.copy()
        return other

    def getPoints(self):
        return list(map(Point.clone, self.points))

    def _move(self, dx, dy):
        for p in self.points:
            p.move(dx,dy)
   
    def _draw(self, canvas, options):
        args = [canvas]
        for p in self.points:
            x,y = canvas.toScreen(p.x,p.y)
            args.append(x)
            args.append(y)
        args.append(options)
        return GraphWin.create_polygon(*args) 

class Text(GraphicsObject):
    
    def __init__(self, p, text):
        GraphicsObject.__init__(self, ["justify","fill","text","font"])
        self.setText(text)
        self.anchor = p.clone()
        self.setFill(DEFAULT_CONFIG['outline'])
        self.setOutline = self.setFill

    def __repr__(self):
        return "Text({}, '{}')".format(self.anchor, self.getText())
    
    def _draw(self, canvas, options):
        p = self.anchor
        x,y = canvas.toScreen(p.x,p.y)
        return canvas.create_text(x,y,options)
        
    def _move(self, dx, dy):
        self.anchor.move(dx,dy)
        
    def clone(self):
        other = Text(self.anchor, self.config['text'])
        other.config = self.config.copy()
        return other

    def setText(self,text):
        self._reconfig("text", text)
        
    def getText(self):
        return self.config["text"]
            
    def getAnchor(self):
        return self.anchor.clone()

    def setFace(self, face):
        if face in ['helvetica','arial','courier','times roman']:
            f,s,b = self.config['font']
            self._reconfig("font",(face,s,b))
        else:
            raise GraphicsError(BAD_OPTION)

    def setSize(self, size):
        if 5 <= size <= 36:
            f,s,b = self.config['font']
            self._reconfig("font", (f,size,b))
        else:
            raise GraphicsError(BAD_OPTION)

    def setStyle(self, style):
        if style in ['bold','normal','italic', 'bold italic']:
            f,s,b = self.config['font']
            self._reconfig("font", (f,s,style))
        else:
            raise GraphicsError(BAD_OPTION)

    def setTextColor(self, color):
        self.setFill(color)


class Entry(GraphicsObject):

    def __init__(self, p, width):
        GraphicsObject.__init__(self, [])
        self.anchor = p.clone()
        #print self.anchor
        self.width = width
        self.text = tk.StringVar(_root)
        self.text.set("")
        self.fill = "gray"
        self.color = "black"
        self.font = DEFAULT_CONFIG['font']
        self.entry = None

    def __repr__(self):
        return "Entry({}, {})".format(self.anchor, self.width)

    def _draw(self, canvas, options):
        p = self.anchor
        x,y = canvas.toScreen(p.x,p.y)
        frm = tk.Frame(canvas.master)
        self.entry = tk.Entry(frm,
                              width=self.width,
                              textvariable=self.text,
                              bg = self.fill,
                              fg = self.color,
                              font=self.font)
        self.entry.pack()
        #self.setFill(self.fill)
        self.entry.focus_set()
        return canvas.create_window(x,y,window=frm)

    def getText(self):
        return self.text.get()

    def _move(self, dx, dy):
        self.anchor.move(dx,dy)

    def getAnchor(self):
        return self.anchor.clone()

    def clone(self):
        other = Entry(self.anchor, self.width)
        other.config = self.config.copy()
        other.text = tk.StringVar()
        other.text.set(self.text.get())
        other.fill = self.fill
        return other

    def setText(self, t):
        self.text.set(t)

            
    def setFill(self, color):
        self.fill = color
        if self.entry:
            self.entry.config(bg=color)

            
    def _setFontComponent(self, which, value):
        font = list(self.font)
        font[which] = value
        self.font = tuple(font)
        if self.entry:
            self.entry.config(font=self.font)


    def setFace(self, face):
        if face in ['helvetica','arial','courier','times roman']:
            self._setFontComponent(0, face)
        else:
            raise GraphicsError(BAD_OPTION)

    def setSize(self, size):
        if 5 <= size <= 36:
            self._setFontComponent(1,size)
        else:
            raise GraphicsError(BAD_OPTION)

    def setStyle(self, style):
        if style in ['bold','normal','italic', 'bold italic']:
            self._setFontComponent(2,style)
        else:
            raise GraphicsError(BAD_OPTION)

    def setTextColor(self, color):
        self.color=color
        if self.entry:
            self.entry.config(fg=color)


class Image(GraphicsObject):

    idCount = 0
    imageCache = {} # tk photoimages go here to avoid GC while drawn 
    
    def __init__(self, p, *pixmap):
        GraphicsObject.__init__(self, [])
        self.anchor = p.clone()
        self.imageId = Image.idCount
        Image.idCount = Image.idCount + 1
        if len(pixmap) == 1: # file name provided
            self.img = tk.PhotoImage(file=pixmap[0], master=_root)
        else: # width and height provided
            width, height = pixmap
            self.img = tk.PhotoImage(master=_root, width=width, height=height)

    def __repr__(self):
        return "Image({}, {}, {})".format(self.anchor, self.getWidth(), self.getHeight())
                
    def _draw(self, canvas, options):
        p = self.anchor
        x,y = canvas.toScreen(p.x,p.y)
        self.imageCache[self.imageId] = self.img # save a reference  
        return canvas.create_image(x,y,image=self.img)
    
    def _move(self, dx, dy):
        self.anchor.move(dx,dy)
        
    def undraw(self):
        try:
            del self.imageCache[self.imageId]  # allow gc of tk photoimage
        except KeyError:
            pass
        GraphicsObject.undraw(self)

    def getAnchor(self):
        return self.anchor.clone()
        
    def clone(self):
        other = Image(Point(0,0), 0, 0)
        other.img = self.img.copy()
        other.anchor = self.anchor.clone()
        other.config = self.config.copy()
        return other

    def getWidth(self):
        """Returns the width of the image in pixels"""
        return self.img.width() 

    def getHeight(self):
        """Returns the height of the image in pixels"""
        return self.img.height()

    def getPixel(self, x, y):
        """Returns a list [r,g,b] with the RGB color values for pixel (x,y)
        r,g,b are in range(256)

        """
        
        value = self.img.get(x,y) 
        if type(value) ==  type(0):
            return [value, value, value]
        elif type(value) == type((0,0,0)):
            return list(value)
        else:
            return list(map(int, value.split())) 

    def setPixel(self, x, y, color):
        """Sets pixel (x,y) to the given color
        
        """
        self.img.put("{" + color +"}", (x, y))
        

    def save(self, filename):
        """Saves the pixmap image to filename.
        The format for the save image is determined from the filname extension.

        """
        
        path, name = os.path.split(filename)
        ext = name.split(".")[-1]
        self.img.write( filename, format=ext)

        
def color_rgb(r,g,b):
    """r,g,b are intensities of red, green, and blue in range(256)
    Returns color specifier string for the resulting color"""
    return "#%02x%02x%02x" % (r,g,b)

def test():
    win = GraphWin()
    win.setCoords(0,0,10,10)
    t = Text(Point(5,5), "Centered Text")
    t.draw(win)
    p = Polygon(Point(1,1), Point(5,3), Point(2,7))
    p.draw(win)
    e = Entry(Point(5,6), 10)
    e.draw(win)
    win.getMouse()
    p.setFill("red")
    p.setOutline("blue")
    p.setWidth(2)
    s = ""
    for pt in p.getPoints():
        s = s + "(%0.1f,%0.1f) " % (pt.getX(), pt.getY())
    t.setText(e.getText())
    e.setFill("green")
    e.setText("Spam!")
    e.move(2,0)
    win.getMouse()
    p.move(2,3)
    s = ""
    for pt in p.getPoints():
        s = s + "(%0.1f,%0.1f) " % (pt.getX(), pt.getY())
    t.setText(s)
    win.getMouse()
    p.undraw()
    e.undraw()
    t.setStyle("bold")
    win.getMouse()
    t.setStyle("normal")
    win.getMouse()
    t.setStyle("italic")
    win.getMouse()
    t.setStyle("bold italic")
    win.getMouse()
    t.setSize(14)
    win.getMouse()
    t.setFace("arial")
    t.setSize(20)
    win.getMouse()
    win.close()

#MacOS fix 2
#tk.Toplevel(_root).destroy()

# MacOS fix 1
update()

if __name__ == "__main__":
    test()
```





#Tic Tac Toe
>Besides being a German female pop group, Tic Tac Toe is a game for 2 players. Each player can 
place one mark (or stone) per turn on the 3x3 grid The player who succeeds in placing three of 
their marks in a horizontal, vertical, or diagonal row wins the game. The marks used are usually 
'x' and 'o' for respective players.

>The final aim in this task is that one of the players will be the computer. You will implement 
an algorithm, that will help the computer to beat the human.

>First things first, let's start from the base. These are the basic things your program should be able to do:
* shortly describe game rules
* display the game board
* ask the player #1 to choose the position to take
* display the game board with the newly taken position
* ask the player #2 to choose the position to take
* display the game board with the newly taken position etc.

>The program should be able to assess and inform the user, whether either of the players won the 
ame or the players drew. (Don't forget to terminate the program).

>Once your game can perform the stuff above, try to do the bonus tasks.

**Example**
>Converting from decimal to binary:
```
[test@test ]$ ./ttt.py
Welcome to Tic Tac Toe, the game where ...
#somewhere here display the game board
What position will you take?
...
```
**Bonus**
* Include the computer as the second player (who will start the game? Will it be always the same player?)

* Implement minimax algorithm to help the computer to beat the human

* Try to create GUI with Pygame library

* Your game board can be bigger than 3x3. Does your algorithm still work?






#Open Data
>Open data sets: 
* Government open data - http://www.otevrenadata.cz/otevrena-data/zdroje-dat/
* Brno - https://datahub.io/cs_CZ/organization/statutarni-mesto-brno?page=3
* European data portal - http://data.europa.eu/euodp/en/data
* https://www.brno.cz/aktivni-obcan/
* http://www.otevrenadata.cz/
* https://datahub.io/cs_CZ/organization/statutarni-mesto-brno?page=3
* http://www.datablog.cz/zdroje-informaci
* https://www.reddit.com/r/datasets/
* http://www.datasets.co/
* NSFW- http://www.pornhub.com/webmasters


#Transparent Account Visualizer
>Your task is to get relevant data from transparent accounts and save them to database/csv file. 
Use visualization libraries afterwards to visualize the scraped data. Look for different anomalies, 
interesting conotations, find accounts with the most transfers.
* We recommend using bokeh visualization library:
    * http://bokeh.pydata.org/en/latest/
    * https://demo.bokehplots.com/apps/movies
    * http://bokeh.pydata.org/en/latest/docs/gallery/iris.html
* Bank & Sources/APIs:
    * https://www.fio.cz/bankovni-sluzby/bankovni-ucty/transparentni-ucet/vypis-transparentnich-uctu
    * https://www.csas.cz/cs/transparentni-ucty#/
    * https://www.kb.cz/cs/transparentni-ucty/
    
>There was already a group of people working on this project, you might find new correlations and 
work with data further.
* https://m.facebook.com/orwen/albums/10207255721526680/








#Semantic Diff
>Everyone knows the diff tool, right? The old-school utility taking two files on input and 
producing how the two files differ from each other. Together with another old-school utility, 
patch, it pretty much enabled distributed, collaborative software development.
But comparing source code as text should not be the end of it. Python code has rules and structure. 
It has entities like modules, classes and methods. It is possible to compare two versions 
of a Python project as programs, not as text, taking into account the semantics of the code. 
Which modules, classes or methods were changed, which were added, removed or moved around. 
What changed in the entities: were interfaces or contracts changed, or just implementation? 
Was is core of the program, or some weird, rarely used plugin?
The goal of this project is to produce a tool that understand Python code and is able to 
semantically compare two Python program versions (like a baseline and a pull request).

**How to start**
>Programs are trees (ASTs) and there are good tools that can read Python into ASTs for you already 
(astroid: https://pypi.python.org/pypi/astroid ). Simple semantic diff is probably a tree graph 
difference problem, for which there might 
be some nice solutions already in some graph library. Then it’s mostly a matter of determining what 
changes to look for, what to do with them and how to present them. Plus dealing with 
pseudo-differences like moving code around, renaming etc.

**Futher ideas**
>Program that describes a change in a natural language, just as a programmer would

>Program that extracts semantic properties of changes, for example to create a data set describing 
evolution of a software project that could be analysed for insights.

>A GitHub-integrated service producing useful information for PR reviewers

>Integration with pylint that would allow pylint to focus only on the code that was changed.

**Resources and inspiration:**
* https://www.semanticmerge.com/
* https://stackoverflow.com/questions/523307/semantic-diff-utilities





#Typespeed
>Typespeed is a game in which you'll test your typing skills on the keyboard. Your task is to 
create an environment where there will be moving words on the screen (from left to right or 
top down) and the task of the player is to type them as quickly as possible, before they hit 
specified barrier. The speed of the words will increase in time, so only better people will get 
further in the game.
* Video visualization of the game (older): https://www.youtube.com/watch?v=ENF_q-rRrcU&t=30s

**Bonus**
* Advanced game: ZTYPE (http://zty.pe/)
* Rankings
* Running as a web service








#Bullshit Generator
>The time is valuable to all of us and it is pain to dedicate yours to create approvals, motivation 
letters and justifications to various tasks (promotions, ...). That's why it is a good idea to 
automate these kind of tasks so you can focus on the work.

**Bonus**
* Advanced algorithms
* Running as web service
* Multiple language support








#Universal Testing Framework
>It’s your turn to dictate how things should be tested. Feeling somewhat powerful yet? Wait until 
after you design your very own appropriate (or inappropriate) pattern for testing someone else's code!

>Write a library of object-probing tools, which probe classes and functions (optionally change or 
replace them entirely if necessary) for people to test their code with. It runs the tests and 
prints beautiful verbose output as well.

>People should be able to use your library without having to consult you about it’s usage, so you 
should keep the code as readable and simple as possible.








#CV Parser
>CVs are mainly distributed in PDFs and we need raw information about them. It is not so easy to 
determine proper metadata from data extracted, since the sections of CVs usually differs, so your 
task is to create a general way how to parse CVs. We will provide database of anonymized CVs.

**Database of CVs**
* http://hack.engeto.com/CVs.zip

**Bonus**
* Advanced algorithms
* Running as webservice
* Multiple language support
