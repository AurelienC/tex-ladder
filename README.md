# Ladder TeX package
_This package permit the creation of simple ladder diagram into TeX documents._

[Example](https://github.com/AurelienC/tex-ladder/blob/master/ladder.pdf)

## Usage
The code must be inserted between en `tikzpicture` section.

Add the packages :
    \usepackage{tikz}
    \usepackage{ladder}



### Net
_All contacts and relays are, by default, added in series_
* `\ladderLine` begin a new ladder net
* `\startParallel` begin a parallel segment
* `\setParallel` begin the new parallel segment
* `\unsetParallel` end of the parallel segment

### Contacts
* `\ladderNO[type]{name}{mnemonic}` a Normally Opened contact 
* `\ladderNC[type]{name}{mnemonic}` a Normaly Closed contact
_Type may be P (rising edge), N (falling edge)..._

### Relays
* `\ladderc[type]{name}{mnemonic}` a relay
_Type may be R (reset), S (set)..._
