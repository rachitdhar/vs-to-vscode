# vs-to-vscode
VS Code config for .NET apps previously running on Visual Studio.

Here, two projects are taken as an example. One is a simple .NET project, where the .dll is needed to be run. The second is an Azure Functions project, which requires a different config, along with the corresponding extension (as mentioned below).

## Steps

- Open the root directory in vscode
- Here, add the .vscode folder inside. (make sure it is ignored by git, if so required)
- Inside this .vscode folder, add two config files. These files are for telling vscode how it is going to launch any particular project: (1) launch.json, and (2) tasks.json.

These files are given in the repo.

**Note**: "Clean Solution" will show up as an option in the Run and Debug menu list.
Alternatively, clean solution can be done directly by running the command:

```
dotnet clean ./<PATH_TO_.sln>
```

at the root directory path.

## VS Code Extensions to Install

- For basic C# project work, install C# Dev Kit (by Microsoft)
- To use Azure functions projects, install the Azure Functions (by Microsoft). No sign in is required to use this for running and debugging locally.

