# Light_Schedule
Light relay for an aquaponic grow system that is controlled by the daily sunrise and sunset times of Portland, OR. 

We use MATLAB code to read daily sunrise and sunset times from the website https://sunrise-sunset.org/ (specifically for Portland, OR data: https://sunrise-sunset.org/search?location=Portland%2C+OR%2C+United+States ).

Once we retrieve this data we convert into a character array, then a numerical array, eventually to be converted into the daytime array for MATLAB so we can speak to Thingspeak.com

From the description in the MATLAB code:  
"This script will grab the most current sunset and sunrise 
  times of Portland, OR, convert it to datetime arrays and let Matlab
 determine whether to turn the light relay on or off based on the current
 time. In addition, the state of the relay will be sent to ThingSpeak and
 produce a plot on a field. Matlab will then check if the data sent is
 equivalent to the data stored on ThingSpeak."


From the description in the arduino code:
" This Arduino code should make a beefcake relay switch on and off accordingly to a
  Matlab script that is communicating to it over serial. "
  
  Thanks to the previous PCC students for writing much of the previous Arduino code.
