vvvv-p4v
========

minimalistic package manager for vvvv

Random Ideas
============

p4v can be readed "p for v" (or "pav" or whatever). I just liked the idea of a palindrome name for the file p4v.v4p

A package manager for language Foo should be written with language Foo.

p4v

A package is just a folder containing your stuff. It should have only the following folders

    * effects
    * modules
    * plugins

So a root patch in your package will _see_ those folders.

Install p4v should be as easy as copyng the p4v.v4p pach in your empty folder.

p4v.v4p is separated from your root patch, to run it you need to open it explicitly.

If you install package Pippo, p4v will try to
    1. look for Pippo in the registry
    2. get the .zip url associated with Pippo package: this can be a url pointing to the github repo .zip file 
    3. unzip that file in the current folder and then remove it


TODO
====

* p4v registry, that is just a 2 fields table: name -> url
* .p4vignore or whatever to skip files, could be also a naming coventions on the folders structure (effects, modules, plugins) and a set of sensible defaults (skip .xml, dynamic plugins dlls etc)
* contextual menu: p4v here, so you can create an empty folder and start a project.
* add dependency chain if it does make sense
