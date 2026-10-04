# copyingRepos
Documentation on Copying Repositories (Harder than you might think) and deleting commits.    
MJS 10.4.26    
    
==================================   
GOAL: It is desired to produce new repos, such as bootcamp homework repos, with the  
original set-up. In other words the original files from the bootcamp are 
"loaded", but no changes have been made to them.  
============================================   
CANT: One cannot fork one's own repo into the user's account !!  

CAN: (A) Fork repo into organizational account.  
CAN: (B) Likely can clone repo to local machine, change name of remote and upload all files.   

==========================================================   
CANT: It is just not possible to create a fork of a repo in the same account as the original repo.  

CAN: (A) Fork repo into an organizational account.    
Step 1: Create an organization (if not already created).  
   Step 1A: Open user navigation menu (top right).   
   Step 1B: Click Organizations   
   Step 1C: Click New Organization (near top right).   
Step 2: Unlink the forked organizational repo.   
   Or else it will always tell you the fork is out of synch with the parent repo.   
   And commits in only the fork likely wont count.   
   Step 2A: Click settings (gear icon).   
   Step 2B: Click General.  
   Step 2C: Find the "Danger Zone" box near the bottom.   
   Step 2D: Unlink the forked repo, using the button.   
   Step 2E: Wait (up to 15 minutes).   
Step 3: Deleting Commits from the unlinked forked organizational repo.   
   Step 3A:  Clone the unlinked forked organizational repo. (Copy name, then git clone <paste>).   
   Step 3B:  Find and copy the "SHA" name of the last commit you wish to keep in Github.     
   Step 3C:  Delete commits from cloned repo using "git reset --hard <commit SHA>" (which deletes commits from local clone).  
   Step 3D:  Delete commits from the Github organizational repo using "git push origin main --force"   
   Note:  You may also "revert" to a prior commit, but with all old commits retained.  


CAN: (B) Likely can clone repo to local machine, change name of remote repo and upload all files (git add --all, git commit).     
   This likely will NOT keep all commits.  

   
