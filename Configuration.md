# Introduction #

Here's a reference for the configuration options at the top of the file.

# Screenshots #

ArcherSeven's hosting screenshots for easy viewing.
http://archerseven.silverirc.com/screenfetch/pics/

# Reference #

## distro ##
This setting controls what ASCII logo / label and text color scheme is displayed in the final result. This can be set to one of the following values: Arch Linux, Debian, Ubuntu, Crunchbang, Linux Mint, Gentoo, Fedora, BSD, None.

## display ##
This setting controls what information is displayed in the final result. Possible values are: OS, Kernel, Uptime, DE, WM, Win\_theme, Theme, Icons, Font.

## textcolor and labelcolor (optional) ##
This setting controls the color of the information text in the final result. This follows standard Bash prompt color codes. This does not have to be set, and is recommended to not be set, but if you must, uncomment these two lines and set them as desired. The reason these do not have to be set here is because they are set individually depending on what you set in “distro”, using the color scheme of that distribution’s logo.

## wmnames ##
This is a list of supported Window Manager process names for screenFetch. This list is used to scan the process list of the machine running the script and determine what Window Manager it is running of these. To add more WM’s to screenFetch, you would have to add the process names of those WM’s here. This setting does not need to be messed with.

## denames ##
This is a list of supported Desktop Environment process names for screenFetch. This list is used to scan the process list of the machine running the script and determine what Desktop Environment it is running of these. To add more DE’s to screenFetch, you would have to add the process names of those DE’s here. This setting does not need to be messed with.

## screenie (IMPORTANT) ##
This setting controls whether screenFetch will actually take a screenshot upon execution or not. Values are as follows: 0 = No screenshot, 1 = Screenshot. By default, this is set to 0, so if you are planning to take a screenshot using screenFetch, you MUST set this to 1 or specify -s|--screen on the command-line when executing the script.

## screenCommand (optional) ##
This setting can be used to specify a custom screenshot command. Just uncomment and edit. Otherwise, screenFetch will use the default command of “scrot -cd3”.