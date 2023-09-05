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