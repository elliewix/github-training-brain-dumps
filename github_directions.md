# Getting started with GitHub

## What is GitHub?

Those of you choosing to do a programming project for your final will need to use GitHub to store and track your code.  This is a required and graded element of your project.

GitHub is a website that allows people to host programming projects online, with extra features to support users with collaboration and project organization.  There are a huge number of features and tools you can use in GitHub, but everyone needs to start with the same basic skills:

* Make a repository
* Get that repository onto your local machine
* Upload changes to your GitHub repository

You may be thinking that GitHub is something like a cloud storage service.  That isn't incorrect, but a very incomplete picture of what it can do.  Where GitHub differs between simple file storage is its version control capabilities.

## What is version control?

You a likely used to editing files in programs such as Word.  You add and change content in your file, saving as you go.  Every time you save you are writing over your previous file.  You can use the Undo function to back away from undesired changes.  This works pretty well most of the time.  However, having a queue of your 10 most recent changes may not be sufficient.  When it comes to writing code, there are very specialized needs that go well beyond the normal undo functions.  This isn't meant to be a lesson on version control, so we'll gloss over a lot of this.

There isn't a one size fits all way of using version control, so don't look at these tools as dictating your workflow.  The goal is to fit them into your natual workflow, and you'll find youself using more features as the need arises and you become more comfortable.

At a mimimum, version control for programming means that you can:

* create checkpoints for your code, representing milestones such as a completed feature or the end of you work day.
* view the differences between these checkpoints
* roll back to a previous version of a file
* restore a deleted file

GitHub uses the git version control system and has added specialized tools on top of it.  

## Getting started with GitHub

Now that you know a little about what this is about, we can start stepping through the process.

### Create a GitHub account

