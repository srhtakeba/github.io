# Personal Website Hack Day 2019! 🎉

Ever wanted to build your own website? With NUWIT, you'll learn how—and more!
## Table of Contents
- [ Getting Started ](#getting-started)
  - [ Wireframing](#wireframing)
  - [ Code Editors](#code-editors)
  - [ Installing Git](#installing-git)
  - [ Using Git and Github](#using-git)
  
- [Bare Bones HTML](#bare-bones)
  - [ Edit HTML](#edit-html)
  - [ Commit Changes to Git and Github](#commit-changes)
  - [ HTML Tags and Attributes](#html-tags)
  - [ CSS](#css)
  - [ CSS and HTML Together](#css-html)
  - [ Developer Tools](#developer-tools)
  
- [ Bootstrap ](#bootstrap)
- [ Advanced Bootstrap ](#advanced-bootstrap)
  - [Responsive Breakpoints](#responsive-break)
  - [Grid](#grid)
  - [Flex](#flex)
- [Google Fonts](#google-fonts)
- [FontAwesome](#font-awesome)
- [Wrap-Up](#wrap-up)

<a name="getting-started"></a>
## Getting Started
<a name="wireframing"></a>
### Wireframing
- **[Figma](https://www.figma.com/)**: A wireframing application that can help you plan out your website! 
<a name="code-editors"></a>
### Code Editors
Here is a great **open source** code editor that is compatible with Windows, Mac, and Linux:
- **[Visual Studio Code](https://code.visualstudio.com/download)**: Microsoft's code editor with a super sleek user interface and terminal integration.  

There are lots of other code editors out there if you'd prefer something different, but this is the code editor we'll be using during our demos. 
<a name="installing-git"></a>
### Installing Git
Git is a **version control** system. It, like our code editors, is open source. Essentially, git allows us to make changes to code, revert code to a past version, and add features to code without necessarily having those features part of our final product.

- **[For Mac](http://git-scm.com/download/mac)**
- **[For Windows](https://gitforwindows.org/)**
- **[For Linux](https://git-scm.com/download/linux)**

<a name="using-git"></a>
### Using Git and Github ###

[Create a github account.](https://github.com/join)

Fork this repository using the link below the topbar:
![How to fork a repository](https://help.github.com/assets/images/help/repository/fork_button.jpg)

**Copy** your new repo's clone url:

![Clone button](https://help.github.com/assets/images/help/repository/clone-repo-clone-url-button.png)

![Url to clone](https://help.github.com/assets/images/help/repository/https-url-clone.png)

Open your terminal in your code editor:
- Use the `` ⌃` `` keyboard shortcut with the backtick character.
- Use the `View > Terminal` menu command on windows, and the `Terminal > New Terminal` menu command on Mac. 
- From the Command Palette (`⇧⌘P`)

**Type** the following command into your terminal, **pasting** the git clone url you just copied:

```$ git clone [COPIED GIT CLONE URL]```

and press enter...

You should now have this repo on your machine!
<a name="bare-bones"></a>
## Bare Bones HTML 
<a name="edit-html"></a>
### Edit some HTML
In your editor, open the `hack_day_2019/bare_bones` folder. 

You'll notice that there are two files in this folder: `index.html` and `style.css`

On line of 7 of index.html, replace:

``` <title>My Website</title>```

with 

```<title>[YOUR NAME HERE]</title>```
 
And on line 9, replace:

``` <meta name="author" content="Your Name">```

with 

``` <meta name="author" content="[YOUR NAME HERE]">```

You can also add a description to your site on line 8, in the `content` attribute.  

Save these changes. 
<a name="commit-changes"></a>
### Commit Changes to Git and Github

To stage your changes to be committed, type:

`$ git add .`

Then type the following command to commit the changes to your **local repository**. Your local repository is the git repository that is tracking the changes on your laptop only. Your **remote repository** is your Github repository, the one that saves all your changes online.

`$ git commit -m "Add my name"`

The quotation following `-m` is the commit message, which gives a description of what changes were made in that commit. 

Once the changes are committed, let's push them to your Github repo. 

`$ git push -u origin`

You should now see the changes on your Github repo. 

You can use those three commands to save your work throughout your coding process. 

<a name="html-tags"></a>
### HTML Tags and Attributes
Here, we're going to give you an overview of HTML and show you some demos. But in case you need resources, we've listed quite a few below: 

- **[HTML Overview](https://www.w3schools.com/html/html_intro.asp)**
- **🌟[Cheat Sheet](http://www.simplehtmlguide.com/cheatsheet.php)🌟**
- **[In Depth Tutorial](http://www.tutorialspoint.com/html/html_quick_guide.htm)**

<a name="css"></a>
### CSS
Once again, CSS will require a bit of in-person explanation. But here are resources just in case:

- **[CSS Syntax Intro](https://www.w3schools.com/css/css_syntax.asp)**
- **🌟[Cheat Sheet](https://www.toptal.com/css/css-cheat-sheet)🌟**

<a name="css-html"></a>
### CSS & HTML - Put it all together!
Getting a bit lost putting it all together? Here's some example code!

- **[Topbar Reference](https://www.w3schools.com/css/css_navbar.asp)**

Don't forget to commit your changes!

<a name="developer-tools"></a>
### Developer Tools

Sometimes figuring out the correct CSS is a lot of trial and error. There are a lot of different CSS attributes, and it's hard to memorize them all, let alone everything they do. Google Chrome's Developer Tools can help you.

Developer Tools allows you to see immediate changes to a website as you toggle CSS attributes and edit HTML. Note that these changes won't actually be made to your code — they'll just temporarily manipulate the website as it appears in your browser. But it's still a good way to experiment and identify problems in your HTML or CSS. 

If you'd like to test out a new look for Wikipedia's logo, for example, you can add the yellow background:
![Alt text](/../screenshots/screenshots/devtools2.png)

And then toggle it off again:

![Alt text](/../screenshots/screenshots/devtools1.png)

You can open the Developer Tools by right clicking on some component of a website and selecting "Inspect: 
![Open Developer Tools with right click](https://developers.google.com/web/tools/chrome-devtools/images/inspect.png)

Or through the Chrome menu:
![Open Developer Tools through Chrome Menu](https://developers.google.com/web/tools/chrome-devtools/images/open-from-main.png)

Need more help with Developer Tools? Check out these Google tutorials:

- **[Developer Tools and HTML for Beginners](https://developers.google.com/web/tools/chrome-devtools/beginners/html)**
- **[Developer Tools and CSS for Beginners](https://developers.google.com/web/tools/chrome-devtools/beginners/css)**

<a name="bootstrap"></a>
## Bootstrap 
Open the `hack_day_2019/bootstrap` folder and open `index.html`. 

Your `index.html` is already set up with Bootstrap installed. 

Trying to figure out Bootstrap? Here are some important pages in the documentation: 
- **[Layout](https://getbootstrap.com/docs/4.1/layout/overview/)**
- **[How Bootstrap Formats HTML tags](https://getbootstrap.com/docs/4.1/content/reboot/)**
- **[Copy and Paste Components](https://getbootstrap.com/docs/4.1/components/)**
- **[Bootstrap Demos](https://getbootstrap.com/docs/4.1/examples/)**
<a name="advanced-bootstrap"></a>
## Advanced Bootstrap Utilities
<a name="responsive-break"></a>
### Responsive Breakpoints
**Breakpoints** are common device widths at which we should change our layout to optimize readability and usability. For example, while a set of links can span horizontally across a laptop screen, those links should stack vertically on a phone. Otherwise some text could get cut off. 

Here are Bootstrap's breakpoints. 
```
// Extra small devices (portrait phones, less than 576px)
// No media query for `xs` since this is the default in Bootstrap

// sm - Small devices (landscape phones, 576px and up)  
@media (min-width: 576px) { ... }

// md - Medium devices (tablets, 768px and up)
@media (min-width: 768px) { ... }

// lg - Large devices (desktops, 992px and up)
@media (min-width: 992px) { ... }

// xl - Extra large devices (large desktops, 1200px and up)
@media (min-width: 1200px) { ... }
```

You can set certain (but not all) Bootstrap utilities to activate at certain breakpoints. To do this, use the following syntax in your class names:

```[Bootstrap attribute]-[breakpoint abbreviation]-[Bootstrap value]```

For example:

```text-left text-md-center```

Using the above class names, your text will be left-aligned on all screens with widths smaller than 768px, but centered on all screens above that. 

Your default styling, aka the styling that applies to extra small (xs) screens, should have no breakpoint. In this case `text-left`. For greater screen sizes that require different styling, add the appropriate breakpoints. The styling you provide for a breakpoint will apply for all screen sizes greater than that breakpoint — until/unless it reaches a greater breakpoint where you've different styling. 

You can change styling at every breakpoint, if you want. For example:

``text-left text-sm-center text-md-right text-lg-justify text-xl-right``

In this example, extra small screens will have left-aligned text, small screens will have center-aligned text, medium screens will have right-aligned text, large screens will have justified text, and extra large screens will have right-aligned text. 
<a name="grid"></a>
### Grid 
         
<a name="flex"></a>
### Flex
         
<a name="font-awesome"></a>
## FontAwesome ##

Want fun icons like these on your website? 
![Font Awesome Icons](https://i0.wp.com/blogs.innovationm.com/wp-content/uploads/2017/10/fontawesome-text-icons-0041-jpg.jpeg?w=625)

To use icons in your HTML, add the following code before `</head>`:

```<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.7.2/css/all.css" integrity="sha384-fnmOCqbTlWIlj8LyTjo7mOUStjsKC4pOpQbqyi7RrhN7udi9RwhKkMHpvLbHG9Sr" crossorigin="anonymous">```

Then, check out this [list of FontAwesome icons](https://fontawesome.com/icons?d=gallery). Take note of the names of icons you want to use.

To use an icon, add an `<i></i>` tag with the following class names:

```<i class="fas fa-[ICON NAME]></i>```

To insert a star, for example:

```<i class="fas fa-star></i>```

<a name="google-fonts"></a>
## Google Fonts

Tired of boring web safe fonts like Helvetica and Times New Roman? Well, you're in luck! Google Fonts has a wide selection of fonts that you can embed on your webpage. 

- **[Google Font List](https://fonts.google.com/)**

Once you pick a font, take note of its name. Then add the following code before `</head>`:

```<link href="https://fonts.googleapis.com/css?family=[FONT NAME]" rel="stylesheet">```

For example, 

```<link href="https://fonts.googleapis.com/css?family=Roboto" rel="stylesheet">```

And if you want to add only specific weights:

```<link href="https://fonts.googleapis.com/css?family=Roboto:400,500,700" rel="stylesheet">```

Each font will have different weights, or sometimes, only one weight. Check which weights are available for your chosen font

<a name="wrap-up></a>
## Wrap-Up 
Feel free to delete the starter files. Make sure your final `index.html` is at the root of your directory. 

Now let's push your finished website to your personal Github page.

Create a **NEW** Github repository.  **DO NOT INITIALIZE THE REPO WITH A README** and make sure to give it a name in the following format:

``[YOUR GITHUB USERNAME].github.io``

For example: ``username.github.io``

In your terminal, type the following command:

``$ git remote add website https://github.com/[YOUR GITHUB USERNAME]/[YOUR GITHUB USERNAME].github.io``

...where ``website`` is the name of your new remote repository. 

Check that your new remote repository exists:

``$ git remote -v``

Finally, push your finished website to Github pages:

`$ git push website master`

That's it! Check out ``[YOUR GITHUB USERNAME].github.io`` for your published website! It might take some time to show up, but it should be there within an hour or so. 

