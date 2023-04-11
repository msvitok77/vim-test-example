# How to reproduce
In neovim go to line 13 and run: `:TestNearest<cr>` you're gonna get this result:
```
testing: warning: no tests to run
PASS
ok      simplesuite     0.003s [no tests to run]

[Process exited 0]
```

When you open the terminal and run:
`go test -timeout 30s -run ^TestExampleTestSuite$ -testify.m ^(TestList)$ simplesuite`
you're gonna get this result:

```
PASS
ok      simplesuite     0.004s
```

