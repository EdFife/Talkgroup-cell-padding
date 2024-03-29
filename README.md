Talkgroup-cell-padding
Python script to add user defined digit and pad the talkgroup field to 7 digits for use with Ham radio DMR hotspot software custom configuration of Pi-Star or WPSD hotspot software.
This helps format your talkgroups correctly for custom talkgroup routing rules.

Script written for Windows environment since most DMR radios only have windows apps for codeplug manipulation. 

Requires Python3,  Python modules os, csv, tkinter.

Written by Ed, KE8TES

Frustrated to have to pad out TG cells again I wrote this quick script. 

This will work on all talkgroup lists to pad out the Talkgroup number to 7 digits for Custom network configuration. 

To Use this script:

1. Download .csv file for you talkgroup listing
2. Execute the script
3. Input your first digit for talkgroup padding 
4. Select your file when asked
5. Script outputs files in same directory as original  file
6. Files are named TG_x_List.csv and TG_x_Errorlog.csv

The error log file only is created if talkgroups exist in original list equal to 7 digits then they are processed to see if any with 7 have same first digit as your leading digit and if so they are added back into the TG_x_List.csv file and the other 7 digit ones written to TG_x_Errorlog.csv

When creating this script I realized there are some talkgroups with 7 digits already and some of those did not have 4, 3 etc. as their leading digit. 

***** Note: This script will work with whatever digit you want from 1 - 9. *****

So I pulled out those with 7 which did not start with the desired leading digit; saving them to error file so they did not corrupt your codeplug in case they were overlooked.

I did not add header row to the output files as you typically are just pasteing the files together anyway and some talkgroups lists have headers and some do not.

***********************************************

Please use and modify as you see fit.

73s, Ed
