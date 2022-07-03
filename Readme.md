# OVERVIEW
## Report
In-browser cryptojacking is an urgent threat to web users, where an attacker abuses the users' computing resources without obtaining their consent 
Our task was to built a In-browser detection system, We Deviated a bit from the intially built work flow though there were not many changes we faced some difficulty while using or import a certain library.
Firstly, We decided to built a Html script so we can monitor the resources of the CPU while running the script with the JS library embedded into the code,  We were faced with a problem, We could not find any working JS library used for crypto jacking we tried using coinhive but it was found that the domain of the coin hive lib was bought by another company. then we did some research and found another library known as coinimp which did not meet our standards as It was not that resourceful and we had to build a proper account to manage the library, We came upon this website Known as browsemine which converts your browser into a crypto mining system, we choose this library to embedded into our code which worked brilliantly.
We chose python as a goto language to implement our system as it gave us idle environment to monitor the browser and the processes.

MODULES:

Module no.1:
STATIC ANALYSIS:
The first module is designed to take a URL from the user to extract the java script libraries used in the HTML script of the website and stores the used libraries in a file named “Java_Libs.txt” this part was implemented by using two Libraries Beautysoup to organize the HTML code and request to capture the website
Module no.2:
DYNAMIC ANALYSIS:
In the second module we have used two libraries matplotlib and psutil. 
Matplotlib is a library used to plot graphs, the second library we have used is psutil, 
It is a library used to access the information of the resources of the hardware of the machine.
we have used psutil to extract the CPU usage as time progresses and used the matplotlib to plot a graph for the CPU usage as well as its Temperature and the temperature of Core 1 over the period of  TIME, we have also used this library to extract the information of the processes running on the system, 
It prompts the user if a process is using too much CPU displaying its memory usage and the Process ID of the process. it also detects if the processes are running on the browser or not. It is also designed to store the information of the processes running on the browser.

Module no.3:
We have designed this module to sniff the network traffic and the size of data being passed through the network, by the Psutil library. 
Initially we had planned to use pyshark in this module but for some reason it was not being imported to our code that is we had to use psutil else Pyshark may have given an advantage to calculate and monitor the network.




