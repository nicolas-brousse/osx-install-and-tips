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


## Checksum

*shasum*

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
wget -O /dev/null http://speedtest.wdc01.softlayer.com/downloads/test10.zip

wget -O /dev/null http://ipv6.intuxication.testdebit.info/fichiers/1Mo.dat # 1Mo
wget -O /dev/null http://ipv6.intuxication.testdebit.info/fichiers/100Mo.dat # 100Mo
wget -O /dev/null http://ipv6.intuxication.testdebit.info/fichiers/1000Mo.dat # 1Go
```
