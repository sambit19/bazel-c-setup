This directory contains C files and Bazel files: The primary unit of code organization in a workspace is the package. A package is a collection of related files and a specification of the dependencies among them.

One or more BUILD files, which tell Bazel how to build different parts of the project. (A directory within the workspace that contains a BUILD file is a package. You will learn about packages later in this tutorial.)

If you look at the code under package_1/main directory:

```
cc_binary{
    name = "hello-bazel",
    srcs = ["hello-bazel.c"],
}

````

In this case the hello-bazel target instantiates Bazel's built-in cc_binary rule. The rule tells Bazel to build a self-contained executable binary from the hello-bazel.c source file with no dependencies