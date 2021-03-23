# Easy latex editer with vscode, docker, and github actions!

## local container
1. Install VScode and open this project directory with VScode.
1. VScode recommend you reopen this project in container, so check it.
1. It will take some time to open docker container for the first time.
1. deit main.tex and save. main.pdf will automatically be compiled.
1. Boring installing of latex tools is never be needed!! Edit latex files with docker container.

## git management
You can manage your files with git.
By default, locally created main.pdf will be excluded from git management.

## github actions
Pushed tex files will be automatically compiled with github-actions. It will take some times for this process (3~5 minutes).

## github release
You can check compiled main.pdf and diff.pdf with github-release. I Recommend you to use git tag to manage github-release.
![check pdf files with github release](https://imgur.com/R56YasZ)


# thanks
[ローカルでのdockerを用いたlatex環境作成について参考にさせていだだきました。](https://korosuke613.hatenablog.com/entry/2019/06/24/171246)

[vscodeの神拡張機能 latex-workshopのwiki](https://github.com/James-Yu/LaTeX-Workshop/wiki/)

[latex コンパイルのためのアクション。日本語対応はしていないかもしれない。](https://github.com/xu-cheng/latex-action)

[latexdiff-vcのmanページ。直前のコミットとの差分をとって diff.tex の作成までやってくれる優れもの。](https://www.mankier.com/1/latexdiff-vc)

[日本語環境でのlatexコンパイルをお任せしているaction](https://3rdjcg.dev/ja/post/latex-github-action/)

[github release による asset 管理を参考にさせていただきました。](https://github.com/tsukuba-mas/platex-action)
