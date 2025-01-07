# Welcome to The Multilingual Quantitative Biologist!

The frontiers of Biology are increasingly at the interface between
mathematics, computing, and large empirical datasets (increasingly
often, *truly* "big data"). Answering important problems about issues
ranging from disease dynamics and epidemiology to the effects of climate
change and over-fishing on aquatic ecosystems require computationally
sophisticated approaches for management & analysis of large amounts of
data, building theoretical models, and fitting these models to those
data. Indeed, biology is *the* new frontier for applied computer science
and mathematics. Donald Knuth, an eminent mathematician and computer
scientist has said:

```{epigraph}
"It is hard for me to say confidently that, after fifty more years of explosive growth of computer science, there will still be a lot of fascinating unsolved problems at peoples' fingertips, that it won't be pretty much working on refinements of well-explored things. Maybe all of the simple stuff and the really great stuff has been discovered. It may not be true, but I can't predict an unending growth. I can't be as confident about computer science as I can about biology. Biology easily has 500 years of exciting problems to work on, it's at that level." 
```

This Book aims to provide materials to self-learn or teach computational
approaches, methods and techniques for the empirical and theoretical study of
ecological and evolutionary systems. A major focus is on *Data Science* and
*Ecology and Evolutionary Biology* in particular, because some of the most
complex and important data and dynamics in human-dominated as well as natural
environments arise from ecological and evolutionary processes. Therefore,
computational skills needed to analyse and model ecological and evolutionary
systems are very relevant to other disciplines. For example, it is now generally
recognized that a major new frontier in understanding disease dynamics and
epidemiology is the need to consider the *Ecology* of infectious diseases.
Similarly, scientists are increasingly beginning to appreciate that the ecology
of, and evolution in, agricultural crop fields is crucial for maintaining
yields. Furthermore, ecological and evolutionary models and computational tools
are also relevant for non-biological disciplines --- for example, ecosystem
models are increasingly being considered relevant for understanding
microeconomic systems.

## Why Quantitative Biologist?

The goal of this book is to teach you to become (or at least show you the path
towards becoming) a competent quantitative biologist. A large part of this
involves learning computer programming. Why do biologists need to write computer
programs? Here are some (hopefully compelling!) reasons:

* Short of fieldwork, programs can do anything (that can be specified). In fact,
  even fieldwork, if you could one day *program* a robot to do it for you
  <sup>[^footnote1]</sup>.

* As such, no software is typically available to perform exactly the analysis
  you are planning. You should be unhappy if you are trying to shoehorn your
  data into methods that don't quite seem right.

* Biological problems and datasets are some of the most complicated imaginable.
Programming permits success despite complexity through precise specification and
modularization of complicated analyses.

* Modularity – programming allows you to break up your complex analysis in
  smaller pieces, yet keep all the pieces in a single, functional analysis.

* Reproducibility – you (or someone else) can just re-run the code to reproduce
  your analysis. This is also the key to maintaining scientific accountability,
  integrity, and accuracy.

* Organized thinking – writing code requires you to do this!

* Career prospects – good, scientific coders are in short supply in all fields,
  but most definitely in biology!

## Why *Multilingual*?

There are several hundred programming languages currently available – which ones
should a biologist choose? This book are built on the philosophy that
quantitative biologists can significantly benefit from being multilingual
programmers, knowing:

1. A modern, easy-to-write, versatile, interpreted (or semi-compiled) language
   that is "reasonably" fast, like `Python`

2. Mathematical and statistical software with programming and graphing
   capabilities, like `R`

3. A compiled (or semi-compiled)
   '[procedural](https://en.wikipedia.org/wiki/Procedural_programming)'
   language, like `C`

And all these because one language doesn't fit all purposes. Something like `C`,
the last item in the list above, is a "procedural" language that forces you to
deal with the real "under the hood" workings of your computer (especially,
memory management). Without an understanding of these 'low-level' aspects of
computer programming, you will be limited in your ability to develop
applications that either intrinsically require you to optimize performance, or
need to be run in a memory- or performance-constrained environment (combination
of computer hardware and operating system). Languages like Python and R
intentionally obscure a lot of details of the underlying computer science,
trading-off performance in favor of ease of programming and running code.
However, they are sufficient for the purposes of most research and industry
programming requirements.

