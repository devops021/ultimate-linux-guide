Tutorial URL -
<br>
https://www.youtube.com/watch?v=29eDuMjsEF8
<br>
`mukul@ubuntu-server:~$` <br>
mukul        → Username<br>
@            → Separator<br>
ubuntu-server→ Hostname / IP<br>
:~           → Current directory<br>
$            → Normal user prompt<br>

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
x	→ Delete character<br>
dw	→ Delete word<br>
dd	→ Delete line<br>
D	→ Delete to end<br>
d$	→ Delete to end of line<br>
:%d	→ Delete all<br>
di"	→ Delete inside quotes<br>
u	→ Undo<br>
ctrl+r → Redo<br>
```
| Category        | Command       | Purpose                   |
| --------------- | ------------- | ------------------------- |
| Mode            | `Esc`         | Normal mode               |
| Left            | `h`           | Move left                 |
| Right           | `l`           | Move right                |
| Down            | `j`           | Move down                 |
| Up              | `k`           | Move up                   |
| Next Word       | `w`           | Jump next word            |
| Previous Word   | `b`           | Jump previous word        |
| End of Word     | `e`           | Move to word end          |
| Line Start      | `0`           | Beginning of line         |
| First Character | `^`           | First non-space character |
| Line End        | `$`           | End of line               |
| Top of File     | `gg`          | Go to top                 |
| Bottom of File  | `G`           | Go to bottom              |
| Specific Line   | `:25`         | Go to line 25             |
| Search          | `/text`       | Search text               |
| Next Match      | `n`           | Next search result        |
| Previous Match  | `N`           | Previous result           |
| Half Page Down  | `Ctrl+d`      | Scroll down               |
| Half Page Up    | `Ctrl+u`      | Scroll up                 |
| Full Page Down  | `Ctrl+f`      | Next page                 |
| Full Page Up    | `Ctrl+b`      | Previous page             |
| Match Bracket   | `%`           | Jump matching bracket     |
| Show Lines      | `:set number` | Line numbers              |
| Save            | `:w`          | Save file                 |
| Quit            | `:q`          | Quit                      |
| Save & Quit     | `:wq`         | Save and exit             |
| Force Quit      | `:q!`         | Exit without saving       |
| Undo            | `u`           | Undo                      |
| Redo            | `Ctrl+r`      | Redo                      |
| Delete Line     | `dd`          | Delete current line       |
| Delete Word     | `dw`          | Delete word               |
| Copy Line       | `yy`          | Copy line                 |
| Paste           | `p`           | Paste                     |
```
