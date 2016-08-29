# K-State CIS 301, Fall 2016
 
This repository holds student coursework for CIS 301, Fall 2016.

## Directory and File Naming Conventions

Each homework should be contained in a directory named
``hw``*X* where *X* is the homework number.

Put the homework solution file for each problem inside the
corresponding homework directory with the following naming
conventions:

* If the file is a Logika text file, it should be named
  *Y*``.logika``, where *Y* is the problem number in the
  homework.

* If the file is a Z3 text file, it should be named
  *Z*``.smt``, where *Z* is the problem number in the
  homework.

For example, if the first problem in Homework #1 is a 
Logika truth table, then the solution file should be named
``1.logika`` and stored immediately under the ``hw1``
directory.
Another example, if the fourth problem in Homework #2 is
a Z3 query, then the solution file should be named
``4.smt`` and stored immediately under the ``hw2`` directory.

The grading script will assume the above file/directory
conventions, thus, any deviation will result in a zero point
for your specific solutions or even for a whole homework.

## Homework Workflow

Download and install Git: https://git-scm.com/downloads
(note: OS X and Linux distributions typically already have 
Git installed.)

If you are not familiar with Git and GitHub, here
are some good resources: 

* GitHub Training website: https://services.github.com/kit/
* Pro Git book: https://git-scm.com/book
* Git and GitHub for Beginners video: https://www.youtube.com/watch?v=Z9fIBT2NBGY

You don't need to learn all features of Git or GitHub because
the Git workflow for the course is simple as described below
(if you have not used Git/GitHub before, you want to work on the 
homework as soon as possible to avoid last minute submission issues).

First, clone this repository (replace ``username`` with your GitHub username):

```
git clone https://github.com/ksu-cis-301/301f16-username
```

This will create a local copy of the Git repository in a 
directory named ``301f16-username`` under the directory
where you execute the above command.

Alternatively, if you have set up your SSH key in GitHub 
(https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/):
   
```
git clone git@github.com:ksu-cis-301/301f16-username
```

If you use IntelliJ with the Logika plugin installed,
you can open the local copy of the Git repository directly
(see https://www.jetbrains.com/help/idea/2016.2/opening-reopening-and-closing-projects.html).
IntelliJ comes with a nice Git integration that you can take
advantage of (see https://www.jetbrains.com/help/idea/2016.2/using-git-integration.html).

Otherwise, using the command-line, change to the directory:

```
cd 301f16-username
```

At this point, here are the steps that you want to follow:

1. Do a Git pull:

   ``git pull``
   
   This is not necessary if you always use the same machine
   when working on the course work (as no one else will be making
   changes to the repository beside you).
   
2. Work on your homework solutions following the directory and
   file naming conventions described above (the instructor will
   announce where to find the homework description, which will
   contain more information regarding the specific homework
   problems).
   
3. Commit and push your files to GitHub (change ``descriptive message`` to
   any text that you want to help you remember what you worked 
   on):
 
   ```
   git add --all
   git commit -a -m "descriptive message"
   git push
   ```
   
   You can do Steps 2 and 3 as many times as you want 
   **before the homework deadline**.
   
4. Check that your latest push made it through online in GitHub 
   by opening ``https://github.com/ksu-cis-301/301f16-username``
   in your browser and navigate through the files that you just
   changed.
   
   You can also see your commit history at:
   
   ``https://github.com/ksu-cis-301/301f16-username/commits/master``
   
   to check whether the changes went through.
   
## Git and GitHub Questions?

If you have questions on Git or GitHub, we will be happy to help
you (contact us at help-301@santoslab.org).
However, it might be prudent to first try to find answers at
https://stackoverflow.com or https://google.com as it
is highly likely that someone else has already asked the
questions that you have in mind (and answered them thoroughly).