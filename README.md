## Usage

```sh-session
$ cat source.txt
foo${bar}baz
foo$${bar}baz

$ cat vars.txt
# replace `${bar}` with `qux`
bar = qux

$ ./replace source.txt vars.txt
fooquxbaz
foo${bar}baz
```
