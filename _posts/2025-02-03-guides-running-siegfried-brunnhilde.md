---
layout:     post
title:      "Running Siegfried & Brunnhilde"
date:       2025-02-03
categories: brunnhilde siegfried guides
---

This page contains the instructions for running tools that can help with file reporting. These are useful tools that can create some of the preservation description information, which might accompany an information package, and to create technical information that can be used for tracking file integrity and duplication.

# Setup

The following sections show how to get set up to run the file reporting tools.

## Sample Files

All of the activities will use the course's sample files, which you should have previously downloaded during class in January. If you didn't download them, have lost those files, or want a new copy, they are located in the course github repository, and you can download them all directly as a zip file at [{{ site.course_data_download_link }}]({{ site.course_data_download_link }}). Unzip that folder somewhere on your computer, for example in your `Desktop` or `Documents` folder. This should result in a folder named `si667-2025`, which will match the demonstrations below. (_Nota bene: the files below were recorded in 2023 and the folder in the video shows the year 2023 in its name._)

# Install Siegfried

To install Siegfried, follow the instructions at the tool's site: [https://www.itforarchivists.com/siegfried/#install](https://www.itforarchivists.com/siegfried/#install). These instructions work well if you're using a Unix-style system (such as a Linux machine or Mac OS). The instructions use another tool, HomeBrew, which is a useful utility to manage command line programs, and if you need that, see the program's homepage for good installation instructions (note that it will require an internet connection): [https://brew.sh/](https://brew.sh/).

If you're running on a different style of system (like Windows), the instructions are a bit less specific. If you have had trouble following those instructions, [try these step-by-step instructions for Windows]({% post_url 2025-02-09-guide-installing-siegfried-windows-11 %}). Linux systems may require more modifications.

# Install Brunnhilde

Brunnhilde is a python-based tool, so you can install it as you would other Python extensions using `pip`. The process is explained on the tool's site: [https://github.com/tw4l/brunnhilde#installation](https://github.com/tw4l/brunnhilde#installation).

If those instructions aren't working well, here is a [Windows-specific walkthrough of the installation process](https://docs.google.com/document/d/1LKZA3ahzkM-Ic7w17f-doHIA342oKoS8kxROPKYOtqI/edit?usp=sharing).  

# Check if the tools are running

This screencast shows how to see if the tools are running:

<iframe width="560" height="315" src="https://www.youtube.com/embed/z1GOoispJ5k?si=v13jCbDgm1nx6j1R" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

&nbsp;

# Running `brunnhilde.py`

This screencast explains how `brunnhilde.py` works and demonstrates how to run the command:

<iframe width="560" height="315" src="https://www.youtube.com/embed/yuZQmpnjKhE?si=zvCO1X2RUB8iCNSd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
