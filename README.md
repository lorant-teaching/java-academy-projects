# ENGETO Java Academy projects

## Create program to solve "Create 24 using numbers 8,8,3,3" puzzle

__Puzzle:__ Find a mathematical expression using numbers 8,8,3,3 (all of them exactly once) and basic operations (addition, subtraction, multiplication, division) which evaluates to 24. Grouping with parentheses is allowed. 

__Assignment:__ Create a Java program for solving the above puzzle.

__Bonus tasks:__   
Find all the solutions to the puzzle with rules:
1. Allowed are unary operators square root and factorials
2. In addition to 1):
	- logarithm is allowed where the base is one of the numbers used (e.g. log3(8) uses up one 3 and one 8)
	- cube root is allowed (on real numbers), where the expression 3√8 uses up one 3 and one 8

__Implementation details:__ Create a data model and methods for evaluating mathematical expressions using the basic operations (addition, subtraction, multiplication, division) and groupings with parentheses. Package this model as a separate java library (.jar). Create a java program which finds a solution for the puzzle using your library. You can use brute force, but any creative optimizations are welcome. For the bonus task you may want to extend the original library with unary functions. 

__Notes:__ API of the library should be clean and concise (and javadoc documented!), so it can be possibly useful for the developer community (as projects will be open-source)

## Conway's Game of life

Implement an application which can compute the state of Conway's game of life at given generation. The input will be a text file with a defined pattern for the initial state of the game and the number of the requested generation to be computed, the output a similar file with the state at the requested generation. The game should be able to handle finite and infite fields.

__Bonus tasks:__  
1. Compute a sequence of generations defined by the user and use a library to save them as image files - for a slideshow of evolution   
2. Add support for a Moebius strip field
3. Create a simple GUI for the application

__Resources:__ https://en.wikipedia.org/wiki/Conway%27s__Game__of__Life


## (Re)Create your favorite board/card game

Create your favorite board game as an application! Focus on abstraction, specifically state and interactions. The base should be a library, which contains objects representing the state of the game and interfaces providing methods to manipulate the state (play the game). Use test driven development to faciliate the design of a concise interface. On top of this, create a CLI (command-line interface) to play the game by human players. No graphics or AI players required.

__Inspiration:__   
https://jonthysell.com/2016/07/13/creating-an-ai-to-play-hive-with-mzinga-part-i/  
https://en.wikipedia.org/wiki/Algebraic__notation__(chess)

## Text processor

Create a text processor, which allows the user to (functions ordered from basic to advanced):
- search for given words
- search for given sequence of words
- search for parts of the text of length N where the occurence of the given word is highest
- create a moving window function for the occurence of a given word in the text (parameters: word, window size)
- create a moving window function for the occurence of more given words in the text (parameters: words, window size)

The input text should be a simple .txt file, the output should be the position of the searched expression in the file (row, column). The program doesn't have to be able to handle texts too long, since you're not required to persist the indexes required for the tasks outside of the JVM's memory.

__Bonus tasks:__  
- Build the indexes in a persistence layer (DB)
- Use a library to plot the functions on the screen

## Invoice processing from image

Create an application that scrapes the important data from images of invoices (may be handwritten). Use a public OCR (optical character recognition) API or library.  

__Input:__ images of invoices  
__Expected output:__ structured text files containing the important information from the invoices (sender and reciever name, address, ICO, billed items and cash amount, etc.)

## Java wrapper for popular web API

Create a Java library which wraps a around popular web API (youtube, facebook, github, etc.) and provides a Java interface for the API. 

__Resources__:  
https://developers.facebook.com/docs/graph-api/overview/  
https://developers.google.com/youtube/v3   
https://developers.google.com/api-client-library/java/apis/youtube/v3


---

__Notes:__
- Final submission of the projects requires to have Unit tests, a Maven project, javadoc documentation, and configured continuous integration with Travis CI/Jenkins 
- For my recommendation for job hunters, I need two of these projects or projects from https://engeto.com/cs/kurz/java-qe/lekce done with good quality. Initial submission can be of lesser quality and we can fine tune your programs to meet quality standards.
