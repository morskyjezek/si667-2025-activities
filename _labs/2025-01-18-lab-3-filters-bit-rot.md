---
layout: post
title:  "Lab 3: Filters, Bitstreams, and Simulated Bit Rot"
date:   2025-01-18
assigned: 2025-01-23
due: 2025-01-28
key: lab-3-key
canvas-link: https://umich.instructure.com/courses/733396/assignments/2649540
categories: lab
---

Record answers for the following questions:

## Problem 1 {#problem-1}

**Question:** Viewing the file's bytes. Choose one of the JPG files. Investigate and answer:

1. What file are you working with?
2. Look at the first 16 bytes. What do you see? Can you confirm that this is a JPG file?
3. What two-byte sequence represents the SOS marker in a JPG file? (see above, represented in hexadecimal)
4. Where does the image stream start? (In other words, what is the byte offset of the SOS marker? This is shown in decimal/hexadecimal at the lower right of the VS Code window.)
5. Look at at least one TIFF, PNG, and SVG file using the same process. Can you identify the file signatures there? (Refer to the list of file signatures under Resources.)

## Problem 2 {#problem-2}

**Question:** Modifying the bitstream, or more interestingly, creating Glitch art: Use the files in the "PKG-images" directory. Choose one of the JPG files. Investigate the following and answer the questions:

1. What file are you examining?
2. Create a copy (you can do this using "Save As..." in VSCode, or copying in your GUI file navigator, you can use the cp command)
3. Open the copied file in a hex viewer. What are the first two bytes in hexadecimal notation?
4. Locate the "Start of Stream" (SOS) marker. Modify anything after that - insert, copy or cut and paste, delete.
5. Save the file, open it in an image viewer, and see what's happened.
6. You may want to iterate on this a few times, or retry. Sometimes it's interesting, sometimes it's not.

## Problem 3 {#problem-3}

**Question:** Create checksums for the JPG files (including your newly created "glitch art" from the previous question!)

1. Use the command `md5` (Mac) or `md5sum` (Windows/GitBash) to create and record the checksum for each of the JPG files. What is the command you will use to do this in one command?  
2. List the names of the files and the corresponding MD5 checksums for each of the JPG files in the directory.
3. If the command line tools aren't working for you, try out the Web-based checksum tool linked above.
4. _Goal:_ a report that lists the MD5 checksum and the file name, separated by a space, on a single line for each file

## Problem 4 {#problem-4}

**Question:** Compare the checksums of the files related to your glitch art, specifically the original and modified files. Are they the same or different?

## Problem 5 {#problem-5}

**Question:** What do you find notable about viewing files in this way? What is the difference between the text files (extensions like: txt, csv, md) and the graphic files (extensions like: jpg, tiff, png)?

## BONUS

Try reopening any of the graphic files that you edited (tif, png, jpg, etc) with a graphic viewer (like a web browser, Mac Preview, or other program). Can you view the files as graphics? If the files are inaccessible after you edit them, what do you think broke these files? Were there any files/filetypes that didn't "break" as easily?

To earn one extra point: Post any interesting images that are created in the online discussion: Glitch Art Gallery on Canvas.

## Resources {#resources}

To see the process, review the last slides from the Week 3 slidedeck.
Here are a few other online resources that you might find useful:

* JPEG article on wikipedia: [https://en.wikipedia.org/wiki/JPEG](https://en.wikipedia.org/wiki/JPEG).
* JPEG discussion that notes signatures/markers (Tachibanaya): [https://www.media.mit.edu/pia/Research/deepview/exif.html](https://www.media.mit.edu/pia/Research/deepview/exif.html).
* JPEG description from Library of Congress: [https://loc.gov/preservation/digital/formats/fdd/fdd000017.shtml](https://loc.gov/preservation/digital/formats/fdd/fdd000017.shtml).
* File signature reference list (wikipedia): [https://en.m.wikipedia.org/wiki/List_of_file_signatures](https://en.m.wikipedia.org/wiki/List_of_file_signatures).
* VS Code Hex Editor extension: [https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.hexeditor).
* Online hex editor: [https://hexed.it/](https://hexed.it/).
* Checksum calculator: [https://codebeautify.org/checksum-calculator](https://codebeautify.org/checksum-calculator).

If you're having trouble getting the hex view, here are examples:

* A hexdump of a small png file: [https://github.com/morskyjezek/si667-2025/blob/main/simplepixel-hexdump](https://github.com/morskyjezek/si667-2025/blob/main/simplepixel-hexdump).
* The file in the course file collection: [https://github.com/morskyjezek/si667-2025/blob/main/simplepixel.png](https://github.com/morskyjezek/si667-2025/blob/main/simplepixel.png).
