Program Overview:
The provided Python program solves the problem of identifying the longest and second longest compound words from a list of words. 
A compound word is a word that can be constructed by concatenating copies of shorter words found in the same list. 
The program reads input words from two files, processes them using a trie data structure, and outputs the longest and second longest compound words,
along with the total number of compound words.


How to Execute the Code:
1.	Prerequisites:
•	Python installed on your system. You can download Python from python.org.
2.	Clone the Repository:
•	Clone this repository to your local machine using Git:
3.	Navigate to the Directory:
•	Open a terminal or command prompt and navigate to the directory where you cloned the repository:
4.	Prepare Input Files:
•	Ensure you have the input files Input_01.txt and Input_02.txt with words list (one word per line, no spaces, all lower case)
        in the same directory as the Python script.
6.	Execute the Program:

 
Design Decisions and Approach:

•	Trie Data Structure:
	The program uses a trie (prefix tree) data structure to efficiently store and search words.
        This allows for quick identification of prefixes and suffixes of words, essential for finding compound words.

 
•	Pair Class:
	A Pair class is used to store word pairs (original word and its suffix) in the queue during processing.
        This helps in maintaining the context of the words being processed.

 
•	Reading Input Files:
	The program reads words from two input files (Input_01.txt and Input_02.txt).
        The read_words_from_file function reads words from a file and returns them as a list.

 
•	Queue-based Processing:
	Words and their suffixes are processed using a queue. Words with possible suffixes are added to the queue, and the program iteratively
        processes these pairs until no further combinations are possible.

 
 •      Output Format:
	The program outputs the longest and second longest compound words, along with the total number of compound words found.
        The output is displayed in the console.
