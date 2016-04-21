## (Synchronize date and time with a server over SSH)[http://www.commandlinefu.com/commands/view/7636/synchronize-date-and-time-with-a-server-over-ssh]
```
date --set="$(ssh user@server date)"
```