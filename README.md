# ME 701 -- Homework 1 -- Zach Kowal

## Instructions

Your solution should be an update to this `README.md` file that will be
committed back to your repository created when you clicked the HW 1 link.

## Problem 1 -- Open-Source Software

### Statement

Think of the things you do routinely on a computer that require
specific software packages.  Find an
open-source solution from the software repository
for one of these activities and tell me about it in 100 words or less.
For example, I used to do lots of audio recording when I was in
high school (not *that* long ago) and used special (and
pretty expensive) tools like
Cakewalk Sonar.  Since then, I've found an
open-source package for doing multitrack
recording called Ardour that doesn't have all the bells and
whistles but, because I can program in C++ and the
source code is available, I could, in theory,
create any such whistles I need.  **Note**: You may not
describe anything already discussed in class (e.g., the LibreOffice suite
or Octave).

### Solution

Often when using the windows media player, videos will load slowly. To circumvent this, I use an open source software package called VLC Media player. VLC media player can play all sorts of videos, screenshot individual frames, convert file types, along with other functionality. I enjoy it because it loads faster and I have more tools to use in general.

## Problem 3 -- Your CPU

### Statement

Figure out how to display information about your CPU via the
command line.  This should include at least the **processor
speed** and the **number of cores**.  Describe your command(s) below.
(Hint: redirection is helpful; remember, that's like
using `ls > directory_contents.txt` to dump the contents of a directory to a file.

### Solution

To display CPU information, I used the following command:

```bash
lscpu -p=CORE,MHz # This displays core numbers and associated speed. Core numbers are indexed from 0.
```
From there, a list of details is displayed on screen, among which is processor information and cores. Because the cores are indedxed form 0, the total number of cores is the highest number plus 1, and the clock speed for each core is listed (which should all match the processor speed).

## Problem 4 -- Resource Hogs

### Statement

Figure out how to list the programs that use the most
amount of (1) processing and (2) memory.  Describe your command(s)
in your writeup.

### Solution

To display a list of processes with resource usage, I used the following command:
```bash
ps aux
```

This displays a list of processes, the user associated with the process, along with the %CPU and %MEM usage for each of them.


## Problem 5 -- `bash`

### Statement

Where is `bash` located on your Linux system?  And what version of
`bash` are you using?  Make sure to provide any commands you use to
determine this information.

### Solution

To find where bash is located on a linux system, the following command can be used:
```
which bash
```

This outputs the path /user/bin/bash .

To find the version of bash, this command can be used:
```
bash --version
```
This outputs the GNU bash version and license information, of which my bash is version 5.1.16(1)-release (x86_64-pc-linux-gnu)
