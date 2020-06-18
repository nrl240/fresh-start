## **Connecting to GitHub:**

### Run the following commands in your terminal.
> **Note:** Pay close attention, as you need to make updates before running the fourth command to include your GitHub login email address.

```
➜  ~ touch ~/.gitignore_global

➜  ~ git config --global core.excludesfile ~/.gitignore_global

➜  ~ open ~/.gitignore_global

➜  ~ ssh-keygen -t rsa -b 4096 -C "email@email.com" # << PUT YOUR GITHUB LOGIN EMAIL HERE

Generating public/private rsa key pair.
Enter file in which to save the key (/Users/username/.ssh/id_rsa):
Created directory '/Users/username/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /Users/username/.ssh/id_rsa.
Your public key has been saved in /Users/username/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:[hidden_for_security_reasons]/g email@email.com
The key's randomart image is:
+---[RSA ####]----+
|       **********|
|      *********  |
|       ********* |
|        ******** |
|        ******** |
|    ***********  |
|   ***********   |
|    *******      |
|   *******       |
+----[SHA###]-----+

➜  ~ eval "$(ssh-agent -s)"
Agent pid 6567

➜  ~ ssh-add ~/.ssh/id_rsa
Enter passphrase for /Users/username/.ssh/id_rsa:
Identity added: /Users/username/.ssh/id_rsa (email@email.com)

➜  ~ pbcopy < ~/.ssh/id_rsa.pub
```
### **Go to GitHub and add.**
