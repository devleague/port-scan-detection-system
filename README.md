# DevLeague Cybersecurity Professional Assessment

### _We need your help._

We have reason to believe that we have been the target of some malicious activity against our network but we're having a hard time tracking down if our suspicions are correct or if paranoia is getting the best of us. We possess some of the greatest secrets known to mankind.

We're not really sure where to begin and we're hoping you can be of assistance. We have been provided some network traffic logs by our IT network operators and we need to examine them for signs of malicious activity and determine if our suspicions are correct.

All we know is that we have the provided log file from our network adiminstrator and the following message from an anonymous source:

__SECRET KEY:__ If they're scanning you, it would probably be using a tool called **Nmap** to perform scan events on your network...
___
### Your Mission
We need you to take the following steps so that we can continue to ensure peace within the galaxy:
1. Create a new directory(folder) called `devleague_discovery` on your computer that you will use for all files related to your analysis.
1. We have given you a download of our provided network SSH log file to download to your new directory at this link: [SSH Log file](https://raw.githubusercontent.com/devleague/cyber-assessment/master/data/ssh.log.txt)
1. After you download the log file, we need you to use your Python skills to write a script that will automatically find instances of malicious activity in our logs.
2. Create a Python file named `scanners.py` where you will write your Python code that will read the `ssh.log` file from the file system
2. When running your Python script, it should create a text file named `scanners_found.txt` that reads all rows in the file and searches for certain text, and gives us the following summary information after analyzing the log file:
    - Displays a count of how many scan events occurred in the logs
    - Displays a list of all host ip addresses where the scans originated from
    - Displays a list of all host ip addresses where the scans were performed against
1. Your final report should include the `scanners.py` and `scanners.txt` files, as well as a summary of any new facts you discovered in your analysis and the procedures you took to complete the challenge.
1. If you could also make some recommendations to keep our network secure we will be able to sleep at night.
1. Provide us with the necessary report documents in a zip archive when completed.

___
The following resources may help you in your mission:

#### Sample Python File for Reading Files
```Python
import os
import re

filePath = "./ssh.log.txt"
fd = open(filePath, 'r')

with fd as reader :
    for line in reader :
        print( line )
```

#### Sample Output for Analysis File
```
[scan attempts] 1234

[scan origin hosts]
  XXX.XXX.X.XX
  ...
  ...

[scan destination hosts]
  XXX.XXX.X.XX
  ...
  ...
```

#### Helpful Resources:
https://automatetheboringstuff.com/#toc

https://www.bro.org/sphinx/logs/index.html#working-with-log-files

https://duckduckgo.com/

##### Make sure to check back in for additional clues as needed.


