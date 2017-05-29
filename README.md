# git ignore
Extend git command and add .gitignore templates more quickly into your new projects. All templates are downloaded from [github.com/github/gitignore](https://github.com/github/gitignore).

## Usage examples
1) List all available templates

```bash
$ git ignore --list
Actionscript.gitignore         
Ada.gitignore                  
Agda.gitignore                 
Android.gitignore              
AppEngine.gitignore            
AppceleratorTitanium.gitignore 
...                 
```

2) Download specific template to active directory

```bash
$ git ignore VisualStudio
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  4839  100  4839    0     0  18191      0 --:--:-- --:--:-- --:--:-- 18191
Done.           
```


## Installation
### Unix / MacOS
Download `git-ignore` file and put it inside `/usr/local/bin`. [What is /usr/local/bin?](https://unix.stackexchange.com/questions/4186/what-is-usr-local-bin)

_I haven't tried this on Unix / MacOS yet._

### Windows
Download `git-ignore` file and put it inside any directory that is added to the PATH.

To find out what are those directories go to  `Control Panel → All Control Panel Items → System → Advanced system settings (in sidemenu)→ Advanced (tab) → Environment Variables... → User variables for <username>`. There should be variable called `PATH`. To view folders or to add your own select PATH variable and click `Edit...`. I prefer to add utilities at `C://Users/<username>/AppData/Roaming/Utilities`.


## Dependencies
To use `$ git ignore --list` make sure `jq` is installed. jq is a lightweight and flexible command-line JSON processor. For more info visit: [stedolan.github.io/jq](https://stedolan.github.io/jq/)

_Note:_ On Windows you can download latest jq .exe file and put it in directory that is added to the PATH.


## Further enhancements
* Currently `git ignore --list` actually lists all files from [github.com/github/gitignore](https://github.com/github/gitignore/) and not all of them are .gitignore's.

## Few resources
* [mfranc.com/tools/git-custom-command](http://mfranc.com/tools/git-custom-command/)
* [adamcod.es/2013/07/12/how-to-create-git-plugin.html](https://adamcod.es/2013/07/12/how-to-create-git-plugin.html)
* [coderwall.com/p/bt93ia/extend-git-with-custom-commands](https://coderwall.com/p/bt93ia/extend-git-with-custom-commands)
