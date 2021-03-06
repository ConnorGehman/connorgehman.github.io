# How to host and Format a Resume on GitHub Pages

# Purpose
This file will guide you through the steps of formatting your resume in Markdown and hosting it on a static site via Github Pages with a customized theme. The individual steps will provide more detail on topics such as Markdown, Github, Github Pages, and Jekyll, and will relate the topics to Andrew Etter's principles from his book: *Modern Technical Writing*.

You can see the wonderful static site resume in action below:
![Website Resume Gif](Website_Resume_Example.gif)


# Prerequisites
*Help for the below requirements can be found under [*More Resources*](#More-Resources)*
* A resume in Markdown format.
    * Markdown is a lightweight, easy to learn, markup language.
    * A Markdown editor will speed up the process.
* Knowledge of Andrew Etter's principles from *Modern Technical Writing* will help, but is not necessary as they will be explained.


# Instructions
## Format your Resume in Markdown
Markdown format is relatively quick to type in compared to alternative markup languages and allows static site generators such as Jekyll to access the contents of your resume, making the upcoming steps much simpler and keeping your work easy to modify.  
1. Download a Markdown editor.
    * There are plenty of Markdown editors, but I personally have 2 favourites (leaning towards the lightweight side): 
        1. Visual Studio Code.
            * This editor is simple, has built-in options for version control (more on this later), and comes with a live-preview option which is in my opinion necessary when working with Markdown.
        2. Sublime Text 3.
            * A very lightweight text-editor that supports Markdown syntax. I use this on my laptop with poor specs alongside a live-preview plugin that can be downloaded via Sublime Text's built-in Package Control.
2. If you are unfamiliar with Markdown itself, I suggest trying [this guide](https://www.markdowntutorial.com/).
3. Create a new  resume or re-write an existing one in Markdown format. 
    * Define your audience. Personalizing your resume for the job you are applying to makes your resume much easier to read for the employer.

Andrew Etter stresses the importance of using a lightweight markup language such as Markdown. It is much easier to work with and will increase your productivity immensely.


## Use Distributed Version Control
Distributed version control systems allow you to manage your projects by providing the means to keep multiple versions of the project, transfer changes between versions, and track all changes made in each version. While the importance of version control is more apparent in projects of a larger scale, we will use Github because of its simple, free static site generation (Github Pages).
1. If you haven't already,[ create a Github account](https://github.com/join).
2. From your Github dashboard, create a Repository (repo).
    * In order to make a Github Pages site in the next step, the repo name must be: `username.github.io`, using your own Github username. For example, my repository is `connorgehman.github.io`.
    * You can select `Add a README` if you like, or add one later. Evidently, READMEs are important for understanding the purpose of the repo.
3. Clone your repository in your Markdown editor (Optional but useful).
    * If you are using a Markdown editor that is compatible with Git version control, you can clone your repository and commit and push any changes to your files from within your editor.
    * I use Visual Studio Code's built-in git support for this. A quick tutorial can be found under [*More Resources*](#More-Resources).




## Generate a Static Website
Now that you have a Markdown formatted resume and a github repository:
1. Rename your resume file to `index.md`.
    * This file will be the main page of your static website.
2. Add your resume file with the name `index.md` to your repository.
    * When commiting a file in Git, provide a short descriptive message about the file or the changes you made to it. Etter's principle of Cataloging the Differences is widely used in Version Control systems. It keeps any changes to the repository well-documented which provides users with the purpose of the changes and allows for easier error-tracking, should something bad happen.
3. Obtain the link to your website.
    * Your specifically named repo and `index.md` file are all Github Pages needs to generate a static website for you from your repository. You can find the link to your static website from the repository under: `Settings -> Github Pages`. You are not done quite yet though...


## Customize your Website's Theme
Andrew Etter stresses the importance of appearance in his book *Modern Technical Writing*, and whats more important than the appearance of your resume? There are multiple ways you can go about changing the theme of your website.

### Option 1 - Github Presets
This is by far the easiest method of changing your website's theme, however, to really personalize your website it is better to go for Option 2.
1. Use Github's Repository settings under the `Github Pages` header to select a theme from some presets.
2. A `_config.yml` file will appear in your repository. edit it (either in your editor of choice or from Github directly) and add a new line `title: Your Name`. This will change your website's title to better fit a resume. The `.yml` file that will be discussed in Option 2.

### Option 2 - Forking a Theme or Jekyll
For more customization you can search for more interesting themes. Many are hosted on github. I will use Beautiful Jekyll as an example. If you wish to make your own, Jekyll has its own tutorials.
1. Search for a theme you like, in this case [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll).
2. Follow its `README.md` for installation instructions.
    * Usually it will involve forking the repository, naming it to the Github Pages naming scheme mentioned above, adding your `index.md` file, then editting the `_config.yml` file to your liking.

I have included an links to YAML syntax and Beautiful Jekyll's `_config.yml` file (which explains what each mapping does) under [*More Resources*](#More-Resources).


## Update your Resume Often
Andrew Etter's principle: Publish Frequently can be used for resumes too. Keep your resume up to date and edit your resume to cater to what a job application is asking for. Since your resume is hosted on a static site it is incredibly simple to change. Just modify your `index.md` file and push the changes. Because its hosted on Github, you can switch between versions of your resume easily. 



## More Resources
1. [Markdown Tutorial](https://www.markdowntutorial.com/)
2. [Andrew Etter's *Modern Technical Writing*](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
3. Markdown Editors: 
    * [Visual Studio Code](https://code.visualstudio.com/)
        * Fairly lightweight, version control support, live preview.
            * [Working with Github in VS](https://code.visualstudio.com/docs/editor/github)
    * [Sublime Text 3](https://www.sublimetext.com/3)
        * Extremely lightweight, supports syntax for many languages, requires Package Control to add a live preview of markdown files.
4. [YAML Syntax Introduction](https://learn.getgrav.org/16/advanced/yaml)
    * [Example _config.yml (Beautiful Jekyll)](https://github.com/daattali/beautiful-jekyll/blob/master/_config.yml)
5. [Github Pages Custom Themes using Jekyll](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/adding-a-theme-to-your-github-pages-site-using-jekyll)
6. Example Theme: [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll)
    * The creator's github page's `README.md` file serves as a very in-depth guide to forking a theme.




# Authors and Acknowledgments
### Principles
* Andrew Etter - [*Modern Technical Writing*](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
### Themes
* Github Pages themes: [slate](https://github.com/pages-themes/slate)
* Example Theme: [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll)

### Peer Review
* Jiachi Sun
* Quoc Nguyen
* Sebastian Araneda


# FAQs
*  Why is Markdown better than a word processor?
    * Markdown is close enough to english that it doesn't impede your writing much at all, and it is compatible with static site generators like Jekyll.
*  Why is my resume not showing up?
    * Github Pages can take anywhere from a minute to several hours (in the worst case) to update your website. Be sure to refresh the cache when viewing your website with `shift + F5`. Take the time to ensure your repo is named properly and ensure there are no errors in your `_config.yml` file.
