# IMS(Interactive Music Shell)<a href="https://codeclimate.com/github/FrankYan93/pa-ims"><img src="https://codeclimate.com/github/FrankYan93/pa-ims/badges/gpa.svg" /></a>
# Author
- **Jiadong Yan**

# Brief Intro
This is a little ruby shell program that records tracks and artists and the play frequency.
# Getting Started
After `chmod u+x ims`, you can run the program just type `./ims`  
There are two files **ims and ims.rb** work as main entrance of the program.  
Their content is same.   
You can run ims either by `ruby ims` or `ruby ims.rb`.
I've tried **PStore** and **YAML:Store**.
PStore is quick but not readable while YAML:Store is readable but not so quick.

# Data
{    tracks => an array includes artist and played times,
  ...  }

# My Solution:  
  class `IMS_Loop` :do the loop job  
  class `Commmand` :respond to user's commands  
  class `Track_artist` :display and add track,artist pair to YAML:Store  
  JSON data :store the data to and from YAML:Store  
  Hash data0 :transform data into hash to do the job easily, then restore to data  

  use `case` to switch from different commands,  
  identify ` by ` to seperate track and artist,  
  use a class `Track_artist` to add new tracks and display,  
  command `Help` to see all commands.  

# Unit Test
**test_ims.rb** used for testing some commands's performance.


## Thank you for reading.
## Version 12/9/2016
