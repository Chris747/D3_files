#Github Tutorial Part 2

<em>This requires that you have successfully completed the first Github exercise. Please see [Part 1](https://github.com/jiwpark00/D3_files/blob/master/GithubExercise1.md)</em>

Step 1: Now that you know how to fork an existing repository and make changes, you are going to first pull from this original repository.

Step 2: There are two changes in this repository. We have a new markdown document called GithubExercise2.md (this is what you are reading now)
as well as the fact that the first Github exercise now contains a big Github icon.

Step 3: So you will need to PULL from this repository to get the information in your repository updated. This essentially is
similar to the concept of "branches" in Git.

![Git Pull](http://code4reference.com/wp-content/uploads/2013/06/git-pull.jpg)

Basically, when you are working on your branch, changes will be made by members of your team.
Your job is to make sure that whatever you are working on stays up-to-date with the master branch.
Future tutorials will cover more on the essence of branches and updating within same Github repository, but for now,
this should at least give you an idea on understanding of what the "PULL" does.

Step 4: So open Command Line/Terminal and go to the directory in which your files for D3 are located.
First, note that if you type "git remote -v" without quotations, you should see "origin" with your Github repository link.
By default, what "git remote -v" does is to provide you with URL containing the location of your "master" branch.
Git commonly uses "origin" to denote the master branch, and this is why in tutorial 1, you did "git push origin" ["master" part
will be discussed later]. 

Step 5: To update your branch with the original branch that you forked from, you will need to tell Git that there is another branch, which commonly is called "upstream."
So, type "git remote add upstream https://github.com/jiwpark00/D3_files.git" without quotations.
Then, type "git remote -v" again - this time, you should see both "origin" and "remote" with respective URLs.

Step 6: Now you want to do PULL. PULL is actually a combination of two commands - fetch and merge.
Fetch means what it says - you fetch from the another repository or often, the master branch.
Merge means take what you fetched and combine with what you already have.
Pull is nice because it does all on one step.
So, type "git pull upstream master" --- basically what this means is, pull from the upstream repository on my master branch
You are going to get a screen show up (this is Vi or Vim) with a comment already added. Simply type ":" (colon; no quotations), then "x" (no quotations) and type Enter (keyboard, not actual word).
This should save the file and update your local repository.

Step 7: Once you have done this, you now want to do two things:
A) You want to first save this changed version to your repository (i.e. your repository). Since you just made a commit, simply type
"git push origin master" without quotations. This should do the job.
B) Now that you get the latest version, you want to show to others that you made this amazing change.
For the sake of simplicity, let's stop this exercise by making you create another change to your DOCX file ("ForkPractice.docx")
to include this progress, add it, and commit it and push it.

Step 8: Once you do these steps, you can email me.
