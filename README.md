# Magento2 Bash Completion
One of the nicest facilities of the modern shell is the built in bash completion support. This script allows you to complete commands and options for Magento CLI bin/magento.

## Example

![Magento2 Bash Completion Screenshot](https://raw.githubusercontent.com/yvoronoy/ReadmeMedia/master/magento2-bash-completion.gif)

```
user@host:~$ bin/magento[TAB][TAB]
admin:user:create                        info:dependencies:show-modules-circular
admin:user:unlock                        info:language:list
bash:completion:generate                 info:timezone:list

...
```

```
user@host:~$ bin/magento setup:install --[TAB][TAB]
--admin-email                   --db-password
--admin-firstname               --db-prefix
--admin-lastname                --db-user
```

## Installation
New completion commands may be placed inside the directory /etc/bash_completion.d or inside /usr/local/etc/bash_completion.d/magento2-bash-completion on MacOSX.

Mac OSX
```
sudo curl -o /usr/local/etc/bash_completion.d/magento2-bash-completion https://raw.githubusercontent.com/yvoronoy/magento2-bash-completion/master/magento2-bash-completion
```


Linux
```
#Linux
sudo curl -o /etc/bash_completion.d/magento2-bash-completion https://raw.githubusercontent.com/yvoronoy/magento2-bash-completion/master/magento2-bash-completion
```

Don't forget reload shell or you can load new complition by next command: `user@host:~$ .  /etc/bash_completion.d/magento2-bash-completion`


If you don't have installed bash-completion follow these guides:
 * [How to install bash-completion in Debian](https://www.howtoforge.com/how-to-add-bash-completion-in-debian)
 * [How to install bash-completion in MacOSX](http://davidalger.com/development/bash-completion-on-os-x-with-MacOSX)
