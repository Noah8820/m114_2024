
# Daten Codieren NUM

## 1

| Dezimal | Hex   | Binär  | Binär  | Binär  | Binär  |
|---------|-------|--------|--------|--------|--------|
| 0       | 0     | 0      | 0      | 0      | 0      |
| 1       | 1     | 1      | 1      | 1      | 1      |
| 2       | 2     | 10     | 10     | 10     | 10     |
| 3       | 3     | 11     | 11     | 11     | 11     |
| 4       | 4     | 100    | 100    | 100    | 100    |
| 5       | 5     | 101    | 101    | 101    | 101    |
| 6       | 6     | 110    | 110    | 110    | 110    |
| 7       | 7     | 111    | 111    | 111    | 111    |
| 8       | 8     | 1000   | 1000   | 1000   | 1000   |
| 9       | 9     | 1001   | 1001   | 1001   | 1001   |
| 10      | A     | 1010   | 1010   | 1010   | 1010   |
| 11      | B     | 1011   | 1011   | 1011   | 1011   |
| 12      | C     | 1100   | 1100   | 1100   | 1100   |
| 13      | D     | 1101   | 1101   | 1101   | 1101   |
| 14      | E     | 1110   | 1110   | 1110   | 1110   |
| 15      | F     | 1111   | 1111   | 1111   | 1111   |

Die Binärzahlen in allen Spalten sind identisch.


## 2

Dezimal: 911 => Binär:  11 1000 1111

## 3

Binär: 1011 0110 => Dezimal: 182

## 4

Binär: 1110 0010 1010 0101 => Hexadezimal: E2A5

## 5

Binär: 1101 1001 + 0111 0101 = 1100 1110

(Das neunte Bit wird entfernt, da nur acht Bit verfügbar sind.)

## 6

a. Binär: 1100 0000 . 1010 1000 . 0100 1100 . 1101 0011 => Dezimal: **192.168.76.211** = IPv4-Adresse
b. Binär: 1011 1110 - 1000 0011- 1000 0101 - 1101 0101 1110 0100 - 1111 1110 => Hex:**BE-83-85-D5E4-FE** = MAC-Adresse


## 8

107 Gondeln => 110 1011 => Codebreite = 7

## 9

Speicherkapazität = (2 ^ 12 * 16) / (8 * 1024) = 8kiB

(1kiB = 1024B)

## 10

a. 1 MHz = 1 Million Takte pro Sekunde =>
   1 Million Bits pro Sekunde (bps) =>
   1 Million bps/8=125'000 Bytes pro Sekunde.

b. 1 MHz * 8 = 8 Millionen bps =>
   8 Millionen bps/8 = 1 Million Bytes pro Sekunde.

## 11

a. 0/255
b. -127/127
c. 0101 0011
d. 1101 0011
e. 1101 0011 + 0101 0011 = 1000 0000
f. 0000 0000 (Nein)
g. Dafür benötige ich die 8 Bits, wobei das höchstwertige Bit das Vorzeichenbit ist.


## 12

Ich würde die Zahl 0.3333333 als 3333333 speichern, mit E - 7.

## 13

a. Logisch UND/AND

| Eingang A | Eingang B | Ausgang |
|-----------|-----------|---------|
| 0         | 0         | 0       |
| 0         | 1         | 0       |
| 1         | 0         | 0       |
| 1         | 1         | 1       |

b. Logisch ODER/OR

| Eingang A | Eingang B | Ausgang |
|-----------|-----------|---------|
| 0         | 0         | 0       |
| 0         | 1         | 1       |
| 1         | 0         | 1       |
| 1         | 1         | 1       |

c. Logisch NICHT/NOT

| Eingang | Ausgang |
|---------|---------|
| 0       | 1       |
| 1       | 0       |

d. Logisch EXOR

| Eingang A | Eingang B | Ausgang |
|-----------|-----------|---------|
| 0         | 0         | 0       |
| 0         | 1         | 1       |
| 1         | 0         | 1       |
| 1         | 1         | 0       |

## 14

a. 11 % 2 = 1
b. 10 % 2 = 0
c. 10 % 3 = 1

# Daten kodieren Alphanum

## 1

### a

- Textsample1 = ANSI
- Textsample2 = UTF8
- Textsample3 = UTF16 BE BOM

### b

68

### c

- Textsample1 -> ANSI => 68 bytes = 1 Byte pro Zeichen

- Textsample2 -> UTF8 => 71 bytes 1 Byte pro ASCII-Zeichen + mehr als 1 Byte pro nicht ASCII-Zeichen

- Textsample3 -> UTF16 BE BOM => 138 bytes = 2 Bytes für die meisten Zeichen + 2 Bytes am Anfang für BOM

### d

ä, €

### e

BE (Big-Endian) = Das höchstwertigste Byte wird zuerst gespeichert oder übertragen.

LE (Little-Endian) = Das niederwertigste Byte wird zuerst gespeichert oder übertragen.

### f

Wenn die Datei ausschließlich ASCII-Zeichen enthält, ändert sich nichts, da diese mit UTF-8 identisch sind. Wenn jedoch Zeichen vorhanden sind, die nicht in ASCII vorkommen, aber in UTF-8, werden diese Zeichen nur korrekt in UTF-8 dargestellt.
