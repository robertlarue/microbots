# microbots
A TCL Expect script for playing [textMMOde.com](http://textmmode.com), a space MMO that can be played through telnet.  
The script adds a menu for completely automated trading and navigation to any sector

##Getting Started##
1. Make sure you have [Expect](http://en.wikipedia.org/wiki/Expect) installed  
    You can download it (Windows/Linux) [here](http://expect.sourceforge.net/).  
    If you have a Debian/Ubuntu based system, simply ```sudo apt-get install expect```.  
    Mac OS X users should have Expect installed already.

2. Clone the repo [here](https://github.com/robertlarue/microbots.git) or download the [zip file](https://github.com/robertlarue/microbots/archive/master.zip)

3. Open the microbots directory

4. Edit the microbots_config file  
    Replace ```<enter username here>``` with your username  
    Replace ```<enter password here>``` with you password

5. Then run the microbots script from a terminal  
   On all platforms:  
    ```expect -f microbots```  
   On Linux/OS X only:
   Make the script executable and run it   
   `chmod 777 microbots`  
   `./microbots`  
   The script will log you in automatically and bring you to the familiar textmmode.com interface
7. Open the new microbots menu by pressing the [tilde](http://wiki.unvanquished.net/images/9/96/Tilde_key.svg) key   
   The menu offers serveral options
   * Auto Trading (Press A)
   * Auto Navigation (Press N)
   * Showing your current XP and Microbots (Press S)
   * Exiting the menu (Press X)

The menu should look like this
```
Menu Options:
Autotrade(a)
Auto Navigate(n)
Show Player Stats(s)
Exit Menu(x)
Menu Choice:
```


##Auto Trading##
Allows you to quickly level up or get microbots.  
Enter Auto Trading mode by pressing the tilde key and then pressing the A key.  
It will then prompt you for an Auto Trading goal. 
You may input a number for one of the following three categories:  
   * Iterations
   * Microbots
   * XP

Simply press enter to skip one of these categories.
###Examples###
####Complete x number of trades###
If your goal is to complete a certain number of trades, at the first prompt input the number of iterations you would like to complete then press enter.  
Then press enter at the next two prompts without inputting any numbers.
####Reach a certain number of microbots(cash)####
If your goal is to reach a certain number of microbots, press enter at first prompt without inputting any number.  
Then at the second prompt, input the number of microbots you would like and press enter.
Then press enter without inputting any numbers at the third prompt.
####Reach a certain XP (for leveling up)####
If your goal is to reach a certain XP, press enter without inputting any numbers at the first two prompts.  
Then input the XP you would like at the third prompt and press enter.

##Auto Navigation##
Useful for getting to trading posts (2001, 4001, 6001, etc.) or spaceports.  
Enter the Auto Navigation menu by pressing the tilde key then pressing the N key.  
Then enter the sector number you would like to travel to.  
If you are travelling a long distance (e.g. sector 1 to sector 300000), it may take a few seconds.  
Also be aware that you cannot travel to sectors outside of your star cluster  
(e.g. the Sands of Time core is located in sectors 1 - 400000)
