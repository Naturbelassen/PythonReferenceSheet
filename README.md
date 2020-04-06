# Python Reference Sheet

Sheet for python and its methods/functions

## list(*string*) - Takes a String as the argument and converts it into a list:  
myString = ("Python")  
myList = list(myString)  
print(myList)  
Output: ['P', 'y', 't', 'h', 'o', 'n']  

## *string*.append - Adds to the end of the List   
myList.append('T')  
print(myList)  
Output: ['P', 'y', 't', 'h', 'o', 'n', 'T']  

## '*seperator*'.join(*Dictionary/List*) - Connect all items in a Tuple into a String:  
myList = '+'.join(myList)  
print(myList)  
Output: P+y+t+h+o+n+T  

## for *iterator* in *List* - Traverses a String/Dictionary/List item by item:  
yourString = ("World")  
for i in yourString:  
	print(i)  
Output:  
W  
o  
r  
l  
d













## Misc  


Bind your Private Key to GitHub to use SSH when remote:  

1. Create new Repository
2. Choose a Name for your Repository
	Optional:
	- Descriptopn: Describe your Project
	- Choose Public or Private
	- Initialize this repository with a README (Don't select this one, we will create it ourselves)
	- Add .gitignore: Choose this if you don't want to push all of your files in your working directory. To do so you need to edit this file later e.g. input .txt -> save -> close, will ignore all .txt files when upload to github.com. Should be in the directory you're working with.
	- Add a license: Click the (i)-button to get further information
3. Create repository
4. Select SSH
	- Create a Directory and head into it. On Windows: Create a Directory, head into it, right click and choose "Git Bash Here" (When not installed downlaod: [https://gitforwindows.org/](https://gitforwindows.org/)
	- echo "# Project Details" >> README.md: Creates a .md (Markdown file) that will showcase how to work with your Application/Software
	- git init: Will initialize your Directory (Only your Directory in which you are right now) which means GitHub will keep track with changes regarding your files
	- Optional: git status -> You'll get a complain that README.md isn't added yet 
	- git add README.md: Will add your file
	- git remote add origin gitgithub.com:*YourUsername*/*YourProjectName*.git
5. [Generating a new SSH key and adding it to the ssh-agent](https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
	- Optional: User eval `ssh-agent` to ensure your ssh-agent is running in the Background
	- ssh-add *Path to your PrivateKey*
6. git push origin master: will upload all files that are not in .gitignore to your account on github.com
	