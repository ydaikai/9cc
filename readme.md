# Dockerを利用した開発環境の構築
MacOSを利用していてM1以降のチップを利用している場合は、Dockerを利用してx86_64のLinux環境下でテスト等を行う必要がある. 以下のページを参考にDocker環境の構築をすることでうまく動くようになる。

`docker build -t compilerbook_x86_64 https://www.sigbus.info/compilerbook/Dockerfile  --platform linux/amd64`
`docker run --rm -it -v to_9cc_directory/9cc:/9cc -w /9cc compilerbook_x86_64`

[参考サイト](https://sbite.hatenablog.com/entry/2021/04/21/222225)