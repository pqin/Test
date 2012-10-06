Fork: clone repository to own account
       //e.g.
       opiette/wxsand.git > pqin/wxsand.git
Clone: copy github repository to local machine
% git clone git@github.com:pqin/wxsand.git
//add remote to original repository
% git remote add upstream git://github.com/opiette/wxsand.git
% git fetch upstream
//switch to different branch, '-b' add branch
% git checkout -b coldself
//update (new) branch with changes to master branch of opiette/wxsand.git
% git pull upstream/master

//show status/changes to any files
% git status
% git diff

//Stage: area where all changes to be committed are stored to be submitted all at once
% git add README
//Commit: submit changes
% git commit -m 'COMMIT MESSAGE GOES HERE'

//Merge
git checkout master
git merge coldself
//Delete branch
git branch -d coldself

//Push: send commit to GitHub repository
% git push origin master