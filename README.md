Fusuma is multitouch gesture recognizer. This gem makes your linux PC able to recognize swipes or pinchs and assign commands to them.


襖(Fusuma) means sliding door used to partition off rooms in a Japanese house.

Installation
1. Grant permission to read the touchpad device
IMPORTANT: You MUST be a member of the INPUT group to read touchpad by Fusuma.
$ sudo gpasswd -a $USER input
Then, You MUST LOGOUT/LOGIN or REBOOT to assign this group.

2. Install libinput-tools
You need libinput release 1.0 or later.
$ sudo apt-get install libinput-tools

3. Install Ruby
Fusuma runs in Ruby, so you must install it first.
$ sudo apt-get install ruby

4. Install Fusuma
$ sudo gem install fusuma

5. Install xdotool (optional)
For sending shortcuts:
$ sudo apt-get install xdotool

Touchpad not working in GNOME
Ensure the touchpad events are being sent to the GNOME desktop by running the following command:
$ gsettings set org.gnome.desktop.peripherals.touchpad send-events enabled

Usage
$ fusuma

Update
$ sudo gem update fusuma


Customize Gesture Mapping



Config file for touchpad gestures on linux machine



Gestures



Mult-touch Gesture | Action |


3 Fingers - Left | Go Back on Browser |


3 Fingers - Right | Switch to last app |


3 Fingers - Up | Show all applications |


3 Fingers - Down | Show all Windows |


4 Fingers - Left |View split screen on left |


4 Fingers - Right | View split screen on right |


4 Fingers - Up | Next Desktop|


4 Fingers - Down | Previous Desktop|
