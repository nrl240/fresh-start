# ****Customize Zsh with Oh-My-ZSH****

```
username@UserName-MacBook-Pro ~ % sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Cloning Oh My Zsh...
Cloning into '/Users/username/.oh-my-zsh'...
remote: Enumerating objects: 1141, done.
remote: Counting objects: 100% (1141/1141), done.
remote: Compressing objects: 100% (1103/1103), done.
remote: Total 1141 (delta 19), reused 1125 (delta 19), pack-reused 0
Receiving objects: 100% (1141/1141), 754.48 KiB | 1.30 MiB/s, done.
Resolving deltas: 100% (19/19), done.

Looking for an existing zsh config...
Found ~/.zshrc. Backing up to /Users/username/.zshrc.pre-oh-my-zsh
Using the Oh My Zsh template file and adding it to ~/.zshrc.

         __                                     __
  ____  / /_     ____ ___  __  __   ____  _____/ /_
 / __ \/ __ \   / __ `__ \/ / / /  /_  / / ___/ __ \
/ /_/ / / / /  / / / / / / /_/ /    / /_(__  ) / / /
\____/_/ /_/  /_/ /_/ /_/\__, /    /___/____/_/ /_/
                        /____/                       ....is now installed!


Please look over the ~/.zshrc file to select plugins, themes, and options.

p.s. Follow us on https://twitter.com/ohmyzsh

p.p.s. Get stickers, shirts, and coffee mugs at https://shop.planetargon.com/collections/oh-my-zsh

[oh-my-zsh] Insecure completion-dependent directories detected:
drwxrwxr-x  3 username  admin   96 Apr 15 18:48 /usr/local/share/zsh
drwxrwxr-x  4 username  admin  128 Apr 15 19:05 /usr/local/share/zsh/site-functions

[oh-my-zsh] For safety, we will not load completions from these directories until
[oh-my-zsh] you fix their permissions and ownership and restart zsh.
[oh-my-zsh] See the above list for directories with group or other writability.

[oh-my-zsh] To fix your permissions you can do so by disabling
[oh-my-zsh] the write permission of "group" and "others" and making sure that the
[oh-my-zsh] owner of these directories is either root or your current user.
[oh-my-zsh] The following command may help:
[oh-my-zsh]     compaudit | xargs chmod g-w,o-w

[oh-my-zsh] If the above didn't help or you want to skip the verification of
[oh-my-zsh] insecure directories you can set the variable ZSH_DISABLE_COMPFIX to
[oh-my-zsh] "true" before oh-my-zsh is sourced in your zshrc file.
```

## Look into the following:

```
Last login: Thu Apr 16 10:50:45 on ttys001
[oh-my-zsh] plugin 'zsh-syntax-highlighting' not found
[oh-my-zsh] Insecure completion-dependent directories detected:
drwxrwxr-x  3 username  admin   96 Apr 15 18:48 /usr/local/share/zsh
drwxrwxr-x  4 username  admin  128 Apr 15 19:05 /usr/local/share/zsh/site-functions

[oh-my-zsh] For safety, we will not load completions from these directories until you fix their permissions and ownership and restart zsh. See the above list for directories with group or other writability.

[oh-my-zsh] To fix your permissions you can do so by disabling the write permission of "group" and "others" and making sure that the owner of these directories is either root or your current user.
[oh-my-zsh] The following command may help:
[oh-my-zsh]     compaudit | xargs chmod g-w,o-w

[oh-my-zsh] If the above didn't help or you want to skip the verification of insecure directories you can set the variable ZSH_DISABLE_COMPFIX to "true" before oh-my-zsh is sourced in your zshrc file.

Oh My Zsh brew plugin:

  With the advent of their 1.0 release, Homebrew has decided to bundle
  the zsh completion as part of the brew installation, so we no longer
  ship it with the brew plugin; now it only has brew aliases.

  If you find that brew completion no longer works, make sure you have
  your Homebrew installation fully up to date.

  You will only see this message once.
```
