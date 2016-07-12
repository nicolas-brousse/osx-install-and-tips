---
layout: page
title: Generic and useful commands
---

```bash
$ dscacheutil -flushcache
$ sudo killall -HUP mDNSResponder
```


## VoiceOver

```bash
$ say -f <textfile> -o <outputfile> -v <voice>
$ say -f input.txt -o output.aiff -v alex
```


## Apple defaults

### Screecapture

```bash
$ defaults write com.apple.screencapture location ~/Pictures
```

## Checksum

### shasum

```bash
$ shasum -a 512 /path/to/file
```


## Show/Hide file/folder in the Finder

```bash
# Hide
$ setfile -a V testfile.txt
# Show
$ setfile -a v testfile.txt
```


## Speed test

```bash
$ wget -O /dev/null http://ping.online.net/1Mo.dat # 1Mo
$ wget -O /dev/null http://ping.online.net/100Mo.dat # 100Mo
$ wget -O /dev/null http://ping.online.net/1000Mo.dat # 1Go
```


## Get mime type

```bash
$ file --mime /path/to/file.txt
```

## Diff

```bash
# Between two files
$ diff file-1 file-2

# Between two folders
$ diff -rq folder-1 folder-2
```


## Search and replace into a file

```bash
$ perl -p -i -e 's/oldstring/newstring/g' to_file.txt
```

## Count lines in a file

```bash
$ wc -l file.txt
```

