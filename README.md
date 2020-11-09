# shell_cookbook

## 1. shell
### output
1: stdout
2: stderr
2>&1: redirect stderr to stdout. `&` is used to mark `1` is the stdout rather than a new file named `1`
Ex: find `logs` dir and does show the `Permission denied` error message
```
find . -name "logs" 2>&1 | grep -v "Permission denied"
```
### tips
```shell
ctrl + r # search historical cmds
ctrl + u # clear current cmds
```

## 2. grep
```
grep -v # excluding pattern
grep -B 4 # before 4 lines
grep -A 4 # after 4 lines
grep -C 4 # == grep -A 4 -B 4
```

## 3. zgrep
grep in zipped file

## 4. Vim
```
:%s/pattern//ng # show number of appearances
```