#luxe

A cross platform game engine written in haxe   
**Note** : If you are using the older haxelab url,    
use `git remote set-url git@github.com:underscorediscovery/luxe.git` to change it to the new url

To get started : 

###Setup Haxe

 Install [Haxe 3](http://haxe.org/download)

###Setup NME build tools

 run `haxelib install nme` , it should be > 4.0.2   
 run `haxelib install openfl-tools`, it should be > 1.0.2    
 run `haxelib install format`   
    
 Then, make sure your build environment is setup, this will install xcode/visual studio, etc.
 
 run `haxelib run nme setup <platform>`,  where <platform> is your current os (mac, windows, linux)
 
###Get LiME

 1) get the [lime](https://github.com/underscorediscovery/LiME) repo from git   
 2) tell haxelib where to find `lime`, by using `haxelib dev lime /path/to/lime`   
 i.e :   

 ` cd ~/mydevfolder && mkdir lime `   
 ` git clone git@github.com:underscorediscovery/LiME.git`    
 ` cd lime `   
 ` haxelib dev lime ./ `   

###Get luxe   

1) get the [luxe](https://github.com/underscorediscovery/luxe) repo from git   
2) set the haxelib dev folder for luxe, like with lime       
 i.e :
 
 ` cd ~/mydevfolder && mkdir luxe `   
 ` git clone git@github.com:underscorediscovery/luxe.git`   
 ` cd luxe `    
 ` haxelib dev luxe ./ `   
 
##Build the simplest project, using `haxelib run luxe`
    
 `cd ~/mydevfolder/luxe/samples/simplest`   
 `haxelib run luxe test mac` or `haxelib run luxe test linux` or `haxelib run luxe test windows`

Note : To use the shortcut version of `luxe`,   
you can copy the included shortcut scripts from /setup/ into the same folder as haxe :

- windows : if haxe binary is C:\dev\haxe\haxe.exe -> C:\dev\haxe\luxe.bat
- mac/unix : if haxe binary is /usr/lib/haxe/haxe -> /usr/lib/haxe/luxe 

This will be automated in an installer, in the near future.

## Troubleshooting

#### Windows
- you get a message such as "Cannot find haxelib luxe [or lime], are you sure it is installed?"
 - check `haxelib list` and see if there is a trailing slash mistake (i.e \/ is invalid). This was a minor haxelib bug.
 - 1) Start by making sure haxelib itself is up to date, To update haxelib run `haxelib selfupdate`, it will do the rest (and inform you of extra steps if required).
 - 2) Once updated, try re-adding the libs using the `haxelib dev` command as above. This should fix any \/ issues. Use `haxelib list` to check.
- By default, haxe and it's libraries will be stored in `C:\HaxeToolkit\haxe\lib\luxe` and `C:\HaxeToolkit\haxe\lib\lime`)

###That should be it!
