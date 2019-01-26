Requirements:
	1.Java
	2.Window builder 
	3.Lucene library 
	4.Apache OpenNLP jars
	5.en-parser-chunking.bin (an OpenNLP tool)

How to run code?

	- Please have the dataset files in a directory "inputfiles", tfWeights, clickStream and docScores files in the same directory as the code file.

	- If new document is to be indexed, uncomment the online query processing function (invertedIndex()) and please specify the filename in the process_files()

	- Once the inverted indices are created, we can comment the online query processing function and run only the offline method.

What are the files and what do they signify?

	Path to all the files: IR_SearchEngine\src\com\opennlp\demo

	- LuceneReadIndexFromFileExample.java - Reads the query and processes it

	- LuceneWriteIndexFromFileExample.java - Indexes all files which contains hashed code 

	- mainpage.java - Initial GUI loading file

	- ParserTest.java - Detects proper nouns in texts

	- project.java - GUI file for user to select whether he wants to query using the Soundex algorithm or without Soundex algorithm

	- search.java - GUI related file

	- Soundex.java - Performs case folding and soundex algorithm

	- soundex_gui.java - GUI to enter query which has to use Soundex algorithm

	- sr.java - Performs stop word removal

	- textDisplay.java - Displays retrieved file

	- without_soundex_gui.java - GUI to enter query which should not use Soundex algorithm