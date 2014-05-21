`git` and github
=================

Introduction
---------------

> Your closest collaborator is you six months ago, but you don't reply emails. 

> -Paul Wilson

`git` and [github](http://github.com) are tools to make version control and collaboration easier. Writing code, papers, presentations, and other scientific products requires iteration and input from multiple sources. *Ad hoc* approaches suffer from a variety of problems that occasionally have disastrous consequences. The following examples illustrate some of these problems. 

### Example 1: Reverting changes

A recent paper I worked on used data from a disease registry, which released "frozen" databases quarterly. While working on the revisions, a new database was released. I used to new database to update the analysis because it contained the most reliable and up to date information. After completing the revisions, I received this email from the lead author (this was in 2013 btw): 

> As you can see from the paper I sent you, it is almost complete and I do not want to re-write it.  Therefore, I just want the data described in the e-mail below from the June 1, 2011 data freeze.  ... Is it possible to reconstruct the data inquiry as per what was originally delivered?

I had not saved prior versions of the analysis code, not to mention the manuscript with all of the results incorporated into the text. My only option at that point was to start over.

### Example 1b: Collaborating on an analysis

Another statistician took over an analysis for a manuscript that I thought was complete. Here is a real email exchange

>The manuscript says that out of 1350 participants there were 411  with incident AFib.
However, when I run your code to create the dataset, I only end up with 232. The AFib data came from a file called “mathew_main”.  Did you use anything else to get the extra AFib cases?

My response:

>I'm not 100% sure about anything without looking at my code. Which file are you going on? There should be a dated .Rnw file my Afib folder that contains all the analysis code. I believe that calls an R script called "load-data-chs.R". The mathew_main file does not sound familiar, I suspect that is from a very old version of the paper. 

:(

### Example 2: Incorporating edits on a manuscript

Applied papers that I've worked on had between 5 and 13 authors. Inevitably, a "final" draft of the manuscript (usually a Word document) gets circulated *via* email and comments or suggestions are solicited. Here are the typical types of responses that I get:

* A new word document with tracked changes
* A new word document with untracked changes
* Suggestions listed in the body of an email
* A txt file with suggested changes
* A scanned copy of the paper with hand-written edits
* No response

The challenge is to incorporate (or not) all of the changes from a variety of collaborators, while keeping a record of who has contributed what. 

### Example 3: Sharing content

Once a paper gets published, occasionally people want to use or extend the method. 

> I would be very grateful if you are able to help me implement this tool in my dataset as well.

 
> Could you please send me your code so that I can try to apply it to my example? 

 
>Would you please kindly e-mail me your article and other works in that field promptly.?


**Email is an ineffective tool for sharing code, data, documents**

What are `git` and github?
----------------

`git` is a system for formal version control. The manpage describes it as "the stupid content tracker". It was developed to manage the source code for Linux. Now it is used to track text files, code, and more. Files are organized into **repositories** in which users **commit** changes and/or additions. The entire history of **commits** and their comments are stored by `git` so that at any point, you can view the differences between current and past versions. It comes preinstalled in Linux and OSX. Type `man git` at the console for more information. 

Github [(www.github.com)](http://github.com) is a website that hosts `git` repositories. It provides an interface for exploring repositories, viewing code, downloading repositories, and interacting with collaborators. It also provides some handy services like website hosting, markdown rendering, and training. 

There are alternative to github. The one that I'm aware of is called [Bitbucket](http://bitbucket.org). *You don't need to use a web host to use `git`*. You can use `git` locally to track content (on a network drive, for instance). 


How do I use them? 
------------------






