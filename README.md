<h1 align="center">Welcome to go2ast 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
  <a href="https://twitter.com/reflog" target="_blank">
    <img alt="Twitter: reflog" src="https://img.shields.io/twitter/follow/reflog.svg?style=social" />
  </a>
</p>

> Transform Go code into it's AST

## Usage

```sh
echo &#34;a := 1&#34; | go run main.go
```

## Example output
```go
[]ast.Stmt {
        &ast.AssignStmt {
                Lhs: []ast.Expr {
                        &ast.Ident {
                                Name: "a",
                        },
                },
                Tok: :=,
                Rhs: []ast.Expr {
                        &ast.BasicLit {
                                ValuePos: 30,
                                Kind: INT,
                                Value: "1",
                        },
                },
        },
}

```

## Author

👤 **Eli Yukelzon**

* Twitter: [@reflog](https://twitter.com/reflog)
* Github: [@reflog](https://github.com/reflog)
