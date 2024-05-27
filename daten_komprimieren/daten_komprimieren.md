# Daten Komprimieren ANNEX

## 1. Huffman-Algorithmus

Dateisysteme haben ebenfalls eine Baumstruktur.

In einem binären Baum hat jeder Knoten höchstens zwei Kinder. Bei nicht-binären Bäumen gibt es diese Begrenzung nicht, sodass ein Knoten beliebig viele Kinder haben kann.

## 2. Huffman-Algorithmus

![image](https://github.com/Noah8820/m114_2024/assets/113603845/011b031d-585f-4f4d-ac5c-591791907e9e)

## 3. RLC

Mit 5 Bit kann man eine Pixelreihe eines Bildes darstellen. Wäre es 1 Bit oder kein Bit, könnte man einfach die Farbe angeben.

Beispiele:

10100 Gelb
1011 Gelb, 10 Schwarz, 111 Gelb
Weitere Beispiele:

10100 Blau
1011 Blau, 1 Rot, 1 Schwarz, 111 Blau
100 Blau, 10 Rot, 1 Schwarz, 10 Blau, 101 Rot, 1 Schwarz, 5 Blau
Und schließlich:

1 Blau

## 4. RLC:  
Sie erhalten diesen RL-Code: 010100011110010010010010010010010010010110010110010010010010010010010010001 

```
010 100 011 110 010 010 010 010 010 010 010 010 010 110 010 110 010 010 010 010 010 010 010 010 001
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 2   4   3   6   2   2   2   2   2   2   2   2   2   6   2   6   2   2   2   2   2   2   2   2   1
 |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
 W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W   S   W

WWSSSSWW
WSSSSSSW
WSSWWSSW
WSSWWSSW
WSSSSSSW
WSSSSSSW
WSSWWSSW
WSSWWSSW


  XXXX
 XXXXXX
 XX  XX
 XX  XX
 XXXXXX
 XXXXXX
 XX  XX
 XX  XX
```

Es wird ein 'A' dargestellt.


### 5. LZW-Verfahren

#### a. 

| Zeichenkette | Gefunden | Gespeichert | Eintrag | Nummer |
| ------------ | -------- | ----------- | ------- | ------ |
| ananas       | a        | a           | an      | 256    |
| nanas        | n        | n           | na      | 257    |
| anas         | a        | 256         | ana     | 258    |
| as           | a        | a           | as      | -      |

ANANAS = an256as

#### b. 

| Zeichenkette  | Gefunden | Ausgabe | Eintrag | Nummer |
| ------------- | -------- | ------- | ------- | ------ |
| erdbe256kl260 | e        | e       | -       | -      |
| rdbe256kl260  | r        | r       | er      | 256    |
| dbe256kl260   | d        | d       | rd      | 257    |
| be256kl260    | b        | b       | db      | 258    |
| e256kl260     | e        | e       | be      | 259    |
| 256kl260      | e        | er      | ee      | 260    |
| kl260         | k        | k       | ek      | 261    |
| l260          | l        | l       | kl      | 262    |
| 260           | e        | ee      | le      | 263    |

erdbe256kl260 = erdbeerdklee


### 8

#### Weitere Verfahren zur verlustlosen Komprimierung 
- Huffman-Codierung 
- Lempel-Ziv-Welch (LZW) 
- Deflate 
- Burrows-Wheeler-Transformation (BWT) 
- Run-Length Encoding (RLE)
 
#### Daten, die verlustlos komprimiert werden sollten 
- Textdateien  
- Quellcode 
- Datenbanken 
- Wichtige Dokumente 
- Medizinische Bilder

#### Auswirkungen verlustbehafteter Komprimierung auf Briefe oder Java-Sourcecode  

- Briefe: Unleserlich oder missverständliche Informationen. 
- Java-Sourcecode: Unbrauchbarer Code, Kompilierungsfehler, fehlerhafte Ausführung. 

