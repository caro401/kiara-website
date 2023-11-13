# Terms

> There's loads of terms thrown around when talking about kiara, which have very specific meanings in this context. We should define the main ones, and when we use those terms in other prose, link to here. I (caro) am super vague on what most of these things actually mean, this existing would be super helpful for me!

## what's a kiara module?

explain this both high level - what does a module mean to a user? some collection of things kiara can do
and at a low level - a module is a python class which subclasses something?

CB: Modules are what you write to create operations. There can be one or multiple modules in one .py document (which allows you to define imported packages and author/desciption metadata). A module will define the inputs and outputs required for an operation; modules are therefore the 'back-end' of the operation, which gets called in the interface/IDE/CLI. Essentially they are the same thing, in two different terms.

## what's a kiara plugin?

again, high level and low level explanation. link out to how to make a plugin tutorial

CB: A kiara 'package': contains all the modules associated with a particular mode of analysis (topic modelling, network analysis etc.) with relevant documentation and, where included, data. Allows people to focus on just the bits they want to use, without downloading everything if they don't want to. Will also allow users to have their own plugin, where they can store all the additional modules that they have created.

## what's a kiara pipeline?

a pipeline isn't a workflow? link out to pipeline tutorial

CB: A collection of modules ordered together (like a defined function) - allows users to run a series of functions/operations all together in one go, rather than step by step.

## what's a workflow?

we kinda use this to mean 2 things, the steps a researcher does to get some results from some data, and a specific kind of file?
[Some of this information also relevant?](https://dharpa.org/kiara/latest/design_docs/architecture/workflows/#the-workflow-lifecycle), maybe we even want a whole page on workflows as a concept?

CB: The process start to end; can be descriptive (aka qualitative understanding of the research process) or literal in terms of the entire coding process. In this second sense, it may be synonymous with pipeline if the pipeline contains all the steps needed for the entire process. It may also be a combination of individual operations and a pipeline, or any conceivable use of kiara start to finish.

## what's a data type?

steps (/operations??) only work on specific data types, they can be something simple like a boolean (true/false) or a string, or complicated like a table with a specific structure

technically, they are a python class that subclasses something??

CB: a bit like string, list, integer etc. in python; essentially same as python data types, though also with kiara specific ones (like network data)

## what's an operation?
CB: A function; 'list operations' gives you all the possible kiara functions, or modules.

## what's a model?

## What's the data store?

maybe this wants a whole page, link also to architecture and reproducible research/lineage. What does it mean to onboard data into kiara, how does it track lineage etc

## what's kiara context
