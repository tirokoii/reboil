## Telefon prövning

### Problem:
1. Kartans storlek skalades inte med websidan
2. Revolutinerande texten vart för nära bilden
3. Hero texten hade för mycket margin åt vänster / den hamnade för långt åt höger

### Fix

1. Skapa en klass (map) som hade display flex
2. Lägga till (.text) margin-top =  5ch till media taggen i about documentet
3. Lägga till en margin-left = 2ch till (.contetnt) media taggen i about style documenter / och sätta en !important till den 

## Wave Validatorn
### Summary
0 Errors

1 Contrast Error - redan känt

21 Alerts - 4 long alternative text, 14 possible headings, 1 device dependent event handler

5 Features

19 Structural Elements

0 ARIA

### Fix

Jag fixade inget.

Vet redan av vad som är contrast error på.
De långa texterna är med mening så att man kan se bildernas source
De possible heading är namnen på korten vilket jag inte planerar att ändra till headings
Device dependent event fungerar på min mobil. (Jag ser inte problemet)

## Validator
### Före
10 Errors - (Id button, fel end tag)

1 Fatal Error -Script tag inte i html tag

2 Warnings - (Id button)

### Efter
4 Errors - button, stray script

2 warnings - button id

### Fix
End tagar som var fel, script tagen i html tagen.

Jag ingnorerade script felet samt id button felet, eftersom det inte skapade några problem.
Felet med att span inte fick vara en child av ul sökte jag upp, man fick ha span som child av ul (och det skapar inget problem)



### Fix 2
Efter att ha validerat sidan igen så fixade jag script felet, vilket bara var att flytta up hela taggen från html till body. Jag ändrade även namnet button id'et till btn för att särskilja den från button taggen. 

Error och warning kring btn kvar står dock, den säger att jag har duplicate ID och noterar första occurences av btn ID'et. Men det är mycket lättare att ha ID'et på flera ställen än skriva flera separata ID'n, det gör det lättare att applicera java script på alla.

