---
layout: post
title: How I organize my life in plain text
tags: [plaintext, markdown]
excerpt: Where I explain how I organize my notes, tasks and scanned documents using just files inside folders.
image:
  feature:
date: 2015-12-12T08:28:47-02:00
---

Yesterday I talked about my dislike for proprietary formats for my notes. Now it's time to explain how I organize my notes, documents, tasks, etc.

If you didn't read the previous post, here's the summary: I use only plain text for my notes and tasks, saved in a Documents directory synchronized by Dropbox.

In my system I stored the following information:

- Notes that I check all the time
- References that I may need someday (about my house, my car, etc)
- Notes about completed/abandoned projects
- Tasks I have yet to do
- Tasks I've done
- My personal and professional journal
- Important documents (invoices, contracts, etc)

## How I organize my notes ##

I have **a lot** of notes. Every information that I (may) have to remember (even if just for a couple days) I write down. My license plate, my phone's IMEI, ideas for a new book, a TV show suggested by a friend, terminal commands that I learned, how I solved a hard problem. The list goes on.

The most important thing is that all my notes are inside my directory `~/Dropbox/Notes`.

### Kinds of notes ###

I classify my notes under two categories: notes and references.

References are information that I save to check someday, but I don't access regularly. Examples: my license plate number, the IP address of every device in my own network, the measurements of every room in my house, what shoe size my wife wears.

Notes are more general that are not only reference. Notes are the ones I am going to view and edit more frequently, and may not last that long. Examples: lists of ideas, movies recommended to me, my grocery list, books I want to buy.

### Projects ###

My notes and references can also be related to a specific project that I'm working on.

When I'm writing down information relative to a specific project, there's no reason to leave it in the middle of my general notes. I have a Projects folder, and inside it I create a folder with the name of the project. This I where I save these notes.

I do that for projects on my day job, but also my personal projects. If a project needs its own notes, that's where I keep them. I don't need to see these notes all the time.

When the project is done (or is abandoned) and I don't need the notes anymore, I don't delete the folder. I move the entire project folder to my Archive folder.

I will *probably* never need those notes again, but you never know. This way I can keep them for future reference if needed, while keeping my Projects folder uncluttered.

I am talking about all that organization, but it's important to make it clear that the *majority* of my notes is just sitting directly under my documents folder, not inside any project. I have much more general notes than I have project notes.

### Markdown ###

There is one thing that is true for all my notes, no matter if Notes or References, general or related to a project. All of them are written in Markdown.

Markdown is not a specific format. We can say it's a syntax, a *style* of writing plain text files. If you follow the Markdown syntax, your text can be transformed into a pretty HTML rich-text file when needed.

Markdown is just plain text with some unobstrusive markup, like **\*\*double asterisks to bold\*\***, or _\_underscores\__ to italicize. There are also markups for headers, links, images, tables, etc.

This is the best of both worlds. You can have a readable and organized plain text file, while also having the option to turn it into HTML or DOC if you need formatting (bold, italics, images, headers, etc).

## How I organize my tasks ##

After reading all that, it shouldn't surprise you that I also keep my task list in plain text.

Similar to Markdown, I use what we could call "rich plain text", or plain text created in a specific way to allow apps to read it too.

I have a file `todo.txt`, using a standard that is (surprisingly) also called [Todo.txt][todotxt]. You can read more about it [here][todotxt].

The idea is simple: every line in the text file is a task. Tasks can have a context marked like @context, and they can be assigned to a project by writing +project.

You can also start the line with (A), or (B) or any other letter in the alphabet to define the priority of that task. And that's mostly it. Simple and easy, readable to humans and machines.

Example:

```
(A) Clean blood stains on the floor @home +body

(B) Hide the body in a bag @home +body

(C) Sell my chainsaw on ebay @computer +body

Look for a new room mate on craigslist +apartment

Buy new lamp @errands
```

Using that simple markup I can read and edit my tasks on any text editor available to me. Or I can use Todo.txt apps that present the information in a more organized manner.

Whatever the case, I can always see what my tasks are, no matter what device I'm using.

This is a great example of how I can use an app to help me do stuff (The Todo.txt compatible apps) while still having control over all my files and its contents.

There are Todo.txt apps for [iOS][todo-ios] and [Android][todo-android]. Also Windows, Mac and Linux.

### Done Tasks ###

There is one more nice Todo.txt feature that I use all the time. When a task is done, all you have to do is put an "x" at the beginning of the line. And then apps can move that task to a done.txt file (or you can do it manually if not using an app).

This way your task list stays clean, and you have a history of all the tasks you have done in the past.

If you do weekly or monthly reviews, it helps a lot.

## How I organize my journal ##

One more thing: my journal is also a plain text file. Shocking!

My journal is a single journal.txt file with all the entries one after the other.

And just like the above examples, this is also handled by an app but in a format that I can read and edit manually if needed. I use a terminal app called [**jrnl**][jrnl]. It offers a handful of terminal commands to write to my journal, review previous entries, and even find by tags or date.

But in the end it's a simple plain text file, giving me the peace of mind of knowing I never lose the information I saved in there.

## Going paperless ##

Last but not least, there is one more thing I save in my Documents folder: scanned versions of paper documents.

I have a scanned copy in PDF of all of my documents. My ID, driver's license, and the many documents the Brazilian government expect you to carry with you.

I also scan and save purchase receipts, invoices, bank statements, contracts I signed. Every important document that I have on paper I also have on my Documents folder.

And for those files, there's no way to use plain text. For them, I use a file format that is so supported by so much open source projects that there's no way it's going to fall out of the Earth any time soon: PDF.

PDF files allow text and image. I can annotate it, I can highlight text. But the important thing is that it has images and doesn't take much space.

So all my paper documents are scanned, OCR'd and saved in PDF.

## Apps that I use ##

On android I use [**Neutrinote**][neutrinote] to edit my notes, and [**Todo.txt**][todo-android] to manage my tasks.

On Linux, I use [**Vim**][vim] to edit my notes, and [**QTodoTxt**][qtodotxt] to manage tasks.

On my Mac, I use [**Notational Velocity**][nvalt] for most of the notes, [**Marked**][marked] to read Markdown files in a beautiful format, and the console version of Todo.txt to manage my tasks.

## Everything is a few clicks away ##

There are some things in commom between all those kinds of documents I keep:

1) All of them are always available to me, no matter if I'm at home or out on the streets.

2) I can access any of those files from any device. A desktop, laptop, phone, tablet, or even someone else's computer with a web browser.

3) They will be readable for years to come, no matter what companies die, what servers are turned off, what services become too expensive for me to pay.

If the most important characteristic of a notes system is being available when you need (and I think it is), then this is a great system.

## Keeping my notes for decades ##

I'm only going through all this trouble of making my own system because I want to keep all my notes for as long as I can. I want these notes to serve as a history of my life. I wish I started doing this much sooner, so I could look back in time to what kind of information I was recording when I was younger.

But now I know that I can look back, five years from now, and see what tasks I was doing, what I was worried about, what were my dreams and troubles in my own words.

Whatever I want to do with the information, I know it will be there waiting for me.

[todotxt]:http://todotxt.com
[todo-ios]:http://itunes.apple.com/br/app/todo.txt-touch/id491342186?ls=1&mt=8
[todo-android]:http://play.google.com/store/apps/details?id=com.todotxt.todotxttouch
[jrnl]:https://github.com/maebert/jrnl
[neutrinote]:https://play.google.com/store/apps/details?id=com.appmindlab.nano&hl=pt_BR
[vim]:http://www.vim.org
[qtodotxt]:https://github.com/QTodoTxt/QTodoTxt
[nvalt]:http://brettterpstra.com/projects/nvalt/
[marked]:http://marked2app.com/
