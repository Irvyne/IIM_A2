IIM A2 Repository
=================

Welcome to the IIM A2 Repository.

1) Installing a CLI Environment
-------------------------------

### I'm on Windows

I have to download Git for Windows on [msysgit.github.io][1]

When installing the software, I must select the second options when asked (for two times) !

Now, I must launch "Git bash" from windows applications.

![ScreenShot][101]

### I'm on Mac OSX

I run the terminal (available in Applications/Utilities/Terminal).

![ScreenShot][102]

### I'm on Linux *(I hope Debian for you !)*

I run a terminal or I use a SSH connection.

![ScreenShot][103]

2) Configuring PHP on a CLI Environment
---------------------------------------

### I'm on Windows (WAMP: Windows + Apache + MySQL + PHP)

Run the following command : `php -v`

![ScreenShot][104]

If you have an error, you must add PHP to your PATH environment !

I assume you have already installed WAMP.

You must identify the directory (absolute path) where the php version lived.

For example, on Windows with MAMP, it's like : `C:\wamp\bin\php\php5.x.x\`

Now, you have to add this directory to the PATH environment :

- Right-click on "Computer" -> then click on "Properties"

- Click on "Advanced system settings" in the left sidebar

- On the bottom right, click on the "Environment variables" button -> a new window open

- In the "System variables" section, select the "PATH" one -> click on the "Edit" button -> a new window open

- In the input "Variable value" go to the end of the line, check that a semicolon appear at the end -> and then add the php path to it (example : "...;C:\wamp\bin\php\php5.x.x\")

- Then click on "OK" and you successfully add the php executable to the System PATH

Restart your terminal (close then re-open it)

Then try again to run the following command : `php -v`

![ScreenShot][105]

It works dude !

### I'm on Mac OSX (MAMP: Mac + Apache + MySQL + PHP)

Run the following command : `php -v`

![ScreenShot][106]

If the PHP version is sufficient for you, STOP, don't touch nothing !

If not, I council you to go to [HomeBrew homepage][2] to install the latest php version in CLI

To test HomeBrew installation, hint `brew doctor` in the terminal, if an error occurred, you must fix it before continuing the nex steps !

Then, after having installed HomeBrew, open a Terminal and hint:

``` bash
brew tap homebrew/dupes
```

following by:

```bash
brew tap josegonzalez/homebrew-php
```

Then, compile PHP (for version 5.5):

```bash
brew install php55
```

### I'm on Linux *(I hope Debian for you !)*

![ScreenShot][107]

3) Configuring a CLI
--------------------



[1]:  http://msysgit.github.io/
[2]:  http://brew.sh/

[101]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-windows.png
[102]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-mac.png
[103]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-linux.png
[104]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-windows-php.png
[104]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-windows-php-works.png
[105]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-mac-php.png
[106]: https://raw.github.com/Irvyne/IIM_A2/master/Resources/img/terminal-linux-php.png