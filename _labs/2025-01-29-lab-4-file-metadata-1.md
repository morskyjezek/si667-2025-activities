---
layout:   post
title:    "Lab 4: File Metadata 1"
date:     2025-01-29
assigned: 2025-01-30
due:      2025-02-04
key:      lab-4-key
canvas-link: https://umich.instructure.com/courses/733396/assignments/2649541
categories: lab
---

This lab asks you to explore concepts and tools related to file identification and characterization, which we have discussed over the last couple of weeks. The files you should use for the assignment are from the course file collection you downloaded previously.

# Lab 4: Using the Shell for File Identification and Characterization

## Problem 1: Embedded Metadata {#problem-1}

**Embedded Metadata.** This exercise is similar to the one demonstrated in class, which looked at the contents of a powerpoint file container. In that demonstration, we "unzipped" a PPTX and took a look at the files. For this exercise, take a look at the DOCX file in the course sample files; you will find a file named `inventory.docx` in the folder named `PKG-legacy-files`. First, open the file using Microsoft Word or a similar document editor; look for the file properties. Can you determine who created the file, and when it was created? Does the creation time match the creation time listed in the file system? Next, "unzip" this `docx` file, and take a look at the results. Answer these questions:

1. What folders and files can you see now?
2. When you opened the file in the Word editor, you may have noticed there is an image in the file. Can you find that image? (Hint, it's name is image1.png.) Where is that embedded image stored? 
3. Can you find the original creation date of the file? Where (what file) contains that creation date, and where is it in the unzipped DOCX structure? (Hint, it's metadata and will be stored in an XML file, once the file is unzipped you can search files in VSCode with Ctrl + F.)
4. Imagine you were a curator tasked with preserving access to this file. What functionalities do you think you would want to preserve? What software might be required to preserve this functionality?  

## Problem 2: The `file` command {#problem-2}

Use the file command to inspect files. Start by looking through all of the files in the `PKG-text-data` directory.

1. First, determine how many files you're looking at (use `wc`). What is the command? How many files are there?
2. Create a command to run file so that it loops through all of the files in the `PKG-text-data/` directory and outputs file characterization information to the terminal display. Examine the results. These are all "text files" but there are different results. Can you identify different text encodings? What else does the output tell you about the files?
3. Reuse the loop you created above to save the output to a file called `text-file-types.txt`.

## Problem 3: Checksums {#problem-3}

**Create checksums.** Checksums are algorithmically-generated strings that can be useful to track file fixity.

1. To create an md5 checksum, what command do you use?
2. Use the `md5` or `md5sum` command to create checksums for all of the TXT files in the text-data directory. What command would you use?  
3. Output the list of checksums to a file called `txt-file-checksums.txt`. Provide the command that you used.

## Problem 4 {#problem-4}

In the previous two problems you created a checksum and listed file types. Do you think this information would be useful to keep as "preservation desciption information"? Why or why not? What benefit is outputting this information to a file that you might want to keep with the folder if you were going to hang on to it for a while?

## Problem 5 {#problem-5}

Choose one of the sample datasets for Assignment 1 ([view assignment 1 in Canvas](https://umich.instructure.com/courses/733396/assignments/2649533)). Use these questions to make a preliminary analysis using the sorts of tools and questions we've been asking so far:

1. What dataset did you choose? What drew you to this dataset?
2. For this dataset, identify at least one file type that appears to hold data. What is the filetype? How can you find out more about the file type?
3. Try to download one (or more) file that you identified above.
4. Is it easy or difficult to identify the file, to download the file? Is there any information that you might use to demonstrate provenance or authenticity about the file in the access interface? (For example, how big is the file, a hash value, creator, filename, creation/modification date, etc?)
5. Using command line tools (i.e., `file` or siegfried/brunnhilde), can you get detailed technical information about the file? Can you identify MIME types? Can you get basic information like who created the file and when? If you were able to identify any file information in the previous step from the data interface, does this agree with the information you found from this closer inspection of the bitstreams?

## Submit Your Work on Canvas

Please submit your responses via Canvas, using [this assignment link]({{ page.canvas-link }}).
