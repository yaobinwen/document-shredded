# Documentation Best Practices

## No-Criticism Principle

When I talk about the problems in the documentation of any existing product in this or other documents, I have no intention to criticize or blame the developers of the product. I'm merely trying to provide my thoughts about what the problem is and how it can be fixed in order to make the documentation better.

## Motivation

I believe **efficient knowledge transfer is a vital factor for successful software development which is mostly done as a team effort**. Think about it: if everyone is an expert on everything, building software, even though which is not guaranteed to succeed, is more likely to succeed because people know how to use the tools correctly while avoiding the pitfalls of using them.

In reality, chances are everyone is just good at one or two areas. We can identify two scenarios where knowledge transfer is needed:

- Firstly, a junior member is recruited into the team so some senior member needs to teach him/her.
- Secondly, in a team where members rotate the roles, one team member may need to teach another team member the things he/she has worked on in the recent past.

Efficient knowledge transfer can minimize the time that is needed to transfer the knowledge while the precision of the understanding of the transferred knowledge is still sustained. In other words, we spend time to transfer knowledge, not confusion or misunderstanding.

Another way of looking at this is: ideally efficient knowledge transfer is similar to running the "copy" command between two machines. Before "copy" is run, the file of knowledge only exists on one machine; after "copy" is run, an exact copy of this file exists on the second machine, too.

In software industry, documentation is an important means of transferring knowledge from the author of a software package to its potential users and prospective maintainers. The documentation can be as simple as a single `README` file or a whole site of documents.

Unfortunately, I've observed many such documentation efforts not achieving the goal of "efficient knowledge transfer": typically, they fail to discuss the topic clearly enough which causes the readers either to be confused thus have to spend more time to learn the material, hence wasting more time, or, worse, to think they "understand" the topic but in fact they really haven't.

This project, `Document Shredded`, aims at advocating the best practices of documentation and alerting the bad practices of documentation so we can make knowledge transfer among software developers more efficient.

## What This Is

This is a repository that collects documentation good practices with examples and bad practices as counter-examples in order to create a repeatible process of creating easy-to-understand documentation.

Although this repository is created with software documentation in mind, I believe the practices are applicable to all technological areas.

## Who This Is For

This repository is primarily targeted to software developers who are usually not considered as a documentation writer. However, as I said above, I believe all the developers or engineers who work in the technological areas can be beneficial from it.

## Best Practices

Provide an overview on the fundamental concepts to lay a good foundation for the readers of why a certain thing is done in a certain way. A good example is the [_SVN Book: Chapter 1. Fundamental Concepts_](https://svnbook.red-bean.com/en/1.7/svn.basic.html). [_Mastering CMake: Key Concepts_](https://cmake.org/cmake/help/book/mastering-cmake/chapter/Key%20Concepts.html#key-concepts) is the same attempt but I don't think the key concepts there are sufficient: they still miss some concepts I think are important for readers to understand the tool.

This article ["What nobody tells you about documentation"](https://www.divio.com/blog/documentation/) is a must-read! It separates the documentation into four quadrants, each of which takes a different responsibility:

> - Tutorials
>   - is **learning-oriented**
>   - allows the newcomer to get started
>   - is a lesson
> - How-to guides
>   - is **goal-oriented**
>   - shows how to solve a specific problem
>   - is a series of steps
> - Explanation
>   - is **understanding-oriented**
>   - explains
>   - provides background and context
> - Reference
>   - is **information-oriented**
>   - describes the machinery
>   - is accurate and complete

The great thanks go to [Daniele Procida](https://twitter.com/evildmp) who makes it so clear and concise!

## Current Issues

With the above-mentioned four documentation quadrants, I find many documentations are poor because of the lack in "Explanation": they provide a lot of tutorials and how-to guides but fail to give a conceptual explanation of the product components and how and **especially why** they are put that way.

I **strongly believe** understanding `why`s is crucial to using the product correctly, because those `why`s reflect the problems the product is solving. Not understanding the `why`s may result in using the product in the wrong context to solve the wrong problem.

## Doc Smells

### Reference without Definition

See the section ["Control Machine Requirements"](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#control-machine-requirements) of Ansible's documentation. This section is the first time the term "control machine" is used, but there is no definition or explanation of what a "control machine" is. The reader needs to infer it from the context.

This looks quite like in a program you start to use a variable without defining it. "Hey," you may argue, "the compiler should be smart enough to figure out what that variable means from its context. Any compiler that's unable to do so is dumb."

## Useful Links

- [14 Examples of Documentation Mistakes You Are Making](http://blog.screensteps.com/14-examples-of-bad-documentation)
- [Poor Documentation: Why It Happens and How to Fix It](http://www.fortherecordmag.com/archives/0516p12.shtml)
- [Documentation Bad Habits: Shortcuts in Electronic Records Pose Risk](http://library.ahima.org/doc?oid=81008#.W1uFmnXwbdE)
