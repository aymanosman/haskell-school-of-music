# haskell-school-of-music

# Getting Started

First install [stack](https://docs.haskellstack.org/en/stable/README/)

then

```
shell> stack ghci

ghci> import Euterpea
ghci> play $ c 4 qn
```

# Troubleshooting

- (macosx) If you see error messages installing `PortMidi` mentioning `gcc`, make sure you are using xcode's version of `gcc` (which is really `clang`).

On my system, I had:

``` sh
> which -a gcc
/usr/local/bin/gcc # <- installed by homebrew
/usr/bin/gcc       # <- system gcc

> /usr/bin/gcc --version
Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/usr/include/c++/4.2.1
Apple LLVM version 10.0.0 (clang-1000.11.45.5)
Target: x86_64-apple-darwin17.7.0
Thread model: posix
InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
```

