Efficient Proof Reader
===
Efficient Proof Reader is a compare and merge tool which employs an efficient method to proof reader a file if a similar file is available for compare. In many real world situations we come across such scenarios. Many document archiving strategies requires digitization of the documents. In such cases, ensuring the accuracy of the data, just relying on the manual keyed in text may not be ideal. At the same time, the reliability of the digitally retrieved data may not be good enough. One can easily compare these two files to find out where exactly have issues in the file. 
There are many tools available for such comparisons. However, they still require someone to go through the entire file, often correcting the same mistakes in different part of the file. The Efficient Proof Reader provides a better alternate.

Algorithm
		Read both files 
		Align them 
		Compare each aligned blocks
			If they are similar
				Go to next block
			Else
				For each set of mismatches
					If the set is not already found in the list
						create a new tuple
						add this tuple to the mismatches list
		For each tuple in mismatches list
			display the words
			Automatically select the one that has more number occurance as the correct word
			Ask user to select the correct word
			Mark the correct word
			
		Open the file to fix the spelling errors
			For each tuple in mismatches list
				Load a concordance of the incorrect word in the file
					(optionally) allow the user to select the entries to be included in the current F/R operation
				Find the incorrect word and replace with correct word
