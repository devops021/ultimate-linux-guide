Tutorial URL -
https://www.youtube.com/watch?v=29eDuMjsEF8

mukul@ubuntu-server:~$

+---------+---+----------------+------+------+
| Username| @ | Hostname / IP  | Path | Sign |
+---------+---+----------------+------+------+
| mukul   | @ | ubuntu-server  | :~   |  $   |
+---------+---+----------------+------+------+

mukul        → Username
@            → Separator
ubuntu-server→ Hostname / IP
:~           → Current directory
$            → Normal user prompt

## First time linux setup
apt update

apt install vim
apt install python3

## Format json
:%!python -m json.tool

## Format xml
apt install libxml2-utils
:%!xmllint --format -
