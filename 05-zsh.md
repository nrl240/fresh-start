# **Install Zsh**

- **Note:** Starting with macOS Catalina (launched in October 2019), Macs will now use Zsh as the default login shell and interactive shell across the operating system. All newly created user accounts in macOS Catalina will use Zsh by default. Bash will still be available, but Apple is signaling that developers should start moving to Zsh on macOS Mojave or earlier in anticipation of Bash eventually going away in macOS.
  - Reference: [Apple replaces bash with zsh as the default shell in macOS Catalina](https://www.theverge.com/2019/6/4/18651872/apple-macos-catalina-zsh-bash-shell-replacement-features)

- If Zsh is ***not*** already installed, in your terminal, install it via `brew`. This will create a symlink at `/usr/local/bin/zsh`.
    - Regardless of whether you use iTerm or Terminal, you can still use Zsh; remember, a terminal is just the UI wrapper around a shell, which is the process that interprets and runs commands.
    ```
    username@UserName-MacBook-Pro ~ % brew install zsh
    ```

- In order to enable switching to this shell, we need to add its path to the system's official list. You can use a text editor, or simply input the following shell commands.
  ```
  sudo -s
  FILE="/etc/shells" # the list of system shells
  LINE="/usr/local/bin/zsh" # the path to our Zsh
  grep -q $LINE $FILE || echo $LINE >> $FILE # add the Zsh path to the list
  exit

- You now ***have*** Zsh, but you are ***not*** using Zsh. There are two methods for persistently activating Zsh: change your system default login shell, and/or change individual terminal profiles.
  - The command `chsh -s /path/to/shell` changes your login shell, which all terminal apps load by default. To use (Homebrew-installed) Zsh, run one of the two following commands:
    ```
    chsh -s /usr/local/bin/zsh
    ```
    ```
    chsh -s /bin/zsh
    ```
  - To confirm, run:
    ```
    echo $SHELL
    ```
    - The output should be `/usr/local/bin/zsh` **OR** `/bin/zsh/`.
