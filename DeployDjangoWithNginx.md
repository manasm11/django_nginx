# Setup Remote Machine
## Add user
1. ```bash
    # while as root user
    useradd -m -s /bin/bash -G sudo manas
    # -m is to create a home directory
    # -s to provide default shell
    # -G is to provide groups

    # To add password
    passwd manas
    ```
2. You can check user added and shell in file: `/etc/passwd`.
To check group, type `groups manas` in terminal.
3. Login into new user created.
You may want to change hostname (username@hostname:cwd_path> )
    1. Using `sudo hostnamectl set-hostname newhostname` 
    OR
    2. Changing text in file `/etc/hostname`

## Setup SSH Keys
1. 