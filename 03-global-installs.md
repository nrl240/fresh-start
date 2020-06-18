# **Global Installs**

1. **Set prefix for global installs**
    - `npm` has a configuration called `prefix`. This configuration setting tells `npm` where to install global modules.
    - In Terminal, run `npm config set prefix ~/.npm`. This is equivalent to editing your `~/.npmrc` to include the line `prefix=~/.npm`. You can make the prefix whatever you like, but it should be in a directory that your user has permissions to write to. That should be anything under your home directory, `~`.
      ```
      [USER_NAME]-MBP ~ % npm config set prefix ~/.npm
      ```
2. **Update `PATH`**
    - You also have to include modules installed here to your `PATH`. In your `.zshrc`, `.profile`, or equivalent you should also set something like `export PATH="$HOME/.npm/bin:$PATH"`. This will allow you to run globally installed modules that are located in `~/.npm/bin`.

      - If you are using zsh, run `echo 'export PATH="$HOME/.npm/bin:$PATH"' >> ~/.zshrc`.
        ```
        username@UserName-MacBook-Pro ~ % echo 'export PATH="$HOME/.npm/bin:$PATH"' >> ~/.zshrc
        ```
      - If you are using bash, run `echo 'export PATH="$HOME/.npm/bin:$PATH"' >> ~/.bashrc`.
        ```
        username@UserName-MacBook-Pro ~ % echo 'export PATH="$HOME/.npm/bin:$PATH"' >> ~/.bashrc