vvvv-p4v
========

minimalistic package manager for vvvv

Random Ideas
============

p4v can be readed "p for v" (or "pav" or whatever). I just liked the idea of a palindrome name for the file p4v.v4p

A package manager for language Foo should be written with language Foo.

p4v is minimal. Less is more. I will try to add all features inside only one patch named p4v.v4p, whenever is possible.

Having a vvvv patch as a package manager will make it easier to be a community driven utility, keeoing it vvvv-user-friendly.

p4v refers to "How it Works" paragraph in [this](http://vvvv.org/documentation/nodes-and-paths) page.

A package is just a folder containing your stuff. It should have only the following folders

* effects
* modules
* plugins

So a patch in your package will _see_ those folders.

Install p4v should be as easy as copyng the p4v.v4p pach in your empty folder.

p4v.v4p is separated from your root patch, to run it you need to open it explicitly.

If you install package Pippo, p4v will try to

0. *TODO* this is a TBD list
1. look for Pippo in the packages folder
2. pick last folder yyyymmdd 
3. copy the content in current folder

p4v should be able to install package from locally
Maybe the easier thing is to put a "packages" folder inside p4v and use git to clone p4v repo and download all modules
packages folder should look like this

packages/<package name>/yyyymmdd

any contributor could add packages to p4v repo. It could also be used the git submodule feature.


TODO
====

* p4v registry, that is just a 2 fields table: name -> url
* .p4vignore or whatever to skip files, could be also a naming coventions on the folders structure (effects, modules, plugins) and a set of sensible defaults (skip .xml, dynamic plugins dlls etc)
* contextual menu: p4v here, so you can create an empty folder and start a project.
* add dependency chain if it does make sense
