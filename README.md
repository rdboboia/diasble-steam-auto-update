# diasble-steam-auto-update
A script that disables Steam's auto update for each installed game.

## How to use it
Inside the "workspace" tag there are 2 variables that can be editted.
The first variable sets the temporal folder's path where the temporal files will be stored. This can be left as it is if you didn't remove your system's %temp% environment variable.
The second variable sets the Steam's steamapps folder which is where the required files are found. This second variable should be editted in order to match your Steam installation. The default configuration should look like this: "C:\Program Files (x86)\Steam\steamapps".

## What this script does
There are comments inside the script that I think are enough to understand how the script works. However, if you want a brief explanation: the script reads all .acf Steam files that are inside the steamapps folder, checks if they have the expected configuration for the "Update only at launch" behavior and asks the user for confimation if changes are needed, changing Steam's files.
