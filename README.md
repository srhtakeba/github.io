# Personal Website Hack Day 2019! 🎉

Ever wanted to build your own website? With NUWIT, you'll learn how—and more!

## Getting Started
### Wireframing
- **[Figma](https://www.figma.com/)**: A wireframing application that can help you plan out your website! 
### Code Editors
Here are some great **open source** code editors that are compatible with Windows, Mac, and Linux:
- **[Visual Studio Code](https://code.visualstudio.com/download)**: Microsoft's code editor with a super sleek user interface and terminal integration. 
- **[Atom](https://atom.io/)**: Github's code editor, also with a sleek UI and terminal integration! 

There are lots of other code editors out there if you'd prefer something different, but these two are highly recommended and completely free!

### Installing Git
Git is a **version control** system. It, like our code editors, is open source. Essentially, git allows us to make changes to code, revert code to a past version, and add features to code without necessarily having those features part of our final product.

- **[For Mac](http://git-scm.com/download/mac)**
- **[For Windows](https://gitforwindows.org/)**
- **[For Linux](https://git-scm.com/download/linux)**

### Using Git and Github ###

[Create a github account.](https://github.com/join)

Fork this repository using the link below the topbar:
![How to fork a repository](https://help.github.com/assets/images/help/repository/fork_button.jpg)



**Copy** your new repo's cloning url:

![Clone button](https://help.github.com/assets/images/help/repository/clone-repo-clone-url-button.png)

![Url to clone](https://help.github.com/assets/images/help/repository/https-url-clone.png)

Open your terminal in your code editor:
- Use the `` ⌃` `` keyboard shortcut with the backtick character.
- Use the `View > Terminal` menu command on windows, and the `Terminal > New Terminal` menu command on Mac. 
- From the Command Palette (`⇧⌘P`)

**Type** the following command into your terminal, **pasting** the git clone url you just copied:

```git clone [COPIED GIT CLONE URL]```

and press enter...

You should now have this repo on your machine!

## Bare Bones HTML 

Using the terminal, enter the first folder using the following command: 

`cd hack_day_2019/bare_bones`

This will bring you into the first folder in this repo. 

You'll notice that there are two files in this folder: `index.html` and `style.css`

On line 7, replace:

``` <title>My Website</title>```

with 

```<title>[YOUR NAME HERE]</title>```
 
And on line 9, replace:

``` <meta name="author" content="Your Name">```

with 

``` <meta name="author" content="[YOUR NAME HERE]">```

You can also add a description to your site on line 8, in the `content` attribute.  

Save these changes. Now let's commit them to Git and Github. 

To stage your changes to be committed, type:

`git add .`

Then type the following command to commit the changes to your **local repository**. Your local repository is the git repository that is tracking the changes on your laptop only. Your **remote repository** is your Github repository, the one that saves all your changes online.

`git commit -m "Add my name"`

The quotation following `-m` is the commit message, which gives a description of what changes were made in that commit. 

Once our changes are committed, let's push them to your Github repo. 

`git push -u origin`

You should now see the changes on your github repo. 

You can use those three commands throughout your coding process to save your work. 

## Wrap-Up 
Now let's push your finished website to your personal Github page. 

