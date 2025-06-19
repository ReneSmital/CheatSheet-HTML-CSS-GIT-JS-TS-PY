# 🐍 Variablen & Datentypen
x = 5                                   - Ganze Zahl (Integer) zuweisen
name = "Anna"                          - String (Text) zuweisen, immer in Anführungszeichen
pi = 3.14                             - Dezimalzahl (Float) zuweisen
is_active = True                      - Boolean, Wahrheitswert (True/False)
my_list = [1, 2, 3, 4]               - Liste, eine geordnete, veränderbare Sammlung von Werten
my_tuple = (1, 2, 3)                 - Tuple, eine geordnete, unveränderbare Sammlung
my_dict = {"name": "Anna", "age": 25} - Dictionary, Sammlung von Schlüssel-Wert-Paaren

# 🔄 Schleifen
for i in range(5):                    - For-Schleife, läuft von 0 bis 4 (range exklusiv oben)
    print(i)                         - Ausgabe der Zahlen 0 bis 4
while x > 0:                         - While-Schleife läuft solange Bedingung True ist
    x -= 1                          - Verringere x um 1

# 🔢 Bedingungen
if x > 10:                          - Wenn x größer als 10 ist
    print("Groß")                   - dann Ausgabe „Groß“
elif x == 10:                      - sonst, wenn x genau 10 ist
    print("Genau 10")               - Ausgabe „Genau 10“
else:                              - sonst
    print("Klein")                  - Ausgabe „Klein“

# 🧩 Funktionen
def begruessung(name):              - Definiert eine Funktion mit Parameter „name“
    return "Hallo " + name          - Funktion gibt Begrüßung als String zurück
print(begruessung("Anna"))          - Ruft Funktion auf und gibt Ergebnis aus

# 📚 Listen-Methoden
my_list.append(5)                   - Fügt Element 5 am Ende der Liste hinzu
my_list.remove(2)                   - Entfernt erstes Vorkommen von 2 aus der Liste
my_list.pop()                      - Entfernt letztes Element und gibt es zurück
len(my_list)                       - Gibt Anzahl der Elemente in Liste zurück

# 🧮 Mathematische Operationen
a = 10 + 5                        - Addition: Ergebnis 15
b = 10 - 5                        - Subtraktion: Ergebnis 5
c = 10 * 5                        - Multiplikation: Ergebnis 50
d = 10 / 5                        - Division: Ergebnis 2.0 (Float)
e = 10 // 3                      - Ganzzahl-Division: Ergebnis 3
f = 10 % 3                       - Modulo (Rest): Ergebnis 1
g = 2 ** 3                       - Exponentiation (2 hoch 3): Ergebnis 8

# 📦 Importieren von Modulen
import math                      - Importiert das Modul für Mathematikfunktionen
print(math.sqrt(16))             - Gibt Quadratwurzel von 16 aus (4.0)
from random import randint       - Importiert nur die Funktion randint aus Modul random
print(randint(1, 10))            - Gibt eine Zufallszahl von 1 bis 10 aus

# 🐍 String-Methoden
text = "hallo welt"
print(text.upper())              - Gibt String in Großbuchstaben zurück: "HALLO WELT"
print(text.capitalize())         - Macht ersten Buchstaben groß: "Hallo welt"
print(text.replace("welt", "Python")) - Ersetzt „welt“ durch „Python“

# 📥 Benutzereingabe
name = input("Wie heißt du? ")   - Fragt Benutzer nach Eingabe und speichert sie als String
print("Hallo, " + name)          - Begrüßt den Benutzer mit dem eingegebenen Namen

# 🚫 Fehlerbehandlung
try:                             - Versucht den folgenden Codeblock auszuführen
    zahl = int(input("Gib eine Zahl ein: "))
    print(10 / zahl)
except ZeroDivisionError:        - Wenn Division durch Null, wird folgender Block ausgeführt
    print("Teilung durch Null nicht möglich!")
except ValueError:               - Wenn Eingabe keine Zahl, wird folgender Block ausgeführt
    print("Das war keine gültige Zahl!")

# 🐍 Klassen und Objekte (OOP)
class Person:                   - Definition einer Klasse Person
    def __init__(self, name, age):   - Konstruktor: initialisiert neue Person mit Name und Alter
        self.name = name
        self.age = age

    def begruessung(self):          - Methode für Begrüßung
        return f"Hallo, mein Name ist {self.name} und ich bin {self.age} Jahre alt."

p1 = Person("Anna", 25)           - Erzeugt Objekt der Klasse Person
print(p1.begruessung())            - Gibt Begrüßung der Person aus

# 🧵 Listen-Komprehension
quad = [x**2 for x in range(5)]   - Erzeugt Liste mit Quadratzahlen von 0 bis 4: [0,1,4,9,16]

# 🔄 Iterieren über Dictionary
for key, value in my_dict.items(): - Schleife über Schlüssel und Werte eines Dictionaries
    print(f"{key}: {value}")       - Ausgabe von Schlüssel und Wert

# 📊 Typprüfung
print(type(name))                 - Gibt Datentyp der Variablen zurück (z.B. <class 'str'>)

# 🛠 Nützliche Built-in Funktionen
sorted([3, 1, 2])                - Sortiert Liste und gibt neue sortierte Liste zurück
enumerate(["a", "b", "c"])       - Gibt Index und Wert als Tupel beim Iterieren zurück

# ⏳ Zeitverzögerung
import time
time.sleep(2)                    - Pausiert Programm für 2 Sekunden

# 🔧 Dateioperationen
with open("datei.txt", "r") as file:  - Öffnet Datei zum Lesen (r) im Kontext-Manager
    inhalt = file.read()              - Liest gesamten Inhalt der Datei
print(inhalt)

with open("datei.txt", "w") as file:  - Öffnet Datei zum Schreiben (w) und überschreibt Inhalt
    file.write("Hallo Welt!")         - Schreibt Text in Datei

# 💡 Lambda-Funktionen (anonyme Funktionen)
add = lambda x, y: x + y           - Definiert kleine Funktion, die zwei Zahlen addiert
print(add(3, 5))                   - Ausgabe: 8