Your first step will be to make a [GitHub account](https://github.com/).

Activity:  create account, about 5 minutes

### Optional:  sign up for a GitHub student developer pack

You can submit your request here: [https://education.github.com/pack/join](https://education.github.com/pack/join). There are various discounts, including free private repositories, available for students and academics. 

## Create a repository

You now have a GitHub account, and your account can have multiple repositories.  You should think of a repository as being a single project.  You can host files and folders in each repository.  Again, there's no hard rule on the boundaries for a repository, and you'll understand them better as you use more features of the platform.

Think of it this way:  this repository will turn into a directory on your computer.  You can store othe folders inside of it, but everything in there will travel together.  Again, this will make more sense once you see things in action.

Step through this process together as a class.

1. Log back into [GitHub](https://github.com/) if you need to
2. On the upper right hand corner of the page you'll see a + (plus) icon.  Click that + and select "New repository"
3. This will take you to a form where you'll add some information about your repository.
4. You'll need to add the following things:
	1. Repository name: your repository name should be something short but descriptive. You might want to name yours `rr-workshop-test-repo`.  Do not include any spaces in your repository name.
	2. Description:  a sentence or two about what your repository will contain.  You might say "My test repository for the Reproducible Research workshop."
	3. Decide if you want to make your repository public or private.  You should be able to leave it as public for this workshop, but you can choose Private to make it viewable only to you and others that you invite.  Private repositories are part of a paid account, but are free (at the time of writing) with the student developer pack.
	4. Add a check next to "Initialize this repository with a README"
5. Click "Create repository" at the bottom of the page.


## What a repository page looks like

You should now see your repository's main page.  The two sections of this page that you should look at are the file section and your readme.

The file section is where you see the `README.md` file that you just made.  This can be hard to distinguish this section against others with only one file, but we'll be adding more.

The very last chunk of the page is the rendered contents of your readme file. This file is written in Markdown, which is a style of easily marking up text for web display.  We'll talk more about it when we start editing things.  The contents that were automatically added when you created the repository were the repository name and your description.  

## Editing your readme file

Any file with the name `README.md` (md is the extention for markdown files) will automatically be rendered and displayed at the bottom of your repository page.  We're going to pracice making some edits to it directly within the website.

Back in the file section, click on the `README.md` link.  This should take you to a new page where you again see the rendered contents of this file.  On the upper right side of this area (not the page) you'll see several buttons (do a page search for History to get to the right place) and several icons next to those buttons.  The pencil icon is the one that we want, hover over the icon and you should see that it says "Edit this file".  Go ahead and click that button now.

The screen will change to show the raw text behind the page (remember that we were seeing the rendered version), but you can also edit it!  Your text will look something like:

```
# jupyter-rr-demo-repo
Demo repo for writing github directions
```

The name of your repository is what will appear after the `#` and the description text will appear just below it.

Let's add some additional text to the end.

```
# jupyter-rr-demo-repo
Demo repo for writing github directions

I will be adding more to this repository as we learn about more features.
```

Once you're happy with your edits, scroll to the bottom of this page to see the Commit changes section. You can think of this like saving our changes to the file, but remember that in GitHub everything you do will have a bit of metadata lagniappe (a bit extra) along with it.  So we aren't just saving our file here, we're saving it along with a message about what we did.

Here you are offered two text fields.  The text box with one line you see just below "Commit changes" is the required commit message.  Version control isn't just about being able to track the changes made to a file, so this is where we can write a message about what this change is.  This message will be public and is meant to help you understand the context of the changes that you made.  The length is limited, so keep it to about 140 characters or less.  

Type in a commit message now:  "adding more information about this repository"

The larger text box just below is optional, and you can provide longer information about what's going on with your changes.  We'll leave this one empty.

Now we're ready to commit our changes!  We're going to use the default mode of `Commit directly to the master branch.`.  Now we're going to commit our changes with our new commit message. Click the big "Commit changes" button.

Once the page reloads, you'll see the new version of your readme file rendered with your additional text!

## Cloning the repo to your local machine

Again, everything with GitHub involved mostly normal things you'd do but with extra stuff and a different name.  Cloning means that you are downloading the repository to your computer, but keeping git aware of the files.  You aren's just downloading and unzipping a folder (which you can do), but downloading it in such a way that git will be watching the changes that you make to the files.

### Use a GitHub client of choice

There are two ways that you can interact with your GitHub repository:

1. On the website, which you've already done.  This is great for quick edits to plain text files, but doesn't allow you to execute any code, for example.
2. On your local machine. Where you have copies of your files that you edit, and then you publish your edits up to GitHub.  This will be the bulk of how you do your edits.

When working on your local copies, the website version of the files will remain the same until you push your changes.  Pushing changes is sort of like uploading your copies, but you're also sending along your commit messages and other metadata.  Again with that theme of "something normal with a bit extra."

As you might expect, you can't just download files to your machine like normal to have all the extra git things.  You need to use an application of some sort to handle the monitoring of local file changes and communication with GitHub.  There are several of these applications available, but two main free options:  the command line or a GUI application.  You can actually use both, so there's no pressure in choosing the one right thing at the start.  You may find that you prefer one but occasionally need the features of the other.  

Here are some examples of that:

* You are happy to work in the command line for the core tasks of committing and pushing, but find it easier to use the GUI application to review history, file differences, and roll back or restore previous versions.  The adrenaline rush of accidentally deleting all your project files can make it hard to focus and remember all the commands and steps for restoring them, and the GUI application can avoid some confusion.
* You prefer to use the GUI application for all your normal activity and this works just fine for most of your projects.  Occasionally you'll have a project that doesn't work well with the application (example: constantly making several hundred thousand files or more), and committing & pushing on the command line works better.

You'll find your own comfort space, and there's nothing wrong with using either method.  Again, focus first on what you can incorporate into your natural workflow, and then add complexity if the need arises.  This lesson will describe the process of installing and using GitHub desktop, but other Carpentries lessons will have directions for command line git.

### Install GitHub Desktop

This is a free application that is made by GitHub.  You can download it here:  [https://desktop.github.com/](https://desktop.github.com/).  

Once you download it, open the installer and follow all the normal installation methods.  Mac users, you'll need to drag the application to your Applications folder, and Windows users you should be able to follow all the exe direction.

After installing, go ahead and open it.  There are some major differences between the Windows and Mac versions, so there will be notes about each as we go along.  The biggest difference will be where you access menu items.  Mac users will have them at the top of the screen as normal.  Windows users will have a gear on the upper right of the screen.  There will also be differences in what things are called, e.g. Finder vs Explorer.

### Connect you account

Upon first opening it, Windows versions will go ahead and prompt you to log it.  

Unsure if macs do.

TODO:  this needs to be tested on a fresh install,

Directions for logging in from the regular GUI:

* Windows: click the gear on the upper right, Select Options.  Click on "+ Add an account"
* Mac:  in the upper menu items, click on GitHub Desktop and select Preferences.  Click on the accounts tab if it isn't already selected.
* Choose the sign in option for to the GitHub.com option.
* Log in with your user name and password

### Do the cloning

From here, it will look pretty empty because you haven't added any repositories.  The good news is that we're finally ready to clone your repository!  Go back to your repository's website.  

You may have closed that website at this point, so we can practice how to find it from your github page.  Go to [GitHub.com](https://www.github.com/) and ensure that you are logged in.  Look on the right side of the page and you'll see a little pod called "Your repositories". You should see the name of your new repository in there.  Click on it and you'll be back.

At the main repository page, on the right you'll see a big green button that says "Clone or download".  Click that, and then "Open in Desktop".  Your operating system may ask to confirm that you want to open an application ("External protocol request" for windows and "Open it GitHub Desktop" for mac).  This will open up an info box in GitHub desktop.  You will want to review these options, so wait before clicking Clone!

The Repository URL will be be filled out for you, and you shouldn't change that. 

The Local Path will also be filled out for you.  By default, it will have a folder in your Documents directory called GitHub.  You can select a different folder if you want. 

Once you're happy with the local path that the repository will be saved in, you can click Clone.  We can confirm that our previous work on the website has been included by looking at the history.  On macs, the left panel will have two tabs for Changes and History.  On Windows these appear roughly in the middle of the window.  

Right now the Changes tab is empty because what we have locally matches exactly with what is on the website version.  Click on the History tab and you'll see two commits:  one for the initial commit where the readme file was created automatically at creation of the repository, and another where we added more info to our readme file.  You can click into those two commits to see the differences between the two files.

## Find the local copies

The interface is now a bit more interesting because you have a repository.  On the left side of the GitHub Desktop window it should say something like "Current Repository".  Clicking on that will toggle another window where it lists out all the git repositiories that it knows about.  It doens't go searching for local repositories on your computer, but you can have it managining multiple repositories.  

If you can't find this window, you can go up to View and select Show Repositories List.

Right now you may only see the one we just cloned, `jupyter-rr-demo-repo`.  Click on the name to go into that repository's view.

You can always use normal file navigation to find the folder that was just made, but there's a nice selection of shortcuts within the application.  THese are in different spots depending on your OS.

* Mac:  with on the upper menu, click Repository and select Show in Finder.
* Windows:  click the gear (upper right) and select Show in Explorer.

This will take you directly to your local folder for this repository.

## Make a Jupyter Notebook in your directory

We're now going to launch a Jupyter Notebook instance and save a notebook in this directory.  

This folder is another directory on your computer, so if you're already comfortable with changing directories in your command line, you can do so.  However, we can also use another shortcut of the application.

Navigate back to the Repositories menu where we just were (Repositories at the top or the gear icon at the left).  This time, select Open in Finder for Macs or Open in Git Shell for windows.

This will open up a shell prompt already inside this directory.  Type in `jupyter notebook` to launch the service in that directiory.  (NOTE: this is presuming you have a standard installation.  You should follow your normal start routine here if you have something that differs.  

TODO: does this work on windows? some screen shots I see show Open in Git Shell, so does jupyter notebook work here?

Once the Jupyter host has started up, launch a Python 3 notebook as normal.  Name this file (by clicking on the "Untitled" at the top) "demo".

Pop back into your GitHub desktop and you should see a bunch of green code in the code window, and some new files.  You can tell that these are new files because there is a big green + sign next to them.

Take a moment to look at the file preview in comparison to how the rendered Jupyter Notebook looks like.  Remember that, like Markdown, Jupyter Notebooks are plain text JSON files that tell the sevice how to render them.  So when you look at the raw contents, it can be very hard to tell what's going on.  Markdown is a bit more readable (and is why most of us write directly inside of Markdown) but Jupyter Notebooks aren't disigned to have pretty 'human readable' code inside.

### Commit the empty file

Let's commit this empty version of the file to our local repository.  Our changes are being saved to our `ipynb` files as we edit them, but this will check in this change to our repository information.  

Go into GitHub Desktop and in the Changes panel you'll see two text boxes like you saw in the website version.  The first short one is your required commit message and the longer second one is the optional description area.  Add a commit message like "Adding empty jupyter notebook" and click "commit to master".

You can now click back into the History tab and see your commit there.

### Commit changes to that file

We're now going to add some content and commit that in.

Activity:

Take 5 minutes and write some silly Python code in your Jupyter Notebook.  Add some Markdown cells explaining what that silly code does.

Example:

(markdown cell)  This makes the worst traffic light results.

```python
import random
```


```python
colors = ['red', 'green', 'yellow']

def traffic_light():
    return random.choice(colors)

for i in range(10):
    print("The light is", traffic_light())
```

    The light is red
    The light is yellow
    The light is red
    The light is yellow
    The light is red
    The light is green
    The light is green
    The light is red
    The light is green
    The light is yellow

Now go back to GitHub desktop.  Click back into the Changes tab if you need.  Once again you'll see your demo.ipynb is in there, but instead of a greed + you can see an orange/yellow dot icon.  This indicates that you have a file change.  
