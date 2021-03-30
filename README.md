# Easy latex editer with vscode, docker, and github actions!

## Usage in private repository without template tags and commit logs.

```
$ git clone git@github.com:mie998/texlive_ja_template.git {new_repo_name} --no-tags --depth 1
$ gh repo create {new_repo_name} --private
```

these error message will be displayed, but just ignore it.  
`fatal: remote origin already exists. /usr/local/bin/git: exit status 128`

```
$ git remote set-url origin {new url}/{new_repo_name}.git
$ git push -u origin main
```

## local container

1. Install VScode and open this project directory with VScode.
1. VScode recommend you reopen this project in container. Select 'Reopen in container'.
   ![github recommendation](https://i.imgur.com/VPUe1Jt.png)
1. It will take some time to open docker container for the first time.
1. deit main.tex and save. main.pdf will automatically be compiled.
1. Boring installing of latex tools is never be needed!! Edit latex files with docker container.

## git management

You can manage your tex files with git.
By default, locally created main.pdf will be excluded from git management.

## github actions

When you push revised tex file with git-tag, it will be automatically compiled with github-actions. It will take some times for this process.

## github release

You can check compiled main.pdf and diff.pdf with github-release. Git-tag by the name of 'vX.X.X' will create github-release and restore pdf files.
![check pdf files with github release](https://imgur.com/R56YasZ.png)

# thanks

[ローカルでの docker を用いた latex 環境作成について参考にさせていだだきました。](https://korosuke613.hatenablog.com/entry/2019/06/24/171246)

[vscode の神拡張機能 latex-workshop の wiki](https://github.com/James-Yu/LaTeX-Workshop/wiki/)

[latex コンパイルのためのアクション。日本語対応はしていないかもしれない。](https://github.com/xu-cheng/latex-action)

[latexdiff-vc の man ページ。直前のコミットとの差分をとって diff.tex の作成までやってくれる優れもの。](https://www.mankier.com/1/latexdiff-vc)

[日本語環境での latex コンパイルをお任せしている action](https://3rdjcg.dev/ja/post/latex-github-action/)

[github release による asset 管理を参考にさせていただきました。](https://github.com/tsukuba-mas/platex-action)
