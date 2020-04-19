# Git Tricks

First, create a new config file somewhere with the settings you want to take effect in the sub-folders.

 Let's say it's at `~/topLevelFolder/.personal_gitconfig`

In `~/.gitconfig`, add:

```
[includeIf "gitdir:~/toplevelFolder/"]
    path = ~/topLevelFolder/.personal_gitconfig
```

Any subfolder of `~/topLevelFolder` will now include the config in `~/toplevelFolder/.personal_gitconfig` . 

Restart your terminal to take effect

###### Remove Proxy

To remove proxy in your `.personal_gitconfig`  you can do :

```
[http]
    proxy =
[https]
    proxy =
```

###### Example:

> ~/.gitconfig

```
[user]
        name = Preety Kumari
        email = preety.kumari@kodefork.com
[http "http://*.web.kodefork.com"]
        proxy =
[http "https://*.web.kodefork.com"]
        proxy =
```



> ~/toplevelFolder/.personal_gitconfig

```
[user]
        name = Preety Kumari
        email = preetykumari@mailvendor.com

[http]
    proxy =
[https]
    proxy =
```



