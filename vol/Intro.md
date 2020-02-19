# Volatility
> [Volatility Framework](https://github.com/volatilityfoundation/volatility) 
- Pythonで書かれたメモリアナライズツール
 
## Installation
- Download
```
$ git clone https://github.com/volatilityfoundation/volatility.git
```

- dependencies(依存パッケージ)
```
$ apt install pcregrep libpcre++-dev python-dev -y
```

## About
- 基本的に"正常な状態"のメモリ状態を把握していないと使えない
    - winword.exeの子プロセスにrundll32やpowershellが呼ばれている→不審 といった感じ
    - OS別のメモリ構造の把握も必要
        - 親から呼ばれがちな子プロセスとか
- Yaraルール適用させるのであればマルウェアの特徴的なStringsなどの知識理解も必要
    - xxmmやsodinokibiみたいな特徴的なStringsがあれば良いが、そうでない場合は大変

## How to use
1. GitHubのWikiを見よう！！！！
> https://github.com/volatilityfoundation/volatility/wiki/Installation
