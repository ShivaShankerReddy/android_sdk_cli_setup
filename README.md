# ANDROID SDK CLI SETUP
--------------------------

## ARCH LINUX:
---------------

[android_sdk_link] - android sdk git link.

## Installation Steps:
-----------------------

1) git clone https://aur.archlinux.org/android-sdk.git
2) cd android_sdk_link
3) sudo makepkg -sfi


## ANDROID SDK in SYS PATH:
------------------------------

1) Open `.bashrc` file if you are bash shell else `.zshrc` file.

    1) if you wanna check which shell is default in your pc. Type `$SHELL` in
    terminal.

2) copy and paste these lines in your `.rc` files sequentially.

    ```
    export PATH=${ANDROID_HOME}/emulator:${PATH}
    export PATH=${ANDROID_HOME}/tools:${PATH}
    export PATH=${ANDROID_HOME}/tools/bin:${PATH}
    export PATH=${ANDROID_HOME}/platform-tools:${PATH}

    ```

3) `source (.bashrc|.zshrc)` to replicate the changes.


## Changing ownership of android sdk folder:
---------------------------------------------

1) `sudo chown -R {whoami} $ANDROID_HOME` : to change the ownership of android
sdk folder to login user to install and make changes based on project
requirement.


[android_sdk_link]: https://aur.archlinux.org/android-sdk.git

