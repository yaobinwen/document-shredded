# CMake and Documentation

## Referenced Version

- [1] I use the source code of [`v3.22.0-rc2`](https://gitlab.kitware.com/cmake/cmake/-/tree/v3.22.0-rc2). The documentation is [here](https://cmake.org/cmake/help/v3.22/).
- [2] The `Mastering CMake` book repository has only the `master` branch without any tags, so I'll pin down [a specific revision](https://gitlab.kitware.com/cmake/mastering-cmake/-/commit/39dfd284e62347eb068b013709697b4e17b43155) as of 2021-11-03. The online version is [here](https://cmake.org/cmake/help/book/mastering-cmake/).
- [3] [CMake Community Wiki](https://gitlab.kitware.com/cmake/community)

## Issues

1. No overview of the concepts.
2. The tutorial `Step 3: Adding Usage Requirements for a Library` doesn't explain the topic well: it talks about **what** to do but doesn't help the readers to see **how** it is done. I didn't understand the topic until I read [here](https://cmake.org/cmake/help/book/mastering-cmake/chapter/Key%20Concepts.html#usage-requirements) which also explains **how** (i.e., the mention of `target_link_libraries`).
3. The tutorial `Step 10: Adding Generator Expressions`.

Generally speaking, after reading the entire tutorial, one still doesn't have a full grasp of the tool: they may know how to write some code to make it work; but if there is a problem, they may not know where to look.
