<!---

TASK LIST:

  * Use cp -rf *.* to copy all of the files and directories in this repository
    to the starter repository for this assignment
  * Change into the directory for the starer repository
  * Update the header (e.g., #) to only give the name of the assignment
  * Update the first paragraph to include the commented-out content
  * Change the link in the # Problems section to point to this lab's starter
  * Create the assignment in the GitHub Classroom, noting the URL
  * Test the assignment by accepting it with your own GitHub account
  * Check to ensure that your GitHub repository is created correctly
  * Share the assignment link with all of the students using email or Slack

PROBLEMS?

  * Contact Gregory M. Kapfhammer by email or Slack
  * Raise an issue in the GitHub repository for this assignment

-->

# cs302-S2019-lab8-starter

Designed for use with [GitHub Classroom](https://classroom.github.com/), this
repository contains the starter for Laboratory 8 in Computer Science 302. Since
the Travis builds for this repository will initially fail (as evidenced by a
red &#x2717; appearing in the commit logs instead of a green &#x2714;), the
programmer is responsible for completing all of the steps needed to satisfy the
requirements for the assignment, thus causing a &#x2714; to instead appear in
the commit logs.

## Introduction

This assignment requires a programmer to implement a static web site that
features a mobile-ready (or, "responsive") design like those described in
Section 7.8 of the textbook. Importantly, a student is fully responsible for
designing, implementing, and testing this responsively designed site. With that
said, you can learn more about the steps that you should take to implement the
mobile-ready site by reviewing the assignment sheet and the comments in the
provided HTML source code. As before, this assignment requires you to run a web
server to provide local access to the static web site, specifically loading the
default document. Finally, you will continue to practice using the
[HTMLHint](http://htmlhint.com/) static analysis code tool that can check HTML
files for potential errors.

The programmer is also responsible for writing a reflection, stored in the file
`writing/reflection.md`, that responds to the questions in the assignment sheet
and explains the challenges that you faced and the solutions you developed.
Please note that this is also a Markdown file that must adhere to the standards
described in the [Markdown Syntax
Guide](https://guides.github.com/features/mastering-markdown/). Remember, you
can preview the contents of a comitted Markdown file by clicking on the name of
the file in your GitHub repository. Finally, don't forget that your
`writing/reflection.md` file and the file mentioned in the previous paragraph
should both adhere to the Markdown standards established by the [Markdown
linting tool](https://github.com/markdownlint/markdownlint) and the writing
standards set by the [Proselint tool](http://proselint.com/).

Please note that this repository only furnishes minimal HTML source code. You
should provide all of the other directories and files that are needed. Remember,
you can use the `mkdir` command to make a directory in your GitHub repository.
If you have not used this command before, then you can learn more about it by
running the command `man mkdir` in your terminal window. Additionally, this
assignment encourages you to load the required CSS files from a "content
delivery network" (or, CDN) that provides access to source code for both
Bootstrap and Bootswatch. Finally, the main checks that GatorGrader performs are
for the existence of certain files (e.g., the screenshot that shows your final
web site). More details about the GatorGrader checks are included later in
this document and in the assignment sheet.

When you use the `git commit` command to transfer your source code to your
GitHub repository, [Travis CI](https://travis-ci.com/) will initialize a build
of your assignment, checking to see if it meets all of the requirements. If both
your source code and writing meet all of the established requirements, then you
will see a green &#x2714; in the listing of commits in GitHub. If your
submission does not meet the requirements, a red &#x2717; will appear instead.
The instructor will reduce a programmer's grade for this assignment if the red
&#x2717; appears on the last commit in GitHub immediately before the
assignment's due date.

A carefully formatted assignment sheet for this project provides more details
about the steps that a computer scientist should take to complete this
assignment. You can view this assignment sheet by visiting the listing of the
laboratories on the course web site. Remember, it is critically important that
you review and understand the notes in the provided source code and referenced
web sites as you are completing this assignment.

## Learning

If you have not done so already, please read all of the relevant [GitHub
Guides](https://guides.github.com/) that explain how to use many of the features
that GitHub provides. In particular, please make sure that you have read the
following GitHub guides: [Mastering
Markdown](https://guides.github.com/features/mastering-markdown/), [Hello
World](https://guides.github.com/activities/hello-world/), and [Documenting Your
Projects on GitHub](https://guides.github.com/features/wikis/). Each of these
guides will help you to understand how to use both [GitHub](http://github.com)
and [GitHub Classroom](https://classroom.github.com/). Additionally, to learn more
about how to include emojis in an HTML file, please read the documentation for
the [Emoji CSS library](https://afeld.github.io/emoji-css/). Finally, don't
forget to read all of the referenced web sites that are mentioned in the
provided HTML source code.

To do well on this assignment, you should also review Chapters 1 through 6 of
the course textbook, additionally paying close attention to Sections 7.1 through
7.8 and Listing 7.4. Please see the course instructor or one of the teaching
assistants or tutors if you have questions about any of these reading
assignments.

## Commands

To get started in using the GatorGrader tool, you can change into the directory
for this assignment and type the command `gradle grade` in your terminal.
Running this command will produce a lot of output that you should carefully
inspect. If the output indicates that GatorGrader judges that there are no
mistakes in the assignment, then this means that your source code and writing
are passing all of the automated baseline checks. However, if the output
indicates that there are mistakes, then you will need to understand what they
are and then try to fix them. Finally, remember that you must run the `gradle
grade` command from the main (or "home base") directory for this assignment
where the `build.gradle` file is located. Then, you can type the command in
the terminal and study the output.

## Checking

In addition to making the checks that were previously mentioned in the
introduction to this document, your final submission must meet the following
requirements. Specifically, GatorGrader will check for the existence of the
`reflection.md` file in the `writing` directory and, respectively, the existence
of `index.html` in the `src/www/` directory and `responsive_submission.png` in
the `images/` directory. GatorGrader will also check to ensure that your files
do not contain any markers indicating that your files are not yet complete.
Finally, GatorGrader will check to ensure that you have furnished an answer
for each of the technical questions in the `reflection.md` file in the
`writing` directory. One of your responses in the `reflection.md` file
should feature two fenced code blocks, with one containing HTML and the
other with CSS. You can learn about the other checks that GatorGrader
performs by typing `gradle grade` in your terminal window.

## Updates

If the course instructor updates the provided material for this assignment and
you would like to receive these updates, then you can type this command in the
main directory for this assignment:

```
git remote add download git@github.com:Allegheny-Computer-Science-302-S2019/cs302-S2019-lab7-starter.git
```

You should only need to type this command once; typing the command additional
times may yield an error message but will not negatively influence the state of
your repository. Now, you are ready to download the updates provided by the
course instructor by typing:

```
git pull download master
```

This second command can be run whenever the course instructor needs to provide
you with new source code for this assignment. However, please note that, if you
have edited the files that the course instructor updated, running the previous
command may lead to Git merge conflicts. If this happens, you may need to
manually resolve them with the help of the instructor or a teaching assistant.

## Travis

This assignment uses [Travis CI](https://travis-ci.com/) to automatically run
the checking programs every time you commit to your GitHub repository. The
checking will start as soon as you have accepted the assignment, thus creating
your own private repository, and the course instructor enables Travis for it. If
you are using Travis for the first time, you will need to authorize Travis CI to
access the private repositories that you created on GitHub.

## Requirements

The GatorGrader software that supports the checking of this assignment was
developed for the following software and versions:

- Gradle 4.6
- Java 1.8.0
- MDL 0.4.0
- Proselint 0.8.0
- Python 3.6

## Problems

If you have found a problem with this assignment's provided source code, then
you can go to the [Computer Science 302 Lab 8
Starter](https://github.com/Allegheny-Computer-Science-302-S2019/cs302-S2019-lab8-starter)
repository and create an issue by clicking the "Issues" tab and then clicking
the green "New Issue" button. If you have found a problem with the [GatorGrader
tool](https://github.com/gkapfham/gatorgrader) and the way that it checks you
assignment, then you can follow the aforementioned steps to create an issue in
its repository. To ensure that your issue is properly resolved, please provide
as many details as is possible about the problem that you experienced. If you
discover a problem with the laboratory assignment sheet, then please raise an
issue in the
[cs302-S2019-sheets](https://github.com/Allegheny-Computer-Science-302-S2019/cs302-S2019-sheets)
repository and mention this assignment.

Students who find, and use the appropriate GitHub issue tracker to correctly
document, a mistake in any aspect of this laboratory assignment will receive
free laptop stickers and extra credit towards their grade for it.

## Assistance

If you are having trouble completing any part of this project, then please talk
with either the course instructor or a teaching assistant during the laboratory
session. Alternatively, you may ask questions in the Slack team for this
course. Finally, you can schedule a meeting during the course instructor's
office hours.
