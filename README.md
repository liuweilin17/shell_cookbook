# shell_cookbook

## std
1: stdout
2: stderr
2>&1: redirect stderr to stdout. `&` is used to mark `1` is the stdout rather than a new file named `1`
Ex: find `logs` dir and does show the `Permission denied` error message
```
find . -name "logs" 2>&1 | grep -v "Permission denied"
```   