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
<p>apt update</p>
<p>apt install vim</p>
<p>apt install python3</p>

## Format json
<p>:%!python -m json.tool</p>

## Format xml
<p>apt install libxml2-utils</p>
<p>:%!xmllint --format -</p>

## Useful Vim Delete Command	Meaning
x	Delete character
dw	Delete word
dd	Delete line
D	Delete to end
d$	Delete to end of line
:%d	Delete all
di"	Delete inside quotes
u	Undo
ctrl+r Redo

