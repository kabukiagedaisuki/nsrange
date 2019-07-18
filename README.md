nsrange
====
`nsrange` enable expand number and string enclosed in brackets.

## Usage
```
$ nsrange [options] STRING
```
options

* **-f, --filename=FILENAME**

    read the file

* **-v, --version**<br>

    output version

* **--help**

    output usage

## Example

| command | output |
|---------|--------|
| `nsrange hoge[0-2]` | hoge0<br>hoge1<br>hoge2 |
| `nsrange hoge[00-10]` | hoge00<br>hoge01<br>...<br>hoge10 |
| `nsrange hoge[135]` | hoge1<br>hoge3<br>hoge5 |
| `nsrange hoge[11,22,33]` | hoge11<br>hoge22<br>hoge33 |
| `nsrange hoge[00-10,99]` | hoge00<br>hoge02<br>...<br>hoge10<br>hoge99 |
| `nsrange hoge01[a-c]` | hoge01a<br>hoge01b<br>hoge01c |
| `nsrange hoge0[1-3][ac]` | hoge01a<br>hoge01c<br>hoge02a<br>...<br>hoge03c |
| `nsrange hoge01.[net,co.jp,com]` | hoge01.net<br>hoge01.co.jp<br>hoge01.com |

