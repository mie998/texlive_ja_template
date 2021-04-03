# Easy latex editer with vscode, docker, and github actions!

## Quick Start
push 'use this template' button.
![template button](https://i.imgur.com/RTSRV8J.png)

## local container

1. Install VScode and open your project directory with VScode.
1. VScode recommend you reopen this project in container. Select 'Reopen in container'.
   ![github recommendation](https://i.imgur.com/VPUe1Jt.png)
1. It will take some time to open docker container for the first time due to docker image build.
1. Edit main.tex and save. main.pdf will automatically be compiled.
1. Feel free to edit latex document in docker container, without pc environmental pollution.

## git management

You can manage your tex files with git.
By default, locally created main.pdf will be excluded from git management.

## github actions

When you push revised tex file with git-tag, tex files will be automatically compiled with github-actions. It will take some times for this process.

## github release

You can check compiled main.pdf and diff.pdf with github-release. Git-tag by the name of 'vX.X.X' will create github-release and restore pdf files.
![check pdf files with github release](https://imgur.com/R56YasZ.png)
