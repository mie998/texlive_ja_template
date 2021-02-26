# やりたいこと

## local docker container 
- https://github.com/korosuke613/texlive-ja-devcontainer-template を参考にしつつ、不要ファイルなどを /build 以下にまとめるなどの工夫を行うこと
- dev Container 内では基本的にlatex-workshopを用いてコンパイルやpdfのビューイングを行うことになる。そのため、このwiki(https://github.com/James-Yu/LaTeX-Workshop/wiki/)が大変参考にできると思う。

## github actions 
- push 時に以前の tex との差分をとって自動的に diff.pdf を作成したい。
- build の終了を slack で通知して、pdf を slack に送信するようにしても面白いかも知れない。
- https://github.com/tawalaya/latex-diff-action 求めるものってこれじゃない？
