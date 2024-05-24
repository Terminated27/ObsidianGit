Termux:tasker is a tasker plugin which allows us to run commands in termux. Termux has huge amount of packages that can be installed for different purposes (for example 7zip, ffmpeg, youtube-dl , etc etc).

Termux is no longer updated on play store due to newer android restrictions (on android>=10 binaries cannot be executed from data directory). Hence termux still targets sdk 28(android 9) so it can execute binaries. Updates for termux and termux:tasker will be released on f-droid only. For the same reason you cannot just put android binaries in tasker data folder and execute it because tasker targets sdk>28. This makes it necessary to utilize termux:tasker to automate commands involving binaries and linux packages.

Preparing the plugin (one time only)

**Step 1**  
Download [termux](https://f-droid.org/en/packages/com.termux/) and [termux:tasker](https://f-droid.org/en/packages/com.termux.tasker/) apps from fdroid. F droid is a repository of open source apps. Make sure both termux and termux:tasker are fdroid version and not play store. If you want to use termux available on play store you will need to buy and install termux:tasker from play store.

**Step 2**  
Open termux and type `termux-setup-storage` and allow storage permission to termux.

**Step 3**  
Open [this pastebin link](https://pastebin.com/raw/2VKmB1k9) and copy all the code to clipboard, or copy the code from below.

`mkdir -p /data/data/com.termux/files/home/.termux/tasker`  
`chmod 700 -R /data/data/com.termux/files/home/.termux`  
`echo -e 'cp "/sdcard/Tasker/$1" "/data/data/com.termux/files/home/$1"\nchmod +x "/data/data/com.termux/files/home/$1"\n"/data/data/com.termux/files/home/$1"'>/data/data/com.termux/files/home/.termux/tasker/tasker.sh`

**Step 4**  
In termux app, long press on terminal screen and paste. Then press enter key. This will make a tasker.sh script in termux directory. I have made this script for ease of use of this plugin for a normal user.

**Step 5**  
Open your settings app, then "App and notifications" and open app info of tasker. Goto permissions. Scroll all the way down and click on "Additional permission". Allow the permission for "Run commands in Termux environment".

All done! You have successfully setup termux:tasker

Now how to execute a script/commands.

**Step 6**  
Open your file manager and navigate to Tasker directory on Internal storage. Make a new file with .txt extension. For example lets say you have made a file with name myscript.txt.

**Step 7**  
Open myscript.txt with a text editor and write the commands in it, like you would do in a shell script. For example lets assume you have written "echo hello" in 1st line, and "echo hello world" in second line. Quotes are not included.

**Step 8**  
Open tasker. Make a new task>plugins>tasker:termux . Open the configuration window of plugin. In executable type "tasker.sh" (quotes not included). In arguments type the name of file in /sdcard/Tasker directory that you want to execute. Here we are executing the "myscript.txt", so type "myscript.txt" in arguments field(quotes ARE included).

Thats all, save your configuration and execute the task. Output is stored in %stdout

[Video tutorial](https://youtu.be/puTNGGyHEmo)

# Ammendum
FYI, you don't need to create physical script files in Termux:Tasker `>= v0.5`, just store them in tasker variables and sent them to [tudo](https://www.reddit.com/r/termux/comments/kd31lw/termuxtasker_version_05_and_tudosudo_scripts/?utm_medium=android_app&utm_source=share) as an argument for execution.

And you should **NEVER** store scripts in public external sdcard storage, a malicious app could modify them and run commands in termux context or even root context if termux has been granted root permissions. There is a reason you normally can't execute scripts directly from public sd card storage, you are just bypassing that safety. And running a copy operation everytime you run a script will have a slight performance impact as well.

If you want to use script files, store them in `~/.termux/tasker` using termux SAF provider, check [Creating And Modifying Scripts](https://github.com/termux/termux-tasker#Creating-And-Modifying-Scripts) section of Termux:Tasker `README`.