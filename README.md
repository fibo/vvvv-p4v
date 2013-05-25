vvvv-p4v
========

minimalistic package manager for [vvvv][1]

> A package manager for vvvv should be coded with vvvv language.

Random Ideas
============

> p4v can be readed "p for v" (or "pav" or whatever). I just liked the idea of a palindrome name for the file p4v.v4p


p4v is minimal. Less is more. I will try to add all features inside only one patch named p4v.v4p, whenever is possible.

Having a vvvv patch as a package manager will make it easier to be a community driven utility, keeping it vvvv-user-friendly.

p4v refers to *How it Works* paragraph in [this page][2].

A package is just a folder containing your stuff. It should have only the following folders

* effects
* modules
* plugins

So a patch in your package will _see_ those folders.

Install p4v should be as easy as copyng the p4v.v4p pach in your empty folder.

p4v.v4p is separated from your root patch, to run it you need to open it explicitly.

If you install Foo contribution, p4v will try to

1. download Foo.zip from contributions
2. unzip Foo contribution under addonpack folder


TODO
====

* add documentation page on vvvv site
* p4v registry, that is just a 2 fields table: name -> url
* .p4vignore or whatever to skip files, could be also a naming coventions on the folders structure (effects, modules, plugins) and a set of sensible defaults (skip .xml, dynamic plugins dlls etc)
* contextual menu: p4v here, so you can create an empty folder and start a project.
* interact with webdevvvvs to create a CVAN (Comprehensive Vvvv Archive Network)and host it on vvvv.org
* upload a contribution

[1]: http://vvvv.org "vvvv - a multipurpose toolkit"
[2] http://vvvv.org/documentation/nodes-and-paths"vvvv documentation - nodes and paths]

