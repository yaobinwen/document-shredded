# Bazel

## Example 1: No example for "Generated files should be prefixed with ":""

The section [References to targets in the current package](https://bazel.build/build/style-guide#targets-current-package) says:

> Files should be referred to by their paths relative to the package directory (without ever using up-references, such as `..`). Generated files should be prefixed with "`:`" to indicate that they are not sources. Source files should not be prefixed with `:`. Rules should be prefixed with `:`. For example, assuming `x.cc` is a source file:
>
> ```
> cc_library(
>     name = "lib",
>     srcs = ["x.cc"],
>     hdrs = [":gen_header"],
> )
>
> genrule(
>     name = "gen_header",
>     srcs = [],
>     outs = ["x.h"],
>     cmd = "echo 'int x();' > $@",
> )
> ```

The problem in this section is: The paragraph mentions two cases of prefixing with `:` but the example seems to only explain the case of rules. As a result, the reader may have the question: **Does the fact that "the example only shows rules being prefixed with `:`" mean "rules" and "generated files" are actually the same thing?**