You will learn `Python` and `R` (along with the `bash` language) in this book.
These two are among the most popular languages
[currently](https://www.tiobe.com/tiobe-index) (also [see
this](https://spectrum.ieee.org/top-programming-languages-2021)), and with good
reasons. We will not learn any procedural languages here, but it may be
necessary for some of you to learn something like `C` in certain lines of
research or industry jobs. Just be aware if this, and keep your mind open to the
possibility of learning yet another language!

## R vs. Python

We will use R mainly for data analysis and visualization because it a great one
stop solution for these purposes. If you are keen on trying data analyses in
Python, see [this Appendix](./notebooks/Appendix-Data-Python.ipynb). In general,
R will do the job for most of your purposes. There not much between these two
languages for data science. Python is somewhat more computationally efficient,
and is a multi-purpose programming language with a very clean and easy-to-learn
syntax. It is generally used by data scientists in the industry to for
exploratory data analysis and machine learning in team-driven production
environments. R, on the other hand, has been built mainly by by academic
researchers and statisticians, and has a wider range of *inbuilt* (not requiring
additional packages) statistical analysis capabilities. Learn more about R vs
Python for data science
[here](https://www.kdnuggets.com/2015/05/r-vs-python-data-science.html) and
[here](http://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1523009719/main-qimg-9dcf536c501455f073dfbc4e09798a51_vpijr0.png). 

## Some guidelines, conventions and rules

Our goal is to teach you not just programming, but also good computing
practices. In this course, you will write plenty of code, deal with different
data files, and produce text and graphic outputs. You will learn to keep your
project and coursework organized in logical, efficient, error-free, and
reproducible *workflows* (that's a mouthful, but an important mouthful).

### Beware the dark forces

Avoid the temptation to use spreadsheet software (e.g., Excel) while working
through this book's content. There are times when you will feel the [pull of the
dark side](https://starwars.fandom.com/wiki/Dark_side_of_the_Force), and imagine
a more "comfortable" world where you are mouse-clicking your way happily though
spreadsheet-based data manipulations and analyses. NO! You will be doing
yourself a disservice. On the long-ish run you will be much better off
visualizing and manipulating data on your computer using a programming language
like R. This is something you will learn, young
[*padawan*](https://starwars.fandom.com/wiki/Padawan)!

### Keep your workflow organized

In the following chapters, you will practice many examples where you are
required to write large blocks of code. Please get into the habit of writing
code into text files with an appropriate extension (e.g., `.R` for `R` code,
`.py` for `python` code, etc.). Furthermore, please keep all your code files
organized in one or more directories (e.g., named `Code`!). Similarly, some of
these scripts will take data files as inputs, and output some results in the
form of text or graphics. Please keep these inputs and outputs organized as
well, in separate directories (e.g., named `Data` and ` Results`) respectively.
Your instructor(s) will help you get set up and abide by this "workflow".

---
```{figure} ./notebooks/graphics/workflow.png
---
width: 300px
name: xkcd-workflows
alt: xkcd on workflows
align: center
---
Logical workflows are important, but don't get married to yours!
<small> <center>(Source: [xkcd](https://xkcd.com/1172/)) 
</center></small>
```

---

### Conventions used in this document

Throughout these sessions, directory paths will be specified in UNIX (Mac,
Linux) style, using `/` instead of the `\` used in Windows. Also, in general, we
will be using [relative paths](https://en.wikipedia.org/wiki/Path_(computing))
throughout the exercises and practicals (more on this later, but google it!).

You will find all command line/console arguments, code snippets and output in
boxes like this:

```

```

You should type the commands/code that you see in such boxes into the relevant
command line. Don't copy-and-paste - you likely need all the command / syntax
typing practice you can get ! Also, copying-and-pasting chunks of code without
understanding them, i.e., blindly shoveling data into a black box and assuming
the output is correct and meaningful, will eventually lead to frustrations, and
if you are unlucky, embarrassments or even catastrophes!

Note that the command line prompt you will see on your own terminal/console will
vary with the programming language: `$` for UNIX, `>>>` for Python, `>` for R,
etc.

Also note that:

&#9733; Lines starting with a star like this will be specific instructions for
you to follow

And there will be notes, tips and warnings that you should pay particular
attention to, which will appear like this:  

```{note}
This is a note
```

```{tip}
This is a tip
```

```{warning}
This is a warning
```

So here's your first (and perhaps most important) tip:

```{tip}
**Finding solutions online.**  This document does not tell you every single thing you need to know to perform the exercises in it. In programming and computing, you learn faster by trying to solve problems on your own. The contemporary way to do this is to google the problem! Some suggestions: 
* Your typical approach should be to serach online the main keywords along the programming language name (e.g., "unix mv vs cp" or "R create empty dataframe"). 
* Look for [stackoverflow](https://stackoverflow.com/) or [stackexchange](https://stackexchange.com/) based results in particular. Look for number of endorsements for both the question that has been asked, and for its answer.
* Be selective - there will often be multiple solutions to the same issue or problem - don't just blindly use the first one you find. 
* Also, every time a mysterious, geeky-sounding term like "relative path" or "version control" appears, please search (e.g., google) it online it as well!
```

### To IDE or not to IDE?

As you embark on your journey to becoming a competent practitioner of biological
computing, you will be faced with a Hamletian question: "To IDE or not to IDE"
(anagram alert!). *OK, maybe not that dramatic or Hamletian...*

An interactive Development Environment (IDE) is a text editor with additional
features that can make life easy by allowing auto-formatting of code, running
code, providing a graphic view of the workspace (your active functions,
variables, etc.), graphic debugging and profiling (you will see these delightful
things later), and allowing integrated version control (e.g., using `git`). 

You will benefit a lot if you use a code editor that can also offer an IDE. At
the very least, your IDE should offer:

* Auto-indentation

* Automatic code wrapping (e.g., keeping lines <80 characters long)

* [Syntax highlighting](https://en.wikipedia.org/wiki/Syntax_highlighting)
  (language elements such as variables, commands, and brackets are differently
  colored)

* Code folding (fold large blocks of code, say an entire function or loop)

* Keyboard control of commenting/uncommenting, code wrapping, etc.

* Embedded terminal / shell / commandline console

* Sending commands to terminal / shell

* Debugging


If you end up using multiple programming languages, you will want an IDE that
can handle them. Four commonly-used and very powerful multi-lingual code
editors/IDEs are: Emacs, Vim, Visual Studio Code (AKA VS Code), and Atom.  We
will use [Visual Studio Code](https://code.visualstudio.com) in this course,
because it is freely available, is relatively easy to master,  and has many
plugins that make multilingual code development easier. Atom, Vim and Emacs are
also great alternatives. The last having a steeper learning curve, but are very
powerful once you have mastered them. 

#### Gooey IDEs

IDEs come with graphic user interfaces (GUI's, or "gooeys") of differing levels
of sophistication and shiny-ness. Some go over and above the call of duty to
offer further useful features like embedded data and plot views and package
management. One such example is th freelty available
[RStudio](http://rstudio.org), which is dedicated to R.  However, there is a
tradeoff &ndash; these are necessarily specialized to one language (e.g.,
RStudio). It is up to you if you want to use multiple, language specific IDEs,
or one somewhat less shiny multi-lingual IDE.

### Assessment

Your MQB coursework may be assessed. If you have been told that it will, please
see [this Appendix](./notebooks/Appendix-Assessment.md). 

## Using this book

Most of the chapters and appendices of this book are written as
[jupyter](./notebooks/Appendix-JupyIntro.ipynb) notebooks. Each is accompanied
by data and code on which you can practice your skills. These materials are
available (and updated regularly) at a public [git
repository](https://github.com/MulQuaBio/MQB).

```{tip}
If you do not use git, you may download the code, data, this book, and other
course materials from the [repository](https://github.com/MulQuaBio/MQB)
at one go look for the green "Clone or Download" button and then clicking on the
"Download repository" link. You can then unzip the downloaded .zip and grab the
files you need.
```

It is important that you work through the exercises and problems in each chapter
pr appendix. This Book does not tell you every single thing you need to know
to perform the exercises in it. In programming and computing, you learn faster
by trying to solve problems (including computer crashes!) on your own, often by
liberally googling the problem!

---

**Footnotes**

[^footnote1]: That way you can traipse around the forest catching rare
    butterflies and frogs while the robot does the boring data collecting for
    you.