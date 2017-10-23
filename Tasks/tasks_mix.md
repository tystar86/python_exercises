#1
>Create a program that asks the user to enter their name and their age. Print out a message addressed to them that tells them the year that they will turn 100 years old.

**Bonus**

* Add on to the previous program by asking the user for another number and printing out that many copies of the previous message. (Hint: order of operations exists in Python)
Print out that many copies of the previous message on separate lines. (Hint: the string "\n is the same as pressing the ENTER button)


#2
>Ask the user for a number. Depending on whether the number is even or odd, print out an appropriate message to the user. Hint: how does an even / odd number react differently when divided by 2?

**Bonus**

* If the number is a multiple of 4, print out a different message.

* Ask the user for two numbers: one number to check (call it num) and one number to divide by (check). If check divides evenly into num, tell that to the user. If not, print a different appropriate message.


#3
>Write a program that takes a list of numbers (for example, a = [5, 10, 15, 20, 25]) and makes a new list of only the first and last elements of the given list. For practice, write this code inside a function.


#4
>Write a function that takes an ordered list of numbers (a list where the elements are in order from smallest to largest) and another number. The function decides whether or not the given number is inside the list and returns (then prints) an appropriate boolean.

**Bonus**

* Use binary search.


#5
>Take the code from some lorem ipsum website, and instead of printing the results to a screen, write the results to a txt file. In your code, just make up a name for the file you are saving to.

**Bonus**

* Ask the user to specify the name of the output file that will be saved.


#6
>Given a .txt file that has a list of a bunch of names, count how many of each name there are in the file, and print out the results to the screen.

**Bonus**

* Instead of using the .txt file from above (or instead of, if you want the challenge), take this .txt file, and count how many of each “category” of each image there are. This text file is actually a list of files corresponding to the SUN database scene recognition database, and lists the file directory hierarchy for the images. Once you take a look at the first line or two of the file, it will be clear which part represents the scene category.


#7
>Implement a function that takes as input three variables, and returns the largest of the three. Do this without using the Python max() function!

>The goal of this exercise is to think about some internals that Python normally takes care of for us. All you need is some variables and if statements!


#8 - Birthsday
>For this exercise, we will keep track of when our friend’s birthdays are, and be able to find that information based on their name. Create a dictionary (in your file) of names and birthdays. When you run your program it should ask the user to enter a name, and return the birthday of that person back to them. The interaction should look something like this:

**Example**
```
> Welcome to the birthday dictionary. We know the birthdays of:

Albert Einstein
Benjamin Franklin
Ada Lovelace

> Who's birthday do you want to look up?

Benjamin Franklin

> Benjamin Franklin's birthday is 01/17/1706.
```
>In the previous exercise we created a dictionary of famous scientists’ birthdays. In this exercise, modify your program from Part 1 to load the birthday dictionary from a JSON file on disk, rather than having the dictionary defined in the program.

**Bonus**
* Ask the user for another scientist’s name and birthday to add to the dictionary, and update the JSON file you have on disk with the scientist’s name. If you run the program multiple times and keep adding new names, your JSON file should keep getting bigger and bigger.
>In the previous exercise we saved information about famous scientists’ names and birthdays to disk. In this exercise, load that JSON file from disk, extract the months of all the birthdays, and count how many scientists have a birthday in each month.

>Your program should output something like:
```
{
	"May": 3,
	"November": 2,
	"December": 1
}
```

#9
>Take a list, say for example this one:
```
  a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```
>and write a program that prints out all the elements of the list that are less than 5.

**Bonus**

* Instead of printing the elements one by one, make a new list that has all the elements less than 5 from this list in it and print out this new list.
* Write this in one line of Python.
* Ask the user for a number and return a list that contains only elements from the original list a that are smaller than that number given by the user.

>In this exercise, use the bokeh Python library to plot a histogram of which months the scientists have birthdays in! Because it would take a long time for you to input the months of various scientists, you can use my scientist birthday JSON file. Just parse out the months (if you don’t know how, I suggest looking at the previous exercise or its solution) and draw your histogram.


#10
>Create a program that asks the user for a number and then prints out a list of all the divisors of that number. (If you don’t know what a divisor is, it is a number that divides evenly into another number. For example, 13 is a divisor of 26 because 26 / 13 has no remainder.)


#11
>Take two lists, say for example these two:
```
  a = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
  b = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]
```
>and write a program that returns a list that contains only the elements that are common between the lists (without duplicates). Make sure your program works on two lists of different sizes.

**Bonus**

* Randomly generate two lists to test this
* Write this in one line of Python (don’t worry if you can’t figure this out at this point - we’ll get to it soon)


#12
>Ask the user for a string and print out whether this string is a palindrome or not. (A palindrome is a string that reads the same forwards and backwards.)


#13
>Let’s say I give you a list saved in a variable: a = [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]. Write one line of Python that takes this list a and makes a new list that has only the even elements of this list in it.


#14
>Write a program that asks the user how many Fibonnaci numbers to generate and then generates them. Take this opportunity to think about how you can use functions. Make sure to ask the user to enter the number of numbers in the sequence to generate.(Hint: The Fibonnaci seqence is a sequence of numbers where the next number in the sequence is the sum of the previous two numbers in the sequence. The sequence looks like this: 1, 1, 2, 3, 5, 8, 13, …)


#15
>Write a program (function!) that takes a list and returns a new list that contains all the elements of the first list minus all the duplicates.

**Bonus**

* Write two different functions to do this - one using a loop and constructing a list, and another using sets.


#16
>Given two .txt files that have lists of numbers in them, find the numbers that are overlapping. One .txt file has a list of all prime numbers under 1000, and the other .txt file has a list of happy numbers up to 1000.

>(If you forgot, prime numbers are numbers that can’t be divided by any other number. And yes, happy numbers are a real thing in mathematics - you can look it up on Wikipedia. The explanation is easier with an example, which I will describe below.)
```
1, 7, 10, 13, 19, 23, 28, 31, 32, 44, 49, 68, 70, 79, 82, 86, 91, 94, 97, 100, 103, 109, 129, 130, 133, 139, 
167, 176, 188, 190, 192, 203, 208, 219, 226, 230, 236, 239, 262, 263, 280, 291, 293, 301, 302, 310, 313, 319,
320, 326, 329, 331, 338, 356, 362, 365, 367, 368, 376, 379, 383, 386, 391, 392, 397, 404, 409, 440, 446, 464,
469, 478, 487, 490, 496, 536, 556, 563, 565, 566, 608, 617, 622, 623, 632, 635, 637, 638, 644, 649, 653, 655,
656, 665, 671, 673, 680, 683, 694, 700, 709, 716, 736, 739, 748, 761, 763, 784, 790, 793, 802, 806, 818, 820,
833, 836, 847, 860, 863, 874, 881, 888, 899, 901, 904, 907, 910, 912, 913, 921, 923, 931, 932, 937, 940, 946,
964, 970, 973, 989, 998, 1000
```
```
2, 3, 5, 7, 11, 13, 17, 19, 23, 29 , 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103,
107, 109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211, 223,
227, 229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293, 307, 311, 313, 317, 331, 337, 347,
349, 353, 359, 367, 373, 379, 383, 389, 397, 401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 
467, 479, 487, 491, 499, 503, 509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607,
613, 617, 619, 631, 641, 643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743,
751, 757, 761, 769, 773, 787, 797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863, 877, 881, 883,
887, 907, 911, 919, 929, 937, 941, 947, 953, 967, 971, 977, 983, 991, 997
```


#17 - Hangman
>In this exercise, the task is to write a function that picks a random word from a list of words from the SOWPODS dictionary. Download this file and save it in the same directory as your Python code. This file is Peter Norvig’s compilation of the dictionary of words used in professional Scrabble tournaments. Each line in the file contains a single word.

* Aside: what is SOWPODS
    * SOWPODS is a word list commonly used in word puzzles and games (like Scrabble for example). It is the combination of the Scrabble Player’s Dictionary and the Chamber’s Dictionary. (The history of SOWPODS is quite interesting, I highly recommend reading the Wikipedia article if you are curious.)
>Let’s continue building Hangman. In the game of Hangman, a clue word is given by the program that the player has to guess, letter by letter. The player guesses one letter at a time until the entire word has been guessed. (In the actual game, the player can only guess 6 letters incorrectly before losing).

>Let’s say the word the player has to guess is “EVAPORATE”. For this exercise, write the logic that asks a player to guess a letter and displays letters in the clue word that were guessed correctly. For now, let the player guess an infinite number of times until they get the entire word. As a bonus, keep track of the letters the player guessed and display a different message if the player tries to guess that letter again. Remember to stop the game when all the letters have been guessed correctly! Don’t worry about choosing a word randomly or keeping track of the number of guesses the player has remaining - we will deal with those in a future exercise.

**Example**
```
>>> Welcome to Hangman!
_ _ _ _ _ _ _ _ _
>>> Guess your letter: S
Incorrect!
>>> Guess your letter: E
E _ _ _ _ _ _ _ E
...
And so on, until the player gets the word.
```
>In this exercise, we will finish building Hangman. In the game of Hangman, the player only has 6 incorrect guesses (head, body, 2 legs, and 2 arms) before they lose the game.

>In Part 1, we loaded a random word list and picked a word from it. In Part 2, we wrote the logic for guessing the letter and displaying that information to the user. In this exercise, we have to put it all together and add logic for handling guesses.

>Copy your code from Parts 1 and 2 into a new file as a starting point. Now add the following features:

>Only let the user guess 6 times, and tell the user how many guesses they have left.
Keep track of the letters the user guessed. If the user guesses a letter they already guessed, don’t penalize them - let them guess again.

**Bonus**
* When the player wins or loses, let them start a new game.
* Rather than telling the user "You have 4 incorrect guesses left", display some picture art for the Hangman. This is challenging - do the other parts of the exercise first!


#18 - Tic Tac Toe
>Time for some fake graphics! Let’s say we want to draw game boards that look like this:
```
 --- --- --- 
|   |   |   | 
 --- --- ---  
|   |   |   | 
 --- --- ---  
|   |   |   | 
 --- --- --- 
```
>This one is 3x3 (like in tic tac toe). Obviously, they come in many other sizes (8x8 for chess, 19x19 for Go, and many more).

>Ask the user what size game board they want to draw, and draw it for them to the screen using Python’s print statement.
>As you may have guessed, we are trying to build up to a full tic-tac-toe board. However, this is significantly more than half an hour of coding, so we’re doing it in pieces.

>Today, we will simply focus on checking whether someone has WON a game of Tic Tac Toe, not worrying about how the moves were made.

>If a game of Tic Tac Toe is represented as a list of lists, like so:
```
game = [[1, 2, 0],
	[2, 1, 0],
	[2, 1, 1]]
```
>where a 0 means an empty square, a 1 means that player 1 put their token in that space, and a 2 means that player 2 put their token in that space.

>Your task this week: given a 3 by 3 list of lists that represents a Tic Tac Toe game board, tell me whether anyone has won, and tell me which player won, if any. A Tic Tac Toe win is 3 in a row - either in a row, a column, or a diagonal. Don’t worry about the case where TWO people have won - assume that in every board there will only be one winner.

>Here are some more examples to work with:
```
winner_is_2 = [[2, 2, 0],
	[2, 1, 0],
	[2, 1, 1]]
```
```
winner_is_1 = [[1, 2, 0],
	[2, 1, 0],
	[2, 1, 1]]
```
```
winner_is_also_1 = [[0, 1, 0],
	[2, 1, 0],
	[2, 1, 1]]
```
```
no_winner = [[1, 2, 0],
	[2, 1, 0],
	[2, 1, 2]]
```
```
also_no_winner = [[1, 2, 0],
	[2, 1, 0],
	[2, 1, 0]]
```
>In a previous exercise we explored the idea of using a list of lists as a “data structure” to store information about a tic tac toe game. In a tic tac toe game, the “game server” needs to know where the Xs and Os are in the board, to know whether player 1 or player 2 (or whoever is X and O won).

>There has also been an exercise about drawing the actual tic tac toe gameboard using text characters.

>The next logical step is to deal with handling user input. When a player (say player 1, who is X) wants to place an X on the screen, they can’t just click on a terminal. So we are going to approximate this clicking simply by asking the user for a coordinate of where they want to place their piece.

>As a reminder, our tic tac toe game is really a list of lists. The game starts out with an empty game board like this:
```
game = [[0, 0, 0],
	[0, 0, 0],
	[0, 0, 0]]
```
>The computer asks Player 1 (X) what their move is (in the format row,col), and say they type 1,3. Then the game would print out
```
game = [[0, 0, X],
	[0, 0, 0],
	[0, 0, 0]]
```
>And ask Player 2 for their move, printing an O in that place.

* Things to note:

    * For this exercise, assume that player 1 (the first player to move) will always be X and player 2 (the second player) will always be O.
    * Notice how in the example I gave coordinates for where I want to move starting from (1, 1) instead of (0, 0). To people who don’t program, starting to count at 0 is a strange concept, so it is better for the user experience if the row counts and column counts start at 1. This is not required, but whichever way you choose to implement this, it should be explained to the player.
    * Ask the user to enter coordinates in the form “row,col” - a number, then a comma, then a number. Then you can use your Python skills to figure out which row and column they want their piece to be in.
    * Don’t worry about checking whether someone won the game, but if a player tries to put a piece in a game position where there already is another piece, do not allow the piece to go there.

**Bonus**
* For the “standard” exercise, don’t worry about “ending” the game - no need to keep track of how many squares are full. In a bonus version, keep track of how many squares are full and automatically stop asking for moves when there are no more valid moves.

>In 3 previous exercises, we built up a few components needed to build a Tic Tac Toe game in Python:

>Draw the Tic Tac Toe game board
>Checking whether a game board has a winner
>Handle a player move from user input
>The next step is to put all these three components together to make a two-player Tic Tac Toe game! Your challenge in this exercise is to use the functions from those previous exercises all together in the same program to make a two-player game that you can play with a friend. There are a lot of choices you will have to make when completing this exercise, so you can go as far or as little as you want with it.

**Here are a few things to keep in mind:**

* You should keep track of who won - if there is a winner, show a congratulatory message on the screen.
* If there are no more moves left, don’t ask for the next player’s move!
* As a bonus, you can ask the players if they want to play again and keep a running tally of who won more - Player 1 or Player 2.


#19
>Make a two-player Rock-Paper-Scissors game. (Hint: Ask for player plays (using input), compare them, print out a message of congratulations to the winner, and ask if the players want to start a new game)

* Remember the rules:

    * Rock beats scissors
    * Scissors beats paper
    * Paper beats rock


#20
>Generate a random number between 1 and 9 (including 1 and 9). Ask the user to guess the number, then tell them whether they guessed too low, too high, or exactly right.

**Bonus**

* Keep the game going until the user types “exit”
* Keep track of how many guesses the user has taken, and when the game ends, print this out.


#21
>Ask the user for a number and determine whether the number is prime or not. (For those who have forgotten, a prime number is a number that has no divisors.). You can (and should!) use your answer to Exercise 4 to help you. Take this opportunity to practice using functions, described below.


#22
>Write a program (using functions!) that asks the user for a long string containing multiple words. Print back to the user the same string, except with the words in backwards order. 

>For example, say I type the string:
```
  My name is Michele
```  
>Then I would see the string:
```
  Michele is name My
```
>shown back to me.


#23
>Create a program that will play the “cows and bulls” game with the user. The game works like this:

>Randomly generate a 4-digit number. Ask the user to guess a 4-digit number. For every digit that the user guessed correctly in the correct place, they have a “cow”. For every digit the user guessed correctly in the wrong place is a “bull.” Every time the user makes a guess, tell them how many “cows” and “bulls” they have. Once the user guesses the correct number, the game is over. Keep track of the number of guesses the user makes throughout teh game and tell the user at the end.

>Say the number generated by the computer is 1038. An example interaction could look like this:
```
  Welcome to the Cows and Bulls Game! 
  Enter a number: 
  >>> 1234
  2 cows, 0 bulls
  >>> 1256
  1 cow, 1 bull
  ...
```
>Until the user guesses the number.


#24
>This time, we’re going to do exactly the opposite. You, the user, will have in your head a number between 0 and 100. The program will guess a number, and you, the user, will say whether it is too high, too low, or your number.

>At the end of this exchange, your program should print out how many guesses it took to get your number.

>As the writer of this program, you will have to choose how your program will strategically guess. A naive strategy can be to simply start the guessing at 1, and keep going (2, 3, 4, etc.) until you hit the number. But that’s not an optimal guessing strategy. An alternate strategy might be to guess 50 (right in the middle of the range), and then increase / decrease by 1 as needed. After you’ve written the program, try to find the optimal strategy! (We’ll talk about what is the optimal one next week with the solution.)


#25
>Write a password generator in Python. Be creative with how you generate passwords - strong passwords have a mix of lowercase letters, uppercase letters, numbers, and symbols. The passwords should be random, generating a new password every time the user asks for a new password. Include your run-time code in a main method.

**Bonus**

* Ask the user how strong they want their password to be. For weak passwords, pick a word or two from a list.


#26
>Use the BeautifulSoup and requests Python packages to print out a list of all the article titles on the New York Times homepage. (https://www.nytimes.com/)
* http://www.practicepython.org/exercise/2014/06/06/17-decode-a-web-page.html


#27
>Using the requests and BeautifulSoup Python libraries, print to the screen the full text of the article on this website: http://www.vanityfair.com/society/2014/06/monica-lewinsky-humiliation-culture.

>The article is long, so it is split up between 4 pages. Your task is to print out the text to the screen so that you can read the full article without having to click any buttons.

* (Hint: The post here describes in detail how to use the BeautifulSoup and requests libraries through the solution of the exercise posted here.)

>This will just print the full text of the article to the screen. It will not make it easy to read, so next exercise we will learn how to write this text to a .txt file.
* http://www.practicepython.org/exercise/2014/07/14/19-decode-a-web-page-two.html


#28
>Write a function that will take a list of words as input and will return back
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

#29
>Write a function that will accept a filenames input return
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

#30
>Write a function that will collect all the even numbers and odd numbers
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

#31
>Write a function, that will accept two tuples of 2 numbers
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

#32
>Write a function that will return a list of numbers divisible by given number
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

#33
>Write a function that will count how many vowels and consonants are in
a given string.

>The function should take as input a string and output a dictionary in form:
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


#34
>Write a function that will create "echo sentences". Each word in
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


#35
>Create a function that will print out how many times does every object occur inside
any list, tuple or string (counts of individual characters).
The function output should be a dictionary with counts associated with each value.

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


#36
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


#37
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

#38
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


#39
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


#40
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

#41
>Dragon curve is a fractal that is naturally created when folding a paper for example. Create a program that will draw 
so called dragon curve of any size. Example of dragon curve after 12 iterations: Dragon curve gets twice longer each 
iteration. We can color the line, that is created during single iteration: You can also try to create combined dragon 
curves, which lines will have different coloures.


#42
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


#43
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

#44
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

#45
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


#46
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

#47
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


#48
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


#49
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


#50
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


#51
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


#52
>The time is valuable to all of us and it is pain to dedicate yours to create approvals, motivation 
letters and justifications to various tasks (promotions, ...). That's why it is a good idea to 
automate these kind of tasks so you can focus on the work.

**Bonus**
* Advanced algorithms
* Running as web service
* Multiple language support


#53
>It’s your turn to dictate how things should be tested. Feeling somewhat powerful yet? Wait until 
after you design your very own appropriate (or inappropriate) pattern for testing someone else's code!

>Write a library of object-probing tools, which probe classes and functions (optionally change or 
replace them entirely if necessary) for people to test their code with. It runs the tests and 
prints beautiful verbose output as well.

>People should be able to use your library without having to consult you about it’s usage, so you 
should keep the code as readable and simple as possible.


#54
>CVs are mainly distributed in PDFs and we need raw information about them. It is not so easy to 
determine proper metadata from data extracted, since the sections of CVs usually differs, so your 
task is to create a general way how to parse CVs. We will provide database of anonymized CVs.

**Database of CVs**
* http://hack.engeto.com/CVs.zip

**Bonus**
* Advanced algorithms
* Running as webservice
* Multiple language support


#55 
>Write a Python program to print the following string in a specific format (see the output).
Sample String : "Twinkle, twinkle, little star, How I wonder what you are! Up above the world so high, Like a diamond in the sky. Twinkle, twinkle, little star, How I wonder what you are" 

**Output:**
```
Twinkle, twinkle, little star,
	How I wonder what you are! 
		Up above the world so high,   		
		Like a diamond in the sky. 
Twinkle, twinkle, little star, 
	How I wonder what you are
```
#56 
>Write a Python program to get the Python version you are using.

#57
>Write a Python program to display the current date and time.

**Example**
```
Current date and time : 
2014-07-05 14:34:14
```

#58
>Write a Python program which accepts the radius of a circle from the user and compute the area.

**Example**
```
r = 1.1
Area = 3.8013271108436504
```
#59
>Write a Python program which accepts the user's first and last name and print them in reverse order with a space between them.

#60
>Write a Python program which accepts a sequence of comma-separated numbers from user and generate a list and a tuple with those numbers.

**Sample data :** ```3, 5, 7, 23```

**Output :**
```
List : ['3', ' 5', ' 7', ' 23'] 
Tuple : ('3', ' 5', ' 7', ' 23')
```

#61
>Write a Python program to accept a filename from the user and print the extension of that.

**Sample filename :** ```abc.java ```

**Output :** ```java```

#62
>Write a Python program to display the first and last colors from the following list.
```
color_list = ["Red","Green","White" ,"Black"]
```

#63 
>Write a Python program to display the examination schedule. (extract the date from exam_st_date).
```
exam_st_date = (11, 12, 2014)

Sample Output : The examination will start from : 11 / 12 / 2014
```

#64
>Write a Python program that accepts an integer (n) and computes the value of n+nn+nnn.
```
Sample value of n is 5 

Expected Result : 615
```

#65
>Write a Python program to print the documents (syntax, description etc.) of Python built-in function(s). 
```
Sample function : abs()

Expected Result : 

abs(number) -> number

Return the absolute value of the argument.
```

#66
>Write a Python program to print the calendar of a given month and year.
```
Note : Use 'calendar' module. 
```

#67
>Write a Python program to print the following here document.

**Sample string :**
```
a string that you "don't" have to escape

This

is a ....... multi-line

heredoc string --------> example
```

#68
>Write a Python program to calculate number of days between two dates.

**Sample dates :** ```(2014, 7, 2), (2014, 7, 11)```

**Expected output :** ```9 days```

#69
>Write a Python program to get the volume of a sphere with radius 6.

#70
>Write a Python program to get the difference between a given number and 17, if the number is greater than 17 return double the absolute difference.

#71
>Write a Python program to test whether a number is within 100 of 1000 or 2000.

#72
>Write a Python program to calculate the sum of three given numbers, if the values are equal then return thrice of their sum.

#73
>Write a Python program to get a new string from a given string where "Is" has been added to the front. If the given string already begins with "Is" then return the string unchanged.

#74
>Write a Python program to get a string which is n (non-negative integer) copies of a given string.

#75
>Write a Python program to find whether a given number (accept from the user) is even or odd, print out an appropriate message to the user.

#76
>Write a Python program to count the number 4 in a given list.

#77
>Write a Python program to get the n (non-negative integer) copies of the first 2 characters of a given string. Return the n copies of the whole string if the length is less than 2.

#78
>Write a Python program to test whether a passed letter is a vowel or not.

#79
>Write a Python program to check whether a specified value is contained in a group of values.

**Test Data :**
```
3 -> [1, 5, 8, 3] : True
-1 -> [1, 5, 8, 3] : False
```

#80
>Write a Python program to create a histogram from a given list of integers.

#81
>Write a Python program to concatenate all elements in a list into a string and return it.

#82
>Write a Python program to print all even numbers from a given numbers list in the same order and stop the printing if any numbers that come after 237 in the sequence.

**Sample numbers list :**
```
numbers = [    
    386, 462, 47, 418, 907, 344, 236, 375, 823, 566, 597, 978, 328, 615, 953, 345, 
    399, 162, 758, 219, 918, 237, 412, 566, 826, 248, 866, 950, 626, 949, 687, 217, 
    815, 67, 104, 58, 512, 24, 892, 894, 767, 553, 81, 379, 843, 831, 445, 742, 717, 
    958,743, 527
    ]
```

#83
>Write a Python program to print out a set containing all the colors from color_list_1 which are not present in color_list_2.

**Test Data :**
```
color_list_1 = set(["White", "Black", "Red"]) 
color_list_2 = set(["Red", "Green"])
```
**Expected Output :**
```
{'Black', 'White'}
```

#84
>Write a Python program that will accept the base and height of a triangle and compute the area.

#85
>Write a Python program to compute the greatest common divisor (GCD) of two positive integers.

#86
>Write a Python program to get the least common multiple (LCM) of two positive integers.

#87
>Write a Python program to sum of three given integers. However, if two values are equal sum will be zero.

#88
>Write a Python program to sum of two given integers. However, if the sum is between 15 to 20 it will return 20.

#89
>Write a Python program that will return true if the two given integer values are equal or their sum or difference is 5.

#90
>Write a Python program to add two objects if both objects are an integer type.

#91
>Write a Python program to display your details like name, age, address in three different lines.

#92
>Write a Python program to solve (x + y) * (x + y).

**Test Data :** ```x = 4, y = 3```

**Expected Output :** ```(4 + 3) ^ 2) = 49```

#93
>Write a Python program to compute the future value of a specified principal amount, rate of interest, and a number of years.

**Test Data :** ```amt = 10000, int = 3.5, years = 7```

**Expected Output :** ```12722.79```

#94
>Write a Python program to compute the distance between the points (x1, y1) and (x2, y2).

#95
>Write a Python program to check whether a file exists.

#96
>Write a Python program to determine if a Python shell is executing in 32bit or 64bit mode on OS.

#97
>Write a Python program to get OS name, platform and release information.

#98
>Write a Python program to locate Python site-packages.

#99
>Write a python program to call an external command in Python.

#100
>Write a python program to get the path and name of the file that is currently executing.

#101
>Write a Python program to find out the number of CPUs using.

#102
>Write a Python program to parse a string to Float or Integer.

#103
>Write a Python program to list all files in a directory in Python.

#104
>Write a Python program to print without newline or space.

#105
>Write a Python program to determine profiling of Python programs.

**Note :** A profile is a set of statistics that describes how often and for how long various parts of the program executed. These statistics can be formatted into reports via the pstats module. 

#106
>Write a Python program to print to stderr.

#107
>Write a python program to access environment variables.

#108
>Write a Python program to get the current username.

#109
>Write a Python to find local IP addresses using Python's stdlib.

#110
>Write a Python program to get height and width of the console window.

#111
>Write a program to get execution time for a Python method.

#112
>Write a python program to sum of the first n positive integers.

#113
>Write a Python program to convert height (in feet and inches) to centimeters.

#114
>Write a Python program to calculate the hypotenuse of a right angled triangle.

#115
>Write a Python program to convert the distance (in feet) to inches, yards, and miles.

#116
>Write a Python program to convert all units of time into seconds.

#117
>Write a Python program to get an absolute file path.

#118 
>Write a Python program to get file creation and modification date/times.

#119
>Write a Python program to convert seconds to day, hour, minutes and seconds.

#120
>Write a Python program to calculate body mass index.

#121
>Write a Python program to calculate the sum of the digits in an integer.

#122
>Write a Python program to sort three integers without using conditional statements and loops.

#123
>Write a Python program to sort files by date.

#124
>Write a Python program to get a directory listing, sorted by creation date.

#125
>Write a Python program to get the details of math module.

#126
>Write a Python program to calculate midpoints of a line.

#127
>Write a Python program to hash a word.

#128
>Write a Python program to get the copyright information.

#129
>Write a Python program to get the command-line arguments (name of the script, the number of arguments, arguments) passed to a script.

#130
>Write a Python program to test whether the system is a big-endian platform or little-endian platform.

#131
>Write a Python program to find the available built-in modules.

#132
>Write a Python program to get the size of an object in bytes.

#133
>Write a Python program to get the current value of the recursion limit.

#134
>Write a Python program to concatenate N strings.

#135
>Write a Python program to calculate the sum over a container.

#136
>Write a Python program to test if a certain number is greater than all numbers of a list.

#137
>Write a Python program to count the number occurrence of a specific character in a string.

#138 
>Write a Python program to check if a file path is a file or a directory.

#139
>Write a Python program to get the ASCII value of a character.

#140
>Write a Python program to get the size of a file.

#141 
>Given variables x=30 and y=20, write a Python program to print t "30+20=50".

#142
>Write a Python program to perform an action if a condition is true.
Given a variable name, if the value is 1, display the string "First day of a Month!" and do nothing if the value is not equal.

#143
>Write a Python program to create a copy of its own source code.

#144
>Write a Python program to swap two variables.

#145
>Write a Python program to define a string containing special characters in various forms.

#146
>Write a Python program to get the identity of an object.

#147
>Write a Python program to convert a byte string to a list of integers.

#148
>Write a Python program to check if a string is numeric.

#149
>Write a Python program to print the current call stack.

#150
>Write a Python program to list the special variables used within the language.

#151
>Write a Python program to get the system time.

**Note :** The system time is important for debugging, network information, random number seeds, or something as simple as program performance.

#152
>Write a Python program to clear the screen or terminal.

#153
>Write a Python program to get the name of the host on which the routine is running.

#154
>Write a Python program to access and print a URL's content to the console.

#155
>Write a Python program to get system command output.

#156
>Write a Python program to extract the filename from a given path.

#157
>Write a Python program to get the effective group id, effective user id, real group id, a list of supplemental group ids associated with the current process.

**Note :** Availability: Unix.

#158
>Write a Python program to get the users environment.

#159
>Write a Python program to divide a path on the extension separator.

#160
>Write a Python program to retrieve file properties. 

#161
>Write a Python program to find path refers to a file or directory when you encounter a path name.

#162
>Write a Python program to check if a number is positive, negative or zero. 

#163
>Write a Python program to get numbers divisible by fifteen from a list using an anonymous function.

#164
>Write a Python program to make file lists from current directory using a wildcard. 

#165
>Write a Python program to remove the first item from a specified list.

#166
>Write a Python program to input a number, if it is not a number generate an error message.

#167
>Write a Python program to filter the positive numbers from a list. 

#168
>Write a Python program to compute the product of a list of integers (without using for loop).

#169
>Write a Python program to print Unicode characters.

#170
>Write a Python program to prove that two string variables of same value point same memory location.

#171
>Write a Python program to create a bytearray from a list.

#172
>Write a Python program to display a floating number in specified numbers.

#173
>Write a Python program to format a specified string to limit the number of characters to 6.

#174
>Write a Python program to determine if variable is defined or not.

#175
>Write a Python program to empty a variable without destroying it.

**Sample data :**
```
n=20
d = {"x":200}
```
**Expected Output :**
```
0
{}
```

#176
>Write a Python program to determine the largest and smallest integers, longs, floats.

#177
>Write a Python program to check if multiple variables have the same value.

#178
>Write a Python program to sum of all counts in a collections?

#179
>Write a Python program to get the actual module object for a given object.

#180
>Write a Python program to check if an integer fits in 64 bits.

#181
>Write a Python program to check if lowercase letters exist in a string.

#182
>Write a Python program to add leading zeroes to a string.

#183
>Write a Python program to use double quotes to display strings.

#184
>Write a Python program to split a variable length string into variables.

#185
>Write a Python program to list home directory without absolute path.

#186
>Write a Python program to calculate the time runs (difference between start and current time) of a program.

#187
>Write a Python program to input two integers in a single line.

#188
>Write a Python program to print a variable without spaces between values.

**Sample value :** ```x =30```

**Expected output :** ```Value of x is "30"``` 

#189
>Write a Python program to find files and skip directories of a given directory.

#190
>Write a Python program to extract single key-value pair of a dictionary in variables.

#191
>Write a Python program to convert true to 1 and false to 0.

#192
>Write a Python program to valid a IP address.

#193
>Write a Python program to convert an integer to binary keep leading zeros.

**Sample data :** ```50```

**Expected output :** ```00001100, 0000001100```

#194
>Write a python program to convert decimal to hexadecimal.

**Sample decimal number :** ```30, 4```

**Expected output :** ```1e, 04``` 

#195
>Write a Python program to find the operating system name, platform and platform release date.
```
Operating system name:

posix 

Platform name: 

Linux 

Platform release:

4.4.0-47-generic 
```

#196
>Write a Python program to determine if the python shell is executing in 32bit or 64bit mode on operating system.

#197
>Write a Python program to check if variable is of integer or string.

#198
>Write a Python program to find the operating system name, platform and platform release date.
```
Operating system name:

posix 

Platform name: 

Linux 

Platform release:

4.4.0-47-generic 
```

#199
>Write a Python program to find the location of Python module sources.
```
Operating system name:

posix 

Platform name: 

Linux 

Platform release:

4.4.0-47-generic 
```

#200
>Write a program which can compute the factorial of a given numbers.
The results should be printed in a comma-separated sequence on a single line.
```
Suppose the following input is supplied to the program:
8
Then, the output should be:
40320
```

#201
>With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary.

>Suppose the following input is supplied to the program:

```8```

>Then, the output should be:

```{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}```

#202
>Write a program which accepts a sequence of comma-separated numbers from console and generate a list and a tuple which contains every number.

>Suppose the following input is supplied to the program:

```34,67,55,33,12,98```

>Then, the output should be:

```
['34', '67', '55', '33', '12', '98']
('34', '67', '55', '33', '12', '98')
```

#203
>Define a class which has at least two methods:
* getString: to get a string from console input
* printString: to print the string in upper case.

>Also please include simple test function to test the class methods.

#204
>Write a program that calculates and prints the value according to the given formula:
`
```Q = Square root of [(2 * C * D)/H]```

>Following are the fixed values of C and H:

```C is 50. H is 30.```

```D is the variable whose values should be input to your program in a comma-separated sequence.```

**Example**

>Let us assume the following comma separated input sequence is given to the program:

```100,150,180```

>The output of the program should be:

```18,22,24```

#205
>Write a program which takes 2 digits, X,Y as input and generates a 2-dimensional array. The element value in the i-th row and j-th column of the array should be i*j.
Note: i=0,1.., X-1; j=0,1,¡­Y-1.

**Example**

>Suppose the following inputs are given to the program:

```3,5```

>Then, the output of the program should be:

```[[0, 0, 0, 0, 0], [0, 1, 2, 3, 4], [0, 2, 4, 6, 8]]```

#206
>Write a program that accepts a comma separated sequence of words as input and prints the words in a comma-separated sequence after sorting them alphabetically.

>Suppose the following input is supplied to the program:

```without,hello,bag,world```

>Then, the output should be:

```bag,hello,without,world```

#207
>Write a program that accepts sequence of lines as input and prints the lines after making all characters in the sentence capitalized.

>Suppose the following input is supplied to the program:
```
Hello world
Practice makes perfect
```
>Then, the output should be:

```
HELLO WORLD
PRACTICE MAKES PERFECT
```

#208
>Write a program that accepts a sequence of whitespace separated words as input and prints the words after removing all duplicate words and sorting them alphanumerically.

>Suppose the following input is supplied to the program:

```hello world and practice makes perfect and hello world again```

>Then, the output should be:

```again and hello makes perfect practice world```

#209
>Write a program which accepts a sequence of comma separated 4 digit binary numbers as its input and then check whether they are divisible by 5 or not. The numbers that are divisible by 5 are to be printed in a comma separated sequence.

>Example:

```0100,0011,1010,1001```

>Then the output should be:

```1010```

**Notes :** Assume the data is input by console.

#210
>Write a program, which will find all such numbers between 1000 and 3000 (both included) such that each digit of the number is an even number.

>The numbers obtained should be printed in a comma-separated sequence on a single line.

#211
>Write a program that accepts a sentence and calculate the number of letters and digits.

>Suppose the following input is supplied to the program:

```hello world! 123```

>Then, the output should be:
```
LETTERS 10
DIGITS 3
```

#212
>Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters.

>Suppose the following input is supplied to the program:

```Hello world!```

>Then, the output should be:
```
UPPER CASE 1
LOWER CASE 9
```
#213
>Write a program that computes the value of a+aa+aaa+aaaa with a given digit as the value of a.

>Suppose the following input is supplied to the program:

```9```

>Then, the output should be:

```11106```

#214
>Use a list comprehension to square each odd number in a list. The list is input by a sequence of comma-separated numbers.

>Suppose the following input is supplied to the program:

```1,2,3,4,5,6,7,8,9```

>Then, the output should be:

```1,3,5,7,9```

#215
>Write a program that computes the net amount of a bank account based a transaction log from console input. The transaction log format is shown as following:
```
D 100
W 200
```
>D means deposit while W means withdrawal.

>Suppose the following input is supplied to the program:
```
D 300
D 300
W 200
D 100
```
>Then, the output should be:
```500```

#216
>A website requires the users to input username and password to register. Write a program to check the validity of password input by users.

>Following are the criteria for checking the password:
* 1. At least 1 letter between [a-z]
* 2. At least 1 number between [0-9]
* 3. At least 1 letter between [A-Z]
* 4. At least 1 character from [$#@]
* 5. Minimum length of transaction password: 6
* 6. Maximum length of transaction password: 12

>Your program should accept a sequence of comma separated passwords and will check them according to the above criteria. Passwords that match the criteria are to be printed, each separated by a comma.

**Example**

>If the following passwords are given as input to the program:
```
ABd1234@1,a F1#,2w3E*,2We3345
```
>Then, the output of the program should be:

```ABd1234@1```

#217
>You are required to write a program to sort the (name, age, height) tuples by ascending order where name is string, age and height are numbers. The tuples are input by console. The sort criteria is:
* 1: Sort based on name;
* 2: Then sort based on age;
* 3: Then sort by score.
>The priority is that name > age > score.

>If the following tuples are given as input to the program:
```
Tom,19,80
John,20,90
Jony,17,91
Jony,17,93
Json,21,85
```
>Then, the output of the program should be:

```[('John', '20', '90'), ('Jony', '17', '91'), ('Jony', '17', '93'), ('Json', '21', '85'), ('Tom', '19', '80')]```

#218
>Define a class with a generator which can iterate the numbers, which are divisible by 7, between a given range 0 and n.

#219
>A robot moves in a plane starting from the original point (0,0). The robot can move toward UP, DOWN, LEFT and RIGHT with a given steps. The trace of robot movement is shown as the following:
```
UP 5
DOWN 3
LEFT 3
RIGHT 2
¡­
```
>The numbers after the direction are steps. Please write a program to compute the distance from current position after a sequence of movement and original point. If the distance is a float, then just print the nearest integer.
```
Example:
If the following tuples are given as input to the program:
UP 5
DOWN 3
LEFT 3
RIGHT 2
Then, the output of the program should be:
2
```

#220
>Write a program to compute the frequency of the words from the input. The output should output after sorting the key alphanumerically. 

* Suppose the following input is supplied to the program:

 ```New to Python or choosing between Python 2 and Python 3? Read Python 2 or Python 3.```
* Then, the output should be:
```
2:2
3.:1
3?:1
New:1
Python:5
Read:1
and:1
between:1
choosing:1
or:2
to:1
```

#221
>Write a method which can calculate square value of number

#222
>Python has many built-in functions, and if you do not know how to use it, you can read document online or find some books. But Python has a built-in document function for every built-in functions.
    Please write a program to print some Python built-in functions documents, such as abs(), int(), raw_input()
    And add document for your own function
    
#223
>Define a class, which have a class parameter and have a same instance parameter.

#224
>Define a function which can compute the sum of two numbers.

#225
>Define a function that can convert a integer into a string and print it in console.

#226
>Define a function that can receive two integral numbers in string form and compute their sum and then print it in console.

#227
>Define a function that can accept two strings as input and concatenate them and then print it in console.

#228
>Define a function that can accept two strings as input and print the string with maximum length in console. If two strings have the same length, then the function should print al l strings line by line.

#229
>Define a function that can accept an integer number as input and print the "It is an even number" if the number is even, otherwise print "It is an odd number".

#230
>Write a program to generate and print another tuple whose values are even numbers in the given tuple ```(1,2,3,4,5,6,7,8,9,10)```. 

#231
>Write a program which accepts a string as input to print "Yes" if the string is "yes" or "YES" or "Yes", otherwise print "No". 

#232
>Define a function which can generate a dictionary where the keys are numbers between 1 and 20 (both included) and the values are square of keys. The function should just print the values only.

#233
>Write a program which can filter even numbers in a list by using filter function. The list is: ```[1,2,3,4,5,6,7,8,9,10]```.

#234
>With a given tuple ```(1,2,3,4,5,6,7,8,9,10)```, write a program to print the first half values in one line and the last half values in one line. 

#235
>Define a function which can generate a list where the values are square of numbers between 1 and 20 (both included). Then the function needs to print the first 5 elements in the list.

#236
>Write a program which can map() to make a list whose elements are square of elements in ```[1,2,3,4,5,6,7,8,9,10]```.

#237
>Write a program which can map() and filter() to make a list whose elements are square of even number in ```[1,2,3,4,5,6,7,8,9,10]```.

#238
>Write a program which can filter() to make a list whose elements are even number between 1 and 20 (both included).

#239
>Write a program which can map() to make a list whose elements are square of numbers between 1 and 20 (both included).

#240
>Define a class named American which has a static method called printNationality.

#241
>Define a class named American and its subclass NewYorker. 

#242
>Define a class named Circle which can be constructed by a radius. The Circle class has a method which can compute the area. 

#243
>Define a class named Rectangle which can be constructed by a length and width. The Rectangle class has a method which can compute the area. 

#244
>Define a class named Shape and its subclass Square. The Square class has an init function which takes a length as argument. Both classes have a area function which can print the area of the shape where Shape's area is 0 by default.

#245
>Please raise a RuntimeError exception.

#246
>Write a function to compute 5/0 and use try/except to catch the exceptions.

#247
>Define a custom exception class which takes a string message as attribute.

#248
>Assuming that we have some email addresses in the "username@companyname.com" format, please write program to print the user name of a given email address. Both user names and company names are composed of letters only.

#249
>Write a program which accepts a sequence of words separated by whitespace as input to print the words composed of digits only.

#250
>Print a unicode string "hello world".

#251
>Write a program to read an ASCII string and to convert it to a unicode string encoded by utf-8.

#252
>Write a special comment to indicate a Python source code file is in unicode.

#253
>Write a program to compute 1/2+2/3+3/4+...+n/n+1 with a given n input by console (n>0).

#254
>Write a program to compute:
```
f(n)=f(n-1)+100 when n>0
and f(0)=1
```
>with a given n input by console (n>0).

#255
>The Fibonacci Sequence is computed based on the following formula:
```
f(n)=0 if n=0
f(n)=1 if n=1
f(n)=f(n-1)+f(n-2) if n>1
```

>Please write a program to compute the value of f(n) with a given n input by console.

#256
>Please write a program using generator to print the even numbers between 0 and n in comma separated form while n is input by console.

#257
>Please write a program using generator to print the numbers which can be divisible by 5 and 7 between 0 and n in comma separated form while n is input by console.

#258
>Please write assert statements to verify that every number in the list ```[2,4,6,8]``` is even.

#259
>Please write a binary search function which searches an item in a sorted list. The function should return the index of element to be searched in the list.

#260
>Please generate a random float where the value is between 10 and 100 using Python math module.

#261
>Please generate a random float where the value is between 5 and 95 using Python math module.

#262
>Please write a program to output a random even number between 0 and 10 inclusive using random module and list comprehension.

#263
>Please write a program to output a random number, which is divisible by 5 and 7, between 0 and 10 inclusive using random module and list comprehension.

#264
>Please write a program to generate a list with 5 random numbers between 100 and 200 inclusive.

#265
>Please write a program to compress and decompress the string "hello world!hello world!hello world!hello world!".

#266
>Please write a program to print the running time of execution of "1+1" for 100 times.

#267
>Please write a program to shuffle and print the list ```[3,6,7,8]```.

#268
>Please write a program to generate all sentences where subject is in ```["I", "You"]``` and verb is in ```["Play", "Love"]``` and the object is in ```["Hockey","Football"]```.

#269
>Please write a program to print the list after removing delete even numbers in ```[5,6,77,45,22,12,24]```.

#270
>By using list comprehension, please write a program to print the list after removing delete numbers which are divisible by 5 and 7 in ```[12,24,35,70,88,120,155]```.

#271
>By using list comprehension, please write a program to print the list after removing the 0th, 2nd, 4th,6th numbers in ```[12,24,35,70,88,120,155]```.

#272
>By using list comprehension, please write a program generate a 3*5*8 3D array whose each element is 0.

#273
>By using list comprehension, please write a program to print the list after removing the 0th,4th,5th numbers in ```[12,24,35,70,88,120,155]```.

#274
>By using list comprehension, please write a program to print the list after removing the value 24 in ```[12,24,35,24,88,120,155]```.

#275
>With two given lists ```[1,3,6,78,35,55]``` and ```[12,24,35,24,88,120,155]```, write a program to make a list whose elements are intersection of the above given lists.

#276
>With a given list ```[12,24,35,24,88,120,155,88,120,155]```, write a program to print this list after removing all duplicate values with original order reserved.

#277
>Define a class Person and its two child classes: Male and Female. All classes have a method "getGender" which can print "Male" for Male class and "Female" for Female class.

#278
>Please write a program which count and print the numbers of each character in a string input by console.

#279
>Please write a program which accepts a string from console and print it in reverse order.

#280
>Please write a program which accepts a string from console and print the characters that have even indexes.

#281
>Please write a program which prints all permutations of ```[1,2,3]```

#282
>Write a program to solve a classic ancient Chinese puzzle: 
We count 35 heads and 94 legs among the chickens and rabbits in a farm. How many rabbits and how many chickens do we have?

#283
>We have two monkeys, a and b, and the parameters a_smile and b_smile indicate if each is smiling. We are in trouble if they are both smiling or if neither of them is smiling. Return True if we are in trouble.
```
monkey_trouble(True, True) → True
monkey_trouble(False, False) → True
monkey_trouble(True, False) → False
```
#284
>Given two int values, return their sum. Unless the two values are the same, then return double their sum.
```
sum_double(1, 2) → 3
sum_double(3, 2) → 5
sum_double(2, 2) → 8
```

#285
>The parameter weekday is True if it is a weekday, and the parameter vacation is True if we are on vacation. We sleep in if it is not a weekday or we're on vacation. Return True if we sleep in.
```
sleep_in(False, False) → True
sleep_in(True, False) → False
sleep_in(False, True) → True
```

#286
>Given an int n, return the absolute difference between n and 21, except return double the absolute difference if n is over 21.
```
diff21(19) → 2
diff21(10) → 11
diff21(21) → 0
```

#287
>We have a loud talking parrot. The "hour" parameter is the current hour time in the range 0..23. We are in trouble if the parrot is talking and the hour is before 7 or after 20. Return True if we are in trouble.
```
parrot_trouble(True, 6) → True
parrot_trouble(True, 7) → False
parrot_trouble(False, 6) → False
```

#288
>Given 2 ints, a and b, return True if one if them is 10 or if their sum is 10.
```
makes10(9, 10) → True
makes10(9, 9) → False
makes10(1, 9) → True
```

#289
>Given a string, return a new string where "not " has been added to the front. However, if the string already begins with "not", return the string unchanged.
```
not_string('candy') → 'not candy'
not_string('x') → 'not x'
not_string('not bad') → 'not bad'
```

#290
>Given a string, we'll say that the front is the first 3 chars of the string. If the string length is less than 3, the front is whatever is there. Return a new string which is 3 copies of the front.
```
front3('Java') → 'JavJavJav'
front3('Chocolate') → 'ChoChoCho'
front3('abc') → 'abcabcabc'
```

#291
>Given 2 int values, return True if one is negative and one is positive. Except if the parameter "negative" is True, then return True only if both are negative.
```
pos_neg(1, -1, False) → True
pos_neg(-1, 1, False) → True
pos_neg(-4, -5, True) → True
```

#292
>Given a string, return a new string where the first and last chars have been exchanged.
```
front_back('code') → 'eodc'
front_back('a') → 'a'
front_back('ab') → 'ba'
```

#293
>Given a non-empty string and an int n, return a new string where the char at index n has been removed. The value of n will be a valid index of a char in the original string (i.e. n will be in the range 0..len(str)-1 inclusive).
```
missing_char('kitten', 1) → 'ktten'
missing_char('kitten', 0) → 'itten'
missing_char('kitten', 4) → 'kittn'
```

#294
>Given an int n, return True if it is within 10 of 100 or 200. Note: abs(num) computes the absolute value of a number.
```
near_hundred(93) → True
near_hundred(90) → True
near_hundred(89) → False
```

#295
>Given a string and a non-negative int n, return a larger string that is n copies of the original string.
```
string_times('Hi', 2) → 'HiHi'
string_times('Hi', 3) → 'HiHiHi'
string_times('Hi', 1) → 'Hi'
```

#296
>Given a string and a non-negative int n, we'll say that the front of the string is the first 3 chars, or whatever is there if the string is less than length 3. Return n copies of the front;
```
front_times('Chocolate', 2) → 'ChoCho'
front_times('Chocolate', 3) → 'ChoChoCho'
front_times('Abc', 3) → 'AbcAbcAbc'
```

#297
>Given a string, return a new string made of every other char starting with the first, so "Hello" yields "Hlo".
```
string_bits('Hello') → 'Hlo'
string_bits('Hi') → 'H'
string_bits('Heeololeo') → 'Hello'
```

#298
>Given a non-empty string like "Code" return a string like "CCoCodCode".
```
string_splosion('Code') → 'CCoCodCode'
string_splosion('abc') → 'aababc'
string_splosion('ab') → 'aab'
```

#299
>Given a string, return the count of the number of times that a substring length 2 appears in the string and also as the last 2 chars of the string, so "hixxxhi" yields 1 (we won't count the end substring).
```
last2('hixxhi') → 1
last2('xaxxaxaxx') → 1
last2('axxxaaxx') → 2
```

#300
>Given an array of ints, return the number of 9's in the array.
```
array_count9([1, 2, 9]) → 1
array_count9([1, 9, 9]) → 2
array_count9([1, 9, 9, 3, 9]) → 3
```

#301
>Given an array of ints, return True if one of the first 4 elements in the array is a 9. The array length may be less than 4.
```
array_front9([1, 2, 9, 3, 4]) → True
array_front9([1, 2, 3, 4, 9]) → False
array_front9([1, 2, 3, 4, 5]) → False
```

#302
>Given an array of ints, return True if the sequence of numbers 1, 2, 3 appears in the array somewhere.
```
array123([1, 1, 2, 3, 1]) → True
array123([1, 1, 2, 4, 1]) → False
array123([1, 1, 2, 1, 2, 3]) → True
```

#303
>Given 2 strings, a and b, return the number of the positions where they contain the same length 2 substring. So "xxcaazz" and "xxbaaz" yields 3, since the "xx", "aa", and "az" substrings appear in the same place in both strings.
```
string_match('xxcaazz', 'xxbaaz') → 3
string_match('abc', 'abc') → 2
string_match('abc', 'axc') → 0
```

#304
>Given a string name, e.g. "Bob", return a greeting of the form "Hello Bob!".
```
hello_name('Bob') → 'Hello Bob!'
hello_name('Alice') → 'Hello Alice!'
hello_name('X') → 'Hello X!'
```

#305
>Given two strings, a and b, return the result of putting them together in the order abba, e.g. "Hi" and "Bye" returns "HiByeByeHi".
```
make_abba('Hi', 'Bye') → 'HiByeByeHi'
make_abba('Yo', 'Alice') → 'YoAliceAliceYo'
make_abba('What', 'Up') → 'WhatUpUpWhat'
```

#306
>The web is built with HTML strings like "<i>Yay</i>" which draws Yay as italic text. In this example, the "i" tag makes <i> and </i> which surround the word "Yay". Given tag and word strings, create the HTML string with tags around the word, e.g. "<i>Yay</i>".
```
make_tags('i', 'Yay') → '<i>Yay</i>'
make_tags('i', 'Hello') → '<i>Hello</i>'
make_tags('cite', 'Yay') → '<cite>Yay</cite>'
```

#307
>Given an "out" string length 4, such as "<<>>", and a word, return a new string where the word is in the middle of the out string, e.g. "<<word>>".
```
make_out_word('<<>>', 'Yay') → '<<Yay>>'
make_out_word('<<>>', 'WooHoo') → '<<WooHoo>>'
make_out_word('[[]]', 'word') → '[[word]]'
```

#308
>Given a string, return a new string made of 3 copies of the last 2 chars of the original string. The string length will be at least 2.
```
extra_end('Hello') → 'lololo'
extra_end('ab') → 'ababab'
extra_end('Hi') → 'HiHiHi'
```

#309
>Given a string, return the string made of its first two chars, so the String "Hello" yields "He". If the string is shorter than length 2, return whatever there is, so "X" yields "X", and the empty string "" yields the empty string "".
```
first_two('Hello') → 'He'
first_two('abcdefg') → 'ab'
first_two('ab') → 'ab'
```

#310
>Given a string of even length, return the first half. So the string "WooHoo" yields "Woo".
```
first_half('WooHoo') → 'Woo'
first_half('HelloThere') → 'Hello'
first_half('abcdef') → 'abc'
```

#311
>Given a string, return a version without the first and last char, so "Hello" yields "ell". The string length will be at least 2.
```
without_end('Hello') → 'ell'
without_end('java') → 'av'
without_end('coding') → 'odin'
```

#312
>Given 2 strings, a and b, return a string of the form short+long+short, with the shorter string on the outside and the longer string on the inside. The strings will not be the same length, but they may be empty (length 0).
```
combo_string('Hello', 'hi') → 'hiHellohi'
combo_string('hi', 'Hello') → 'hiHellohi'
combo_string('aaa', 'b') → 'baaab'
```

#313
>Given 2 strings, return their concatenation, except omit the first char of each. The strings will be at least length 1.
```
non_start('Hello', 'There') → 'ellohere'
non_start('java', 'code') → 'avaode'
non_start('shotl', 'java') → 'hotlava'
```

#314
>Given a string, return a "rotated left 2" version where the first 2 chars are moved to the end. The string length will be at least 2.
```
left2('Hello') → 'lloHe'
left2('java') → 'vaja'
left2('Hi') → 'Hi'
```

#315
>Given an array of ints, return True if 6 appears as either the first or last element in the array. The array will be length 1 or more.
```
first_last6([1, 2, 6]) → True
first_last6([6, 1, 2, 3]) → True
first_last6([13, 6, 1, 2, 3]) → False
```

#316
>Given an array of ints, return True if the array is length 1 or more, and the first element and the last element are equal.
```
same_first_last([1, 2, 3]) → False
same_first_last([1, 2, 3, 1]) → True
same_first_last([1, 2, 1]) → True
```

#317
>Return an int array length 3 containing the first 3 digits of pi, {3, 1, 4}.
```
make_pi() → [3, 1, 4]
```

#318
>Given 2 arrays of ints, a and b, return True if they have the same first element or they have the same last element. Both arrays will be length 1 or more.
```
common_end([1, 2, 3], [7, 3]) → True
common_end([1, 2, 3], [7, 3, 2]) → False
common_end([1, 2, 3], [1, 3]) → True
```

#319
>Given an array of ints length 3, return the sum of all the elements.
```
sum3([1, 2, 3]) → 6
sum3([5, 11, 2]) → 18
sum3([7, 0, 0]) → 7
```

#320
>Given an array of ints length 3, return an array with the elements "rotated left" so {1, 2, 3} yields {2, 3, 1}.
```
rotate_left3([1, 2, 3]) → [2, 3, 1]
rotate_left3([5, 11, 9]) → [11, 9, 5]
rotate_left3([7, 0, 0]) → [0, 0, 7]
```

#321
>Given an array of ints length 3, return a new array with the elements in reverse order, so {1, 2, 3} becomes {3, 2, 1}.
```
reverse3([1, 2, 3]) → [3, 2, 1]
reverse3([5, 11, 9]) → [9, 11, 5]
reverse3([7, 0, 0]) → [0, 0, 7]
```

#323
>Given an array of ints length 3, figure out which is larger, the first or last element in the array, and set all the other elements to be that value. Return the changed array.
```
max_end3([1, 2, 3]) → [3, 3, 3]
max_end3([11, 5, 9]) → [11, 11, 11]
max_end3([2, 11, 3]) → [3, 3, 3]
```

#324
>Given an array of ints, return the sum of the first 2 elements in the array. If the array length is less than 2, just sum up the elements that exist, returning 0 if the array is length 0.
```
sum2([1, 2, 3]) → 3
sum2([1, 1]) → 2
sum2([1, 1, 1, 1]) → 2
```

#325
>Given 2 int arrays, a and b, each length 3, return a new array length 2 containing their middle elements.
```
middle_way([1, 2, 3], [4, 5, 6]) → [2, 5]
middle_way([7, 7, 7], [3, 8, 0]) → [7, 8]
middle_way([5, 2, 9], [1, 4, 5]) → [2, 4]
```

#326
>Given an array of ints, return a new array length 2 containing the first and last elements from the original array. The original array will be length 1 or more.
```
make_ends([1, 2, 3]) → [1, 3]
make_ends([1, 2, 3, 4]) → [1, 4]
make_ends([7, 4, 6, 2]) → [7, 2]
```

#327
>Given an int array length 2, return True if it contains a 2 or a 3.
```
has23([2, 5]) → True
has23([4, 3]) → True
has23([4, 5]) → False
```

#328
>When squirrels get together for a party, they like to have cigars. A squirrel party is successful when the number of cigars is between 40 and 60, inclusive. Unless it is the weekend, in which case there is no upper bound on the number of cigars. Return True if the party with the given values is successful, or False otherwise.
```
cigar_party(30, False) → False
cigar_party(50, False) → True
cigar_party(70, True) → True
```

#329
>You and your date are trying to get a table at a restaurant. The parameter "you" is the stylishness of your clothes, in the range 0..10, and "date" is the stylishness of your date's clothes. The result getting the table is encoded as an int value with 0=no, 1=maybe, 2=yes. If either of you is very stylish, 8 or more, then the result is 2 (yes). With the exception that if either of you has style of 2 or less, then the result is 0 (no). Otherwise the result is 1 (maybe).
```
date_fashion(5, 10) → 2
date_fashion(5, 2) → 0
date_fashion(5, 5) → 1
```

#330
>The squirrels in Palo Alto spend most of the day playing. In particular, they play if the temperature is between 60 and 90 (inclusive). Unless it is summer, then the upper limit is 100 instead of 90. Given an int temperature and a boolean is_summer, return True if the squirrels play and False otherwise.
```
squirrel_play(70, False) → True
squirrel_play(95, False) → False
squirrel_play(95, True) → True
```

#331
>Given a day of the week encoded as 0=Sun, 1=Mon, 2=Tue, ...6=Sat, and a boolean indicating if we are on vacation, return a string of the form "7:00" indicating when the alarm clock should ring. Weekdays, the alarm should be "7:00" and on the weekend it should be "10:00". Unless we are on vacation -- then on weekdays it should be "10:00" and weekends it should be "off".
```
alarm_clock(1, False) → '7:00'
alarm_clock(5, False) → '7:00'
alarm_clock(0, False) → '10:00'
```

#332
>Given 2 ints, a and b, return their sum. However, sums in the range 10..19 inclusive, are forbidden, so in that case just return 20.
```
sorta_sum(3, 4) → 7
sorta_sum(9, 4) → 20
sorta_sum(10, 11) → 21
```

#333
>You are driving a little too fast, and a police officer stops you. Write code to compute the result, encoded as an int value: 0=no ticket, 1=small ticket, 2=big ticket. If speed is 60 or less, the result is 0. If speed is between 61 and 80 inclusive, the result is 1. If speed is 81 or more, the result is 2. Unless it is your birthday -- on that day, your speed can be 5 higher in all cases.
```
caught_speeding(60, False) → 0
caught_speeding(65, False) → 1
caught_speeding(65, True) → 0
```

#334
>The number 6 is a truly great number. Given two int values, a and b, return True if either one is 6. Or if their sum or difference is 6. Note: the function abs(num) computes the absolute value of a number.
```
love6(6, 4) → True
love6(4, 5) → False
love6(1, 5) → True
```

#335
>Given a non-negative number "num", return True if num is within 2 of a multiple of 10. Note: (a % b) is the remainder of dividing a by b, so (7 % 5) is 2.
```
near_ten(12) → True
near_ten(17) → False
near_ten(19) → True
```

#336
>We want to make a row of bricks that is goal inches long. We have a number of small bricks (1 inch each) and big bricks (5 inches each). Return True if it is possible to make the goal by choosing from the given bricks. This is a little harder than it looks and can be done without any loops.
```
make_bricks(3, 1, 8) → True
make_bricks(3, 1, 9) → False
make_bricks(3, 2, 10) → True
```

#337
>Given 3 int values, a b c, return their sum. However, if one of the values is the same as another of the values, it does not count towards the sum.
```
lone_sum(1, 2, 3) → 6
lone_sum(3, 2, 3) → 2
lone_sum(3, 3, 3) → 0
```

#338
>Given 3 int values, a b c, return their sum. However, if one of the values is 13 then it does not count towards the sum and values to its right do not count. So for example, if b is 13, then both b and c do not count.
```
lucky_sum(1, 2, 3) → 6
lucky_sum(1, 2, 13) → 3
lucky_sum(1, 13, 3) → 1
```

#339
>Given three ints, a b c, return True if one of b or c is "close" (differing from a by at most 1), while the other is "far", differing from both other values by 2 or more. Note: abs(num) computes the absolute value of a number.
```
close_far(1, 2, 10) → True
close_far(1, 2, 3) → False
close_far(4, 1, 3) → True
```

#340
>For this problem, we'll round an int value up to the next multiple of 10 if its rightmost digit is 5 or more, so 15 rounds up to 20. Alternately, round down to the previous multiple of 10 if its rightmost digit is less than 5, so 12 rounds down to 10. Given 3 ints, a b c, return the sum of their rounded values. To avoid code repetition, write a separate helper "def round10(num):" and call it 3 times. Write the helper entirely below and at the same indent level as round_sum().
```
round_sum(16, 17, 18) → 60
round_sum(12, 13, 14) → 30
round_sum(6, 4, 4) → 10
```

#341
>Given 3 int values, a b c, return their sum. However, if any of the values is a teen -- in the range 13..19 inclusive -- then that value counts as 0, except 15 and 16 do not count as a teens. Write a separate helper "def fix_teen(n):"that takes in an int value and returns that value fixed for the teen rule. In this way, you avoid repeating the teen code 3 times (i.e. "decomposition"). Define the helper below and at the same indent level as the main no_teen_sum().
```
no_teen_sum(1, 2, 3) → 6
no_teen_sum(2, 13, 1) → 3
no_teen_sum(2, 1, 14) → 3
```

#342
>We want make a package of goal kilos of chocolate. We have small bars (1 kilo each) and big bars (5 kilos each). Return the number of small bars to use, assuming we always use big bars before small bars. Return -1 if it can't be done.
```
make_chocolate(4, 1, 9) → 4
make_chocolate(4, 1, 10) → -1
make_chocolate(4, 1, 7) → 2
```

#343
>Given a string, return a string where for every char in the original, there are two chars.
```
double_char('The') → 'TThhee'
double_char('AAbb') → 'AAAAbbbb'
double_char('Hi-There') → 'HHii--TThheerree'
```

#344
>Return the number of times that the string "hi" appears anywhere in the given string.
```
count_hi('abc hi ho') → 1
count_hi('ABChi hi') → 2
count_hi('hihi') → 2
```

#345
>Return True if the string "cat" and "dog" appear the same number of times in the given string.
```
cat_dog('catdog') → True
cat_dog('catcat') → False
cat_dog('1cat1cadodog') → True
```

#346
>Return True if the given string contains an appearance of "xyz" where the xyz is not directly preceeded by a period (.). So "xxyz" counts but "x.xyz" does not.
```
xyz_there('abcxyz') → True
xyz_there('abc.xyz') → False
xyz_there('xyz.abc') → True
```

#347
>Given two strings, return True if either of the strings appears at the very end of the other string, ignoring upper/lower case differences (in other words, the computation should not be "case sensitive"). Note: s.lower() returns the lowercase version of a string.
```
end_other('Hiabc', 'abc') → True
end_other('AbC', 'HiaBc') → True
end_other('abc', 'abXabc') → True
```

#348
>Return the number of times that the string "code" appears anywhere in the given string, except we'll accept any letter for the 'd', so "cope" and "cooe" count.
```
count_code('aaacodebbb') → 1
count_code('codexxcode') → 2
count_code('cozexxcope') → 2
```

#349
>Return the number of even ints in the given array. Note: the % "mod" operator computes the remainder, e.g. 5 % 2 is 1.
```
count_evens([2, 1, 2, 3, 4]) → 3
count_evens([2, 2, 0]) → 3
count_evens([1, 3, 5]) → 0
```

#350
>Given an array length 1 or more of ints, return the difference between the largest and smallest values in the array. Note: the built-in min(v1, v2) and max(v1, v2) functions return the smaller or larger of two values.
```
big_diff([10, 3, 5, 6]) → 7
big_diff([7, 2, 10, 9]) → 8
big_diff([2, 10, 7, 2]) → 8
```

#351
>Return the "centered" average of an array of ints, which we'll say is the mean average of the values, except ignoring the largest and smallest values in the array. If there are multiple copies of the smallest value, ignore just one copy, and likewise for the largest value. Use int division to produce the final average. You may assume that the array is length 3 or more.
```
centered_average([1, 2, 3, 4, 100]) → 3
centered_average([1, 1, 5, 5, 10, 8, 7]) → 5
centered_average([-10, -4, -2, -4, -2, 0]) → -3
```

#352
>Given an array of ints, return True if the array contains a 2 next to a 2 somewhere.
```
has22([1, 2, 2]) → True
has22([1, 2, 1, 2]) → False
has22([2, 1, 2]) → False
```

#353
>Return the sum of the numbers in the array, except ignore sections of numbers starting with a 6 and extending to the next 7 (every 6 will be followed by at least one 7). Return 0 for no numbers.
```
sum67([1, 2, 2]) → 5
sum67([1, 2, 2, 6, 99, 99, 7]) → 5
sum67([1, 1, 6, 7, 2]) → 4
```

#354
>Return the sum of the numbers in the array, returning 0 for an empty array. Except the number 13 is very unlucky, so it does not count and numbers that come immediately after a 13 also do not count.
```
sum13([1, 2, 2, 1]) → 6
sum13([1, 1]) → 2
sum13([1, 2, 2, 1, 13]) → 6
```

#355
#356
#357
#358
#359
#360
#361
#362
#363
#364
#365
#366
#367
#368
#369
#370
#371
#372
#373
#374
#375
#376
#378
#379
#380
#381
#382
#383
#384
#385
#386
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
#

