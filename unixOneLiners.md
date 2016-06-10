## [Synchronize date and time with a server over SSH](http://www.commandlinefu.com/commands/view/7636/synchronize-date-and-time-with-a-server-over-ssh)
```bash
date --set="$(ssh user@server date)"
```

## (Copy your ssh public key to a server from a machine that doesn't have ssh-copy-id)[http://www.commandlinefu.com/commands/view/188/copy-your-ssh-public-key-to-a-server-from-a-machine-that-doesnt-have-ssh-copy-id]
```bash
cat ~/.ssh/id_rsa.pub | ssh user@machine "mkdir ~/.ssh; cat >> ~/.ssh/authorized_keys"
```

## (Copy files and change ownership at the sametime)[http://unix.stackexchange.com/questions/124855/move-files-and-change-ownership-at-the-sametime]
```bash
 rsync -r --chown=user:group srcDir/ destDir/
 ```