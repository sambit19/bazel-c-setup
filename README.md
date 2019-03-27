This is a sample C Language project where Bazel is being used as the build tool. One can use this project to customize and use it as per his requirements.

Workspace: A workspace is a directory on your filesystem that contains the source files for the software you want to build, as well as symbolic links to directories that contain the build outputs. Each workspace directory has a text file named WORKSPACE which may be empty, or may contain references to external dependencies required to build the outputs

The WORKSPACE file, which identifies the directory and its contents as a Bazel workspace and lives at the root of the project’s directory structure,

Run the command to build
```
cd packge_1
bazel build //main:hello-bazel
````

To run the application

```
bazel-bin/main/hello-bazel
```


