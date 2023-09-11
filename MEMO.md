# Development Notes

## 2023-09-05

- ( 2023-09-05 10:48:15 )
```
jazzwang:~/git$ git clone git@github.com:jazzwang/dotnet-codespace.git
Cloning into 'dotnet-codespace'...
warning: You appear to have cloned an empty repository.
jazzwang:~/git$ cd dotnet-codespace/
jazzwang:~/git/dotnet-codespace$ ls
jazzwang:~/git/dotnet-codespace$ cp ~/.gitconfig .
jazzwang:~/git/dotnet-codespace$ vi .gitconfig
jazzwang:~/git/dotnet-codespace$ git gi csharp > .gitignore
jazzwang:~/git/dotnet-codespace$ git add .
jazzwang:~/git/dotnet-codespace$ git commit -a
jazzwang:~/git/dotnet-codespace$ git push -u origin main
```
- ( 2023-09-05 10:51:42 )
```
jazzwang:~/git/dotnet-codespace$ code README.md
```
- Ref: https://gist.github.com/tianhaoz95/5bf47c416b4b641d83a2022f977a0ec0
- ( 2023-09-05 10:55:07 )
```
jazzwang:~/git/dotnet-codespace$ git add .
jazzwang:~/git/dotnet-codespace$ git commit -a
[main 75f344b] add `open in gitpod` to README.md
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
jazzwang:~/git/dotnet-codespace$ git push
```
- ( 2023-09-05 10:58:19 )
```
jazzwang:~/git/dotnet-codespace$ mkdir sbin; code sbin/install-dotnet
jazzwang:~/git/dotnet-codespace$ code sbin/enable-dotnet
jazzwang:~/git/dotnet-codespace$ git add sbin/.
jazzwang:~/git/dotnet-codespace$ git commit -a ; git push
```
- ( 2023-09-05 03:37:38 )
```
gitpod /workspace/dotnet-codespace (main) $ chmod a+x sbin/install-dotnet
gitpod /workspace/dotnet-codespace (main) $ sbin/install-dotnet
gitpod /workspace/dotnet-codespace (main) $ cat .gitconfig >> .git/config
gitpod /workspace/dotnet-codespace (main) $ cat >> .gitignore << EOF
# 2023-09-05 - ignore .dotnet runtime for gitpod
.dotnet
EOF
gitpod /workspace/dotnet-codespace (main) $ git commit -a ; git push
```

### Testing C# REPL

- ( 2023-09-04 22:03:16 )
- C# REPL Reference: https://dev.to/tallesl/c-repl-gkn
```
gitpod /workspace/dotnet-codespace (main) $ export HOME=$(pwd)
gitpod ~ (main) $ dotnet tool install -g dotnet-script

Welcome to .NET 6.0!
---------------------
SDK Version: 6.0.413

Telemetry
---------
The .NET tools collect usage data in order to help us improve your experience. It is collected by Microsoft and shared with the community. You can opt-out of telemetry by setting the DOTNET_CLI_TELEMETRY_OPTOUT environment variable to '1' or 'true' using your favorite shell.

Read more about .NET CLI Tools telemetry: https://aka.ms/dotnet-cli-telemetry

----------------
Installed an ASP.NET Core HTTPS development certificate.
To trust the certificate run 'dotnet dev-certs https --trust' (Windows and macOS only).
Learn about HTTPS: https://aka.ms/dotnet-https
----------------
Write your first app: https://aka.ms/dotnet-hello-world
Find out what's new: https://aka.ms/dotnet-whats-new
Explore documentation: https://aka.ms/dotnet-docs
Report issues and find source on GitHub: https://github.com/dotnet/core
Use 'dotnet --help' to see available commands or visit: https://aka.ms/dotnet-cli
--------------------------------------------------------------------------------------
Tools directory '/workspace/dotnet-codespace/.dotnet/tools' is not currently on the PATH environment variable.
If you are using bash, you can add it to your profile by running the following command:

cat << \EOF >> ~/.bash_profile
# Add .NET Core SDK tools
export PATH="$PATH:/workspace/dotnet-codespace/.dotnet/tools"
EOF

You can add it to the current session by running the following command:

export PATH="$PATH:/workspace/dotnet-codespace/.dotnet/tools"

You can invoke the tool using the following command: dotnet-script
Tool 'dotnet-script' (version '1.4.0') was successfully installed.
```
- ( 2023-09-05 05:03:33 )
```
```

### Building AWS Lambda Functions

- ( 2023-09-05 04:20:18 )
- Reference: https://docs.aws.amazon.com/lambda/latest/dg/lambda-csharp.html
