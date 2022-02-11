# Lab Report 3

## Streamlining ssh Configuration

* My `.ssh/config file` and how I edited it.
![Image](https://github.com/tag717/cse15l-lab-reports/blob/main/images2/Screen%20Shot%202022-02-11%20at%202.19.11%20PM.png?raw=true)
    * First, go to "~/.ssh" file and create a "config" file.
    * Copy 
    ```
    Host ieng6
        HostName ieng6.ucsd.edu
        User cs15lwi22zzz (use your username)
    ```	
    * into the file.

* `ssh` command logging into my account using just the alias I chose.
![Image](https://github.com/tag717/cse15l-lab-reports/blob/main/images2/Screen%20Shot%202022-02-11%20at%202.10.26%20PM.png?raw=true)
    * Log in using command `ssh ieng6`.
* `scp` command copying a file to my account using just the alias I chose.
![Image](https://github.com/tag717/cse15l-lab-reports/blob/main/images2/Screen%20Shot%202022-02-11%20at%202.18.38%20PM.png?raw=true)

    * I made an example file and `scp` ed using the alias I made. We only replace the username part as the desired hostname.