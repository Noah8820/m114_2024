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

## 4. RLC

0 0 0 0 0 1 1 0  
1 1 1 1 1 1 1 0  
1 0 0 0 0 1 1 0  
0 0 0 0 1 0 0 0  
0 0 0 0 1 0 0 0  
0 0 0 0 1 0 0 0  
0 0 0 0 1 0 0 0  
0 0 0 0 1 0 1 1  

Grafik:

⬜⬜⬜⬜⬜⬛⬛⬜  
⬛⬛⬛⬛⬛⬛⬛⬜  
⬛⬜⬜⬜⬜⬛⬛⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬜⬜  
⬜⬜⬜⬜⬛⬜⬛⬛  
