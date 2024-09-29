# fOSC v1.1.2

## Introduction

A Cinema 4D Plugin for listening to OSC messages. 
Listen to specified port and map incoming data to generated Null objects. 

## History

Based on [NI Mate OSC Receiver](http://www.ni-mate.com/). 

Improved & redesigned by [FillMember](mailto:hi@fillmember.net). 

## Installation

Clone the git repo to, or download the git repository and place the content to
```
Windows:
C:\Users\Name\AppData\Roaming\MAXON\CINEMA 4D R1x_xxxxxxxx\

MAC:
~/Library/Preferences/MAXON/CINEMA 4D R1x_xxxxxxx/plugins/fOSC
```

Tested on R14+. 

## Get Started

1. Open fOSC dialog from Plugin menu. 
2. Check "Create Nulls Objects" to enable fOSC to automatically create Nulls Objects for you. 
3. Click "Start Listening" to start listening to OSC messages. 
4. The plugin will listen to localhost (127.0.0.1).  
In your choice of OSC client, direct your OSC messages to localhost (127.0.0.1), and the port specified in the plugin (The default port is 7000. )
5. Every OSC message received will be represented as a Nulls Object in C4D.  
The name of the Nulls Objects will be the name of the message, the first 6th numbers will be mapped to position X, Y, Z, and rotation H, P, B. 

## Usage

1. Use XPRESSO, Drive/Driven to map the values to other objects.  
It is advised to store the XPRESSO atg or any other addtional tags on targeted objects or objects other than objects generated by fOSC. 
2. When you no longer want Nulls Objects being created automatically, uncheck "Create Nulls Objects".  
You can also manually create Objects within fOSC container, as long as the name matches the messages you're mapping to. 
3. To record incoming message, check "Record Incoming Data".  
Keyframes will be created on the current position on timeline. You can also change Frames Per Second in Cinema 4D to record slower or faster. 

## Tips

- Numbers mapped to rotation are converted to show the original value in degrees.  
integer 30 ---> 30 degree  
float 3.14159 ---> 3.14159 degree (instead of 180 degree)

## References

* [Open Sound Control](http://OpenSoundControl.org)
* [NI Mate](http://ni-mate.com)
* [KiCapOSC](http://www.908lab.de/?page_id=215)

## Questions & Contact

[Ten (fillmember)](mailto:hi@fillmember.net)
