# やりたいこと

## local docker container 
- dev Container 内では基本的にlatex-workshopを用いてコンパイルやpdfのビューイングを行うことになる。そのため、このwiki(https://github.com/James-Yu/LaTeX-Workshop/wiki/)が大変参考にできると思う

## github actions 
- https://3rdjcg.dev/ja/post/latex-github-action/　を参考にいい感じにコンパイルはうまく行ってそう。
- diff も latexdiff-vc を使うことでできてそう。
- artifact 上で pdf を確認することができないのは不便なのでそれだけできるようにしたい。
- build の終了を slack で通知して、pdf を slack に送信するようにしても面白いかも知れない。
