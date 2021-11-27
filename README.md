# search_engine
This project search the word ,sentence /string or Quotations 

Salient features of the projects
1. It is basically a search engine which search the 
 a word , string/Sentence or a quotations in all text files and pdf files
 which are present in a given directory


2. for pdf files first it convert the pdf files into text then search in them.

3. algorithm is using is inverted indexing, making raking and then searching
the word in O(1) time.
preprocessing time is O(n)

4. In texts folder contain all txt files and in PDFs folder contain pdf files

5. command need to execute for search your query
  command 1:   $python search.py
     it give following options to you
1)to create index and search in folder
2)to search in folder
3)to convert pdf to text
4)search in file by kmp
5)recently modified or created files
6)exit program

enter your option like 1, 2 ,3 ,4,5,6


enter one for execute the option 1
first execute the option 1

it make the index and rank the files accordingly
it take a liitle time to make indexing and giving ranking to all the files present in Texts sirectory

now you can chose option on your choice

for Quoray:
for search word simple give input your word example <algorithm>
for Search the Sentence input <your Sentence>
for quotations input <"your quotation">

Output:-
It gives
1 File name and line number containg your query ;
 
Salient Features:

    Multiple Word Searching
    Stemming of Words (Eg:- Spelling -> spell; heroes -> hero). This feature helps us to ignore the form of verbs.
    Exact Searching:- If the query is contained in quotes then the results will contain exactly those results otherwise it may be in some other order. ( Eg:- searching for good boy will show both good boy as well as boy good, but when exact search is selected “good boy” only results of good boy will be shown.
    Indexing of Words:- Words present in stopword.dat files are not indexed as they are commonly used words and doesn't need indexing. Stemming of words is done before indexing them. Also, all words are indexed in lower case so that it is easy to search regardless of case of letters.
    Saving of Indexes:- Once you have indexed a file we save the indexes of it so that we don’t have to wait again for indexing it.
    Ranking is done by TF-IDF algorithm.
    Searches for txt files only.

Data Structures:

The data structures used in the project are Dictionary, Lists and Sets.

    Main Index Dictionary = { Word : { Book : { Page/Line : [occurrences] } } }
    Individual File Dictionary (The one that is saved) = { Word : { Page/Line : [occurrences] } }
    Answer = { Book : [Page/Line Numbers] }

Future Improvements:

This is currently an ongoing project and I am planning to improve it further by adding some features like:

    Did You Mean:- If a particular word is not found then we apply did you mean to get results (This will be done using Peter Norvig's Did You Mean Implementation)
    GUI:- I am planning to make a GTK+ User Interface for this (GTK+ Documentation)
    Recent Searches:- Add option to store the Recent searches in a file
    Opening Files:- On click of a particular result the file opens from that particular Page Number or Line Number of File where the occurrence is present.


I am using Kmp to those files which you add next few files so that not waste time to
make indexing all files after adding few files
If you adding a number of files then you can make indexing executing the command 1

     



 
