# `cedict` 漢英詞典 Go 軟件包

[![GoDoc](https://img.shields.io/badge/godoc-reference-blue.svg?style=flat-square)](https://godoc.org/github.com/Destaq/cedict)
[![Go Report Card](https://goreportcard.com/badge/github.com/Destaq/cedict?style=flat-square)](https://goreportcard.com/report/github.com/Destaq/cedict)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)

# Overview

Golang library for the community maintained Chinese-English dictionary (CC-CEDICT), published by MDBG.

> [https://www.mdbg.net/chinese/dictionary?page=cedict](https://www.mdbg.net/chinese/dictionary?page=cedict)

The basic format of a CEDICT entry is:

    Traditional Simplified [pin1 yin1] /American English equivalent 1/equivalent 2/
    漢字 汉字 [han4 zi4] /Chinese character/CL:個|个/

# Install

First grab the latest version of the package,

    go get -u github.com/Destaq/cedict

Next, include it in your application:

```go
import "github.com/Destaq/cedict"
```

# Getting Started

```go
d := cedict.New()
fmt.Printf("%s\n", cedict.PinyinTones(d.HanziToPinyin("你好，世界！")))
```

# Contributing

1. Fork the repo
2. Clone your fork (`git clone https://github.com/<username>/cedict && cd cedict`)
3. Create your own branch (`git checkout -b my-patch`)
4. Make changes and add them (`git add .`)
5. Commit your changes (`git commit -m 'Fixed #123'`)
6. Push to the branch (`git push origin my-patch`)
7. Create new pull request

## License

Copyright 2020 John Cramb. All rights reserved.

Licensed under the MIT License. See [LICENSE](https://github.com/Destaq/cedict/blob/master/LICENSE) in the project root for license information.
