## test
Exit with the status determined by EXPRESSION. Mostly used with `if`.
```shell
test EXPRESSION
```

```shell
if ! test -f /path/to/file; then
  echo "File does not exist."
fi
```
same as
```shell
if ! [ -f /path/to/file ]; then
  echo "File does not exist."
fi
```


