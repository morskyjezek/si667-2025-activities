---
layout:   post
title:    "Lab 5: File Metadata 2 - Embedded Metadata and Inventorying"
date:     2025-02-04
assigned: 2025-02-07
due:      2025-02-13
key:      #lab-5-key
canvas-link: https://umich.instructure.com/courses/733396/assignments/2649542
categories: lab siegfried brunnhilde metadata inventory
---

This lab moves file inspection activities from identification and file types to embedded metadata. This week's lab questions are prompts that aim to guide you in the file inspection process and to reflect on the information that you can glean in this process. The problems below are designed to run on the course files, which you have previously downloaded, and that the directory is named `si667-2025`.

Note: [First consult the accompanying guide on installing and using Siegfried and Brunnhilde]({{ site.baseurl }}{% post_url 2025-02-03-guides-running-siegfried-brunnhilde %}).

# Lab Questions

The lab questions focus on two tools: Siegfried and Brunnhilde. These tools will be demonstrated again in class, but work through these problems to start gaining familiarity with the tools.

## Problem 1: Setup {#problem-1}

These tools will generate reports about the files in the directory, so you will first create those directories. Use the `mkdir` command to make two new directories in the directory one level above the course files, one titled `sf_out` and the second `br_out`. For example, if you have saved the course files in a folder you use for the course titled `si667-notes`, create these new directories in that notes directory.

## Problem 2: Running Siegfried {#problem-2}

Siegfried is a useful tool to create an inventory and a bulk process for file characterization information. Run the command on the `si667-2025` directory and output the reports to the `sf_out` directory.

1. At the prompt (located one level above the si667-2025 directory), run the command `sf si667-2025/`. What did the command do? (What files and directory have been created by the command? What do you see in the files?)
2. At the prompt, enter the following command: `sf si667-2025/ > sf_out/sf_fileid_report_202502.yaml`. Now what happens? What did the command do?
3. The previous command should have created some new files in the `sf_out` directory. Open the `sf_out` directory and look around. Answer the following:
  1. What did the command do?
  2. What does the file tell you?
  3. Open the new file in a text editor (e.g., VS Code). How would you characterize the data presented in the file?
  4. Does anything strike you as particularly useful? What is odd or questionable about the output?

## Problem 3: Running Brunnhilde {#problem-3}

Brunnhilde produces useful summary reports, as well as the detailed, item-level reports of Siegfried. Your task is to follow the steps demonstrated in the screencast to run `brunnhilde.py` to analyze the files in the sample file group (instructions on the slide titled, ["Run Brunnhilde"](https://docs.google.com/presentation/d/1MGSl026DkESWXIOaCNw8tLdZCVhv5Iq1i_WNfGFPxjU/edit?usp=sharing)). Look at the files that were output when you ran the script, and answer the following:
  1. What did the command do? (What files and directory have been created by the command? What do you see in the files?)
  2. Focus on the `report.html` file that was created. Take a look at the report (open it in a browser to read it): are there duplicate files, if so, how many? What is the most common image type file (check the MIME Types)? What is the most common application type of file?
  3. Are there any duplicate files? If so, what are they named, and how do you think duplicates are identified here?
  4. In the `report.html` file, look at any of the tables with an "ID" column. What is the information in this column? If you click on any of the links in these columns, where does it take you? What information can you learn at these links?
  5. Look at the "unidentified" section of `report.html`. Could you identify any of the files that are listed there? Why do you think the tool was unable to identify these? Now look at the "warnings" section of `report.html`. How could the information in this section be used to address the questions left in the "unidentified" section?

## Submit Your Work on Canvas

Please submit your responses via Canvas, using [this assignment link]({{ page.canvas-link }}).
