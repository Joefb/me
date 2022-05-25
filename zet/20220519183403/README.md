# Understanding git

## git init - git add - git commit

* git init</br>
When I git init the directory is not the repo. The directory is actually
called the **working directory**. The actual repo is stored in the .git
directory **in** the working directory. The working directory is the
workspace of the repo.

* git add</br>
When I git add, git takes a snapshot of the file or files and stores
them in the index that is located in the .git repo. The index is
temporary staging area. After I modify files and I git add them,
their updated contents is added to the index.

* git commit</br>
When I git commit, git permanently stores the contents of the index into 
the repo.

* Final thoughts</br>
When I git init, that directory is a repo. I can clone the repo, push to 
the repo, pull from the repo. Good stuff!

Resource: man gittutorial

    #git #gitlearning #gitbasics
