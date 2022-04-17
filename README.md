#  README
# (please dont)



sch notes
dont expect them to be legible




## How to use:

I make my notes using the [Obsidian note editor](https://obsidian.md/). If you don’t have it, download it (it's completely free and is also really cool) from the hyperlink to view my notes (many things wont look right if you dont)

### Windows

1) Open PowerShell by pressing Win and type “PowerShell”. Right click the program, and press ‘Run as Administrator’.
![[Pasted image 20220417183044.png]]

2) If you’re actually following this, it's likely you don’t have `git`. Type this into the PowerShell Window:
```
winget install git.git
```
Follow the instructions of the wizard that pops up. It might take a while, for me, it took 5 mins.

3) After installation is complete, close PowerShell and open it again as a normal user. Do **not** open it as admin this time. You can do this the same way by pressing Win and typing “powershell”, but left-clicking the application instead of right-clicking.
4) Type the following commands:
```
cd .\Documents\
git clone https://github.com/Serial-Comma/obsidian-notes.git
```
6) After it's done, open your Obsidian Application and press the ‘Open’ button next to “Open folder as vault”
![[Pasted image 20220417183757.png]]
7) You should be able to view and edit it like normal.


### Linux
```
sudo pacman -S git
cd Documents/
git clone https://github.com/Serial-Comma/obsidian-notes.git
```
~~if you dont use arch you might have a worse time~~

### Mac
dont use mac





## Contr