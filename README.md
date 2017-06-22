

## This place is yours to do with what you want.:+1:

![newbie](https://user-images.githubusercontent.com/28729693/27434963-6150a1f6-5752-11e7-9d7c-f4e938087e99.png)

Edit this page as you see fit, Add a folder off the main root and try to confine your fiddlings to your own areas.

*I placed 'this' private repo in MOJ GitHub as place where people can play whilst getting used to GitHub. 
Learn in a safe place without every body creating new Private repos (as its a charged thing - I think) = GjLing 21/6/2017*

##### Check out this online tutorial - gave me a good starting point.
[Nice intro on YouTube](https://www.youtube.com/watch?v=SWYqp7iY_Tc&t=658s)


This is what works for me (Gavin):
Development of Microservices using Java and Springboot framework.
Its a lot less hassle to use your own kit than using MOJ laptops which are locked down, slow and just too small (at the time of writting). and no correct tooling installed.
My own personal Mac & PC have a lot of tools installed to make my life easier - 
- Git client (https://git-scm.com/download/win). 
- GitHub Desktop Client application to play with if I want.

I suggest that you learn the command line client first I also think you should adopt the Unix for Windows, also as it makes life easier in the long run. Unix rocks - PCDOS sucks simple as.



### Check if you've got GIT installed

drop to a terminal window and type:

```
git --version
```

No? (PC user)- install the 'Git' from the above link - take the install defaults. You have 'Git'. 
But you've also got the Unix emulator 'Git Bash', a 'Born Again SHell' where you can think/type in Unix - on a PC :-)

i.e.
```
ls -l c:/data/GitHub
cd c:/data/GitHub
touch abc.txt
vi abc.txt
```
but the Bash shell can access other tools on your PC - type 
```
git --version
java -version
mvn -version
```
   
### Git going with command line
To as this remote cloud base repo to you PC/Mac. Decide where to locate the repos within your systemn. I chose ``c:/data/GitHub`` on my PC and ``~/GitHub`` on my Mac
e.g. (PC user) Drop to a terminal window and navigate to this location
```
cd c:/data/GitHub
ls -l
```
Pull this repo from hte cloud to you location
```
git clone https://github.com/ministryofjustice/laa-playpen-for-newbies.git
```
You should have tjhe newbie project and its directory(ies) on you machine which you can navigate to. Try creating your own folder, your own space to play...  and commit it to the cloud...
```
ls -l
cd laa-playpen-for-newbies
ls -l
mkdir john.doe
```
Lets as an a empty file abc.txt, navigate to your folder and create a new file

```
cd john.doe
touch abc.txt
ls -l
```
The file is present -but not added to Git hubs staging index area yet. Its only in your working area... to see this ask git for the status of the content so far...
```
git status
git add john.doe
git commit -m "Added my playpen"
git status

```
Check the GitHub to see the update. Refresh the https://github.com/ministryofjustice/laa-playpen-for-newbies to see your folder/content
No content.! What the heck!! Its because the 'commit' only happened locally.  You need to push the commited changes to the cloud (GitHub)
```
git push
```



