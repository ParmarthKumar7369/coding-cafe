**1.** pwd printed /home/parmarth i.e. **the path of directory im currently in.**

**2.** ls -a displayed **all the hidden system files** which ls didn't.

**3.** The first column **shows the file type and permissions**.

**4.** coding-cafe/week02 is a **relative path.**
The path works because coding-cafe is inside the current directory, and week02 is inside coding-cafe.

**5.** First, mv README-backup.md week01/ **moved the file from the current directory into week01**. Whereas, 
mv README-backup.md old-readme.md **renamed the file inside week01 from README-backup.md to old-readme.md**.

**6.** There are 19 folders on my PATH.
> /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/wsl/lib:/mnt/c/Windows/system32:/mnt/c/Windows:/mnt/c/Windows/System32/Wbem:/mnt/c/Windows/System32/WindowsPowerShell/v1.0/:/mnt/c/Windows/System32/OpenSSH/:/mnt/c/MinGW/bin:/mnt/c/Users/parma/AppData/Local/Microsoft/WindowsApps:/mnt/c/Users/parma/AppData/Local/Programs/Microsoft VS Code/bin:/mnt/c/Users/parma/AppData/Local/Python/bin:/snap/bin

**7.** The location to my python is **/usr/bin/python3**

**8.** Yes, both the paths are **same**.

**9.** The shell said:
> Command 'pyton3' not found, did you mean:
  command 'python3' from deb python3 (3.14.3-0ubuntu2)
Try: sudo apt install <deb name>

Therefore, after searching every folder in our **PATH**, the shell told us that the command was not found. While it also told us what might be the possible error that we have made.

**10.** As **.venv is a hidden system** file(starts with a .), therefore ls couldn't display it as it doesn't display hidden system files whereas ls -a can.

**11.** **(.venv) was added at the start** of the prompt.

**12.** The paths are **different**. This means that activate changed our path by putting .venv/bin at the beginning and the shell finds the virtual environment python rather than the system wide one.

**13.** The second pip list **includes packages that were not in the first list** :
- certifi
- charset-normalizer
- idna
- requests
- urllib3

**14.** python3 now points towards **/usr/bin/python3** which is our original system wide python path.

**15.** ls -h **displays files and folders in human readable form**.

**16.** Ctrl+C **stops the running operation** in python and raises Keyboard interruption but the **python itself keeps running**.

Whereas, Ctrl+D is used to **exit python itself** and can only be used if the input line is empty and python is not busy executing any other code(like an infinite loop).