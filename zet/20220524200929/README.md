# Understanding git- Merge vs Rebase

### Repo Structure
* main branch
* dev branch

Lets say you branch off of main and create the dev branch. You do some
work and have three commits on the dev branch. You are ready to apply the
changes back to the main branch.

*Merge*</br>
When you merge the dev branch with the main branch, the three commits you
did on dev branch will show up as one commit on the main branch. Its
like you are stuffing the three commits in the dev branch into one
commit and applying it to the main branch.

*Rebase*</br>
When you rebase the dev branch to the main branch, git will apply the
three commits in order and one at a time to the main branch instead of
one big commit.

### Thoughts
I would think that rebasing would give a cleaner history of the repo
since you can see every commit in order. You would not need to go back
and look at the commits of what ever branch merged to the main. I assume
there is a time and place for each method. Ill ask around and do
more research on when you should rebase vs merge.

    #git #gitlearning
