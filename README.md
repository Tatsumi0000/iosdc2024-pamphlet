
# iosdc2024-pamphlet

[iOSDC2024](https://iosdc.jp/2024/)のパンフレットを書くために、[korosuke613/texlive-ja-devcontainer-template](https://github.com/korosuke613/texlive-ja-devcontainer-template)をもとに最新のVS Codeのdevcontainerで動くようにしたリポジトリです。

# texlive-ja-devcontainer-template

VS Code Remote Developmentの機能を用いて、LaTeX環境を容易に構築するサンプルコードです。



Dockerイメージは、[iosdc2024-pamphlet/texlive-ja](https://github.com/Tatsumi0000/iosdc2024-pamphlet/pkgs/container/iosdc2024-pamphlet%2Ftexlive-ja)を利用しています。

(**Dockerが必要です**)

## setup

1. `git clone https://github.com/Tatsumi0000/iosdc2024-pamphlet.git`
2. VS Codeで`iosdc2024-pamphlet`を開く。
3. 拡張機能[Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)を追加する。
4. 左下の`><`アイコンを押して、`Rebuild Container`を実行する。
5. 待つ。
6. ワークスペースが開いたら、terminalを開き、`latexmk iosdc2024.tex`を実行する。
7. 上手くコンパイルできたらsetup完了！

## build

```bash
latexmk iosdc2024.tex
```

`iosdc2024.pdf`という実行ファイルができているはず。