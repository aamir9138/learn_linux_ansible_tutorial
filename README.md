## openSSH Server

install openSSH if it is not installed on server using `sudo apt install openssh-server`. if you use vagrant it has by default installed openssh.

```
vagrant@buster:~/.ssh$ eval $(ssh-agent)
Agent pid 1680
```

```
vagrant@buster:~/.ssh$ ps aux | grep 1680
vagrant   1680  0.0  0.0   5852   472 ?        Ss   12:49   0:00 ssh-agent
vagrant   1684  0.0  0.0   4836   824 pts/0    S+   12:49   0:00 grep 1680
```

in .bashrc we can write an alias for the passphrase. nano to `.bashrc`

```
alias ssha='eval $(ssh-agent) && ssh-add'
```

below command will tell you what the alias is

```
alias ssha
```

```
which git
```

to check your public or private ssh key on the commandline use

```
cat ~/.ssh/id_ed25519.pub
```

The following command will show the git user

```
cat ~/.gitconfig
```
