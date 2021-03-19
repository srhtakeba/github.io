# Personal Website Hack Day 2021! 🎉

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
  - [Responsive Breakpoints](#responsive-break)
  - [ CSS and HTML Together](#css-html)
  - [ Developer Tools](#developer-tools)
- [ Bootstrap ](#bootstrap)
  - [Grid](#grid)
  - [Flex](#flex)
  - [Components](#components)
- [Google Fonts](#google-fonts)
- [FontAwesome](#font-awesome)
- [Wrap-Up](#wrap-up)

<a name="getting-started"></a>
## Getting Started
<a name="wireframing"></a>
### Wireframing
- **[Figma](https://www.figma.com/)**: A wireframing application that can help you plan out your website!
- **[Wireframing 101 & Figma tutorial](https://docs.google.com/presentation/d/143D6zUYFjAOQWJH_0YTpAWVjqFztaRHC8jfzJZIEFqw/edit?usp=sharing)**
<a name="code-editors"></a>
### Code Editors
Here is a great **open source** code editor that is compatible with Windows, Mac, and Linux:
- **[Visual Studio Code](https://code.visualstudio.com/download)**: Microsoft's code editor with a super sleek user interface and terminal integration.  
- **[Live Server Extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)**: An extension that allows you to quickly see your changes to HTML/css files in the browser.

There are lots of other code editors out there if you'd prefer something different, but this is the code editor we'll be using during our demos.
<a name="installing-git"></a>
### Installing Git
Git is a **version control** system. It, like our code editors, is open source. Essentially, git allows us to make changes to code, revert code to a past version, and add features to code without necessarily having those features part of our final product.
If you're unsure if you have git installed, type `$ git` into your terminal. If the response is a list of git commands, you already have git installed!

- **[For Mac](http://git-scm.com/download/mac)**
- **[For Windows](https://www.computerhope.com/issues/ch001927.htm)**
- **[For Linux](https://git-scm.com/download/linux)**

### IMPORTANT: If you have windows, installing git might be slightly more challenging. Read the instructions above carefully and make sure to ask for help if something doesn't work!

<a name="using-git"></a>
### Using Git and Github ###

[Create a github account.](https://github.com/join)

Open your terminal in your code editor:
- Use the `` ⌃` `` keyboard shortcut with the backtick character.
- Use the `View > Terminal` menu command on windows, and the `Terminal > New Terminal` menu command on Mac.
- From the Command Palette (`⇧⌘P`)

Type the following into terminal to add a username to your Git. It can be your Github username, or just your name:

`$ git config --global user.name "[GITHUB USERNAME]"`

And also type the following into terminal to match your Git email to your Github email. **This email must match the one you associated with your Github account**:

`$ git config --global user.email "email@example.com"`

**Optional**: set up VS-Code with git
- Open VS Code, go to Command Palette (Cmd-Shift-P), and click "Shell Command: Install 'code' command in PATH"
- Type `$ git config --global core.editor=code --wait`

Return to the Github repository for Personal Website Hack Day. Fork this repository using the link below the topbar:
  ![How to fork a repository](https://help.github.com/assets/images/help/repository/fork_button.jpg)

**Copy** your new repo's clone url:

![Clone button](https://help.github.com/assets/images/help/repository/clone-repo-clone-url-button.png)

![Url to clone](https://help.github.com/assets/images/help/repository/https-url-clone.png)

**Type** the following command into your terminal, **pasting** the git clone url you just copied:

```$ git clone [COPIED GIT CLONE URL]```

and press enter...

You should now have this repo on your machine!
<a name="bare-bones"></a>
## Bare Bones HTML
<a name="edit-html"></a>
### Edit some HTML
In your editor, open the `hack_day_2021/bare_bones` folder.

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

To see all the files you've changed, type:

`$ git status`

To stage your changes to be committed, type:

`$ git add .` OR
`$ git add [file name]` if you only want to commit certain files

Then type the following command to commit the changes to your **local repository**. Your local repository is the git repository that is tracking the changes on your laptop only. Your **remote repository** is your Github repository, the one that saves all your changes online.

`$ git commit -m "Add my name"` OR
`$ git commit` if you set up VS Code with git

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

Something important to know is CSS inheritance. Let's say we have the following HTML and CSS:

```
<style>
.parent {
  color: red;
}
</style>
<div class="parent">
  Parent
  <div class="child">Child</div>
</div>
```
In this example, both 'Parent' and 'Child will be red since the child div has inherited the color attribute set in the parent div!

![Parent child css example with two red colored divs](/../screenshots/screenshots/pc1.png)

But if we change the code to specify a color attribute for the child div:
```
<style>
.parent {
  color: red
}
.child {
  color: green;
}
</style>
<div class="parent">
  Parent
  <div class="child">Child</div>
</div>
```
![Parent child css example with two different colored divs](/../screenshots/screenshots/pc2.png)

The parent is red, but the child is now green.

There are certain CSS properties that child elements will inherit, like color. [Here is a list of them](https://stackoverflow.com/questions/5612302/which-css-properties-are-inherited). Be careful with inherited properties, as they can mess up the styling of your elements in ways that are hard to identify.

Another important thing to understand about CSS is **Specificity**. Specificity is used to determine which attributes should be used when multiple attributes are competing with one another. For example:
```
<style>
.parent {
  color: red
}
.child {
  color: green;
}
.parent .child {
  color: blue;
}
</style>
<div class="parent">
  Parent
  <div class="child">Child</div>
</div>
```
the 'parent' class is set to red, the 'child' class is set to green, but a 'child' class inside a 'parent' class is set to blue. So which color will the child text be?

![The most specific css is displayed](/../screenshots/screenshots/pc3.png)

It's blue!

This is because of specificity rules, which can be shown in a helpful diagram:

```
                              class,
style                         pseudo-class,
attribute         ID          attribute       element
+-------+      +-------+      +-------+      +-------+
|       |      |       |      |       |      |       |  
|       |      |       |      |       |      |       |  
|       |      |       |      |       |      |       |  
+-------+ ,    +-------+ ,    +-------+ ,    +-------+  

most specificity ----------------------> least specificity
value                                    value
```

Essentially, every time a certain value is set you gain a specificity point and the css with the highest specificity value will be displayed. So for the above example, when .child is set to green, (0,0,1,0) points are applied. However, when .parent .child is set to blue, (0,0,2,0) points are applied since 2 classes have been specified. Therefore it has a higher specificity value and takes priority.

If all selectors are of equal specificity, the last css attribute in the document is chosen. For example:

```
<style>
.parent {
  color: red
}
.child {
  color: green;
}
.child {
  color: orange;
}
</style>
<div class="parent">
  Parent
  <div class="child">Child</div>
</div>
```
![The last css is displayed otherwise](/../screenshots/screenshots/pc4.png)

You can read more about CSS Specificity [here](https://css-tricks.com/specifics-on-css-specificity/)!

<a name="responsive-break"></a>
### Responsive Breakpoints
**Breakpoints** are common device widths at which we should change our layout to optimize readability and usability. For example, while a set of links can span horizontally across a laptop screen, those links should stack vertically on a phone. Otherwise some text could get cut off.

We can set a CSS media query to set attributes depending on the breakpoint/screen size. A media query looks like this:
```
@media only screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```
In this example, it says to set the body background-color to light blue when the screen size is less than 600px. The 'only' keyword prevents older browsers that do not support media queries with media features from applying the specified styles. It has no effect on modern browsers.

These are the typical screen sizes that breakpoints are set on:
- 320px — 480px: Mobile devices.
- 481px — 768px: iPads, Tablets.
- 769px — 1024px: Small screens, laptops.
- 1025px — 1200px: Desktops, large screens.

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
Open the `hack_day_2021/bootstrap` folder and open `index.html`.

Your `index.html` is already set up with Bootstrap installed.

Trying to figure out Bootstrap? Here are some important pages in the documentation:
- **[Layout](https://getbootstrap.com/docs/4.1/layout/overview/)**
- **[How Bootstrap Formats HTML tags](https://getbootstrap.com/docs/4.1/content/reboot/)**
- **[Copy and Paste Components](https://getbootstrap.com/docs/4.1/components/)**
- **[Bootstrap Demos](https://getbootstrap.com/docs/4.1/examples/)**
<a name="advanced-bootstrap"></a>

You can set certain (but not all) Bootstrap utilities to activate at certain breakpoints. To do this, use the following syntax in your class names:

```[Bootstrap attribute]-[breakpoint abbreviation]-[Bootstrap value]```

For example:

```text-left text-md-center```

Using the above class names, your text will be left-aligned on all screens with widths smaller than 768px, but centered on all screens above that.

Your default styling, aka the styling that applies to extra small (xs) screens, should have no breakpoint. In this case `text-left`. For greater screen sizes that require different styling, add the appropriate breakpoints. The styling you provide for a breakpoint will apply for all screen sizes greater than that breakpoint — until/unless it reaches a greater breakpoint where you've applied different styling.

You can change styling at every breakpoint, if you want. For example:

``text-left text-sm-center text-md-right text-lg-justify text-xl-right``

In this example, extra small screens will have left-aligned text, small screens will have center-aligned text, medium screens will have right-aligned text, large screens will have justified text, and extra large screens will have right-aligned text.
<a name="grid"></a>
### Grid

The Bootstrap grid allows you to build website layouts using a 12-column grid system. This grid system relies on rows and columns, nested within a div of the `container` css class.

![The grid system, which contains columns labeled with numbers](/../screenshots/screenshots/gridsystem.png)

**Containers** are *required* in order to use the bootstrap 12-column grid system. Most of the time you will just need one container to wrap around your HTML.

A **row** is exactly what is says, it is a row that spans across the 12-column grid. This will make more sense when we go through an example.

A **column** is nested inside a row, and there are many ways to define and utilize them. Essentially, The width of the row is split up into 12-columns and you can define how many columns you want your HTML element to take up.

Let's go through an example:

```
<div class="container">
  <div class="row">
    <div class="col-4">
    </div>
    <div class="col-8">
    </div>
  </div>
</div>
```

Notice the numbers attached to `col`, like `col-4` and `col-8`? Those are not widths in pixels, rather it is proportional to the parent element. `col-4` says, let this div take up 4 out of 12 of the columns (i.e 1/4th of the width), while `col-8` will have the element take up the remaining 8 columns (i.e 3/4 of the width).

The key to the grid system is this: **the column widths must add up to twelve**. If they're more than twelve, they probably won't work. If they're less than twelve, they probably won't work too. Twelve is the golden number in the Bootstrap grid system.

If you don't want to explicitly set the number of columns an element is taking up, you can also just use `col`, in which case the parent element will allocate equal width to the child columns. For example, this will set 3 equal-width containers inside the row:

```
<div class="container">
  <div class="row">
    <div class="col">
    </div>
    <div class="col">
    </div>
    <div class="col">
    </div>
  </div>
</div>
```

<a name="flex"></a>
### Flex

Though the grid is useful, it can be somewhat inflexible. That's what Flex was created to fix (haha). Flex is useful if you need your HTML elements to have more fluid sizing and more controllable alignment.

Flex can be a tough concept to grasp, which is why it's best exemplified through demos. We'll be showing you some, but here are the official Bootstrap demonstrations if you miss us:

- **[Flex Demos and Explanation](https://getbootstrap.com/docs/4.1/utilities/flex/)**


<a name="components"></a>
### Bootstrap Components

One of the best parts of Bootstrap are the interactive components, which are pre-built web components that you can copy/paste/edit. This allows you to easily integrate cool features such as modals, dropdowns, carousels etc into your site! You can access all Bootstrap components [here](https://getbootstrap.com/docs/5.0/components/accordion/)!

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

<a name="wrap-up"></a>
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
