

Commands für das Terminal :



// ALLGEMEINE VS CODE ABKÜRZUNGEN 

CLI - Command Line Interface, Eingabeaufforderung, in der du Befehle per Tastatur eintippst und ausführst, z.B. im VS Code Terminal.

pwd - Print Working Directory, zeigt den aktuellen Verzeichnis-Pfad im Terminal an.

ls - Listet alle Dateien und Ordner im aktuellen Verzeichnis auf (Linux/Mac), unter Windows dir.

cd - Change Directory, wechselt im Terminal in ein anderes Verzeichnis.

mkdir - Make Directory, erstellt einen neuen Ordner im aktuellen Pfad.

rm - Remove, löscht Dateien oder Ordner (unter Linux/Mac), unter Windows del oder rmdir.

pip - Python Package Installer, dient zur Installation und Verwaltung von Python-Paketen im Terminal.

git - Versionskontrollsystem, das Änderungen im Code verfolgt und Zusammenarbeit erleichtert.

npm - Node Package Manager, verwaltet JavaScript- und Node.js-Pakete und deren Abhängigkeiten.

venv - Virtual Environment, isolierte Python-Umgebung für Projekt-spezifische Paketinstallationen.

node - JavaScript-Laufzeitumgebung, mit der du JS außerhalb des Browsers ausführst, z.B. für Serveranwendungen.

code - Kommando, um Visual Studio Code aus dem Terminal zu öffnen oder Dateien zu laden.

taskkill - Windows-Befehl zum Beenden laufender Prozesse, z.B. um blockierte Programme zu schließen.

clear / cls - Löscht die Terminal-Ausgabe und schafft eine übersichtliche Arbeitsfläche.

exit - Beendet das Terminal oder die laufende Sitzung.



// ALLGEMEINE CODES VS CODE

code . - Öffnet den aktuellen Ordner im VS Code Editor.
code <Datei/Ordner> - Öffnet eine bestimmte Datei oder einen Ordner in VS Code.

python <datei>.py - Führt eine Python-Datei im Terminal aus.

pip install <paket> - Installiert ein Python-Paket im aktiven virtuellen Environment.

pip list - Zeigt alle installierten Python-Pakete mit Versionen an.

git status - Zeigt den aktuellen Status im Git-Repository an.

git add <datei> - Fügt Änderungen einer Datei zum nächsten Commit hinzu.

git commit -m "Nachricht" - Erstellt einen Commit mit einer Nachricht.

git push - Schiebt lokale Commits ins entfernte Git-Repository.

git pull - Holt Änderungen vom entfernten Repository und merged sie lokal.

code --install-extension <ext> - Installiert eine VS Code Extension über Terminal.

code --list-extensions - Listet alle installierten VS Code Extensions auf.

python -m venv .venv - Erstellt ein virtuelles Python-Environment im Ordner .venv.

.venv\Scripts\activate - Aktiviert das virtuelle Environment unter Windows.

deactivate - Deaktiviert das aktive virtuelle Environment.

cls / clear - Terminal-Konsole löschen (Windows: cls, Mac/Linux: clear).




// INSTALLATIONEN 

Selenium - Automatisiert Webbrowser (Klicks, Texteingabe, Navigation). Ideal für UI-Tests und Webautomatisierung.
pip install selenium - Installation
python -m selenium --version - Version prüfen

Cypress - Modernes JavaScript-Testframework, das im Browser läuft. Perfekt für schnelle und interaktive Webtests.
npm install cypress --save-dev - Installation
npx cypress --version - Version prüfen

Playwright - Browser-Automatisierung für Chromium, Firefox und WebKit. Unterstützt Mobile-Simulation und ist sehr stabil.
pip install playwright - Installation
playwright --version - Version prüfen

BeautifulSoup - HTML/XML Parser zum Auslesen von Webseitendaten. Einfaches Webscraping ohne API.
pip install beautifulsoup4 - Installation
Python:
import bs4
print(bs4.__version__) - Version prüfen

Requests - HTTP-Client, um Webseiten oder APIs anzufragen (GET, POST, etc.). Grundlage für Webscraping.
pip install requests - Installation
Python:
import requests
print(requests.__version__) - Version prüfen

Scrapy - Leistungsfähiges Framework für asynchrones Webscraping und Crawling großer Websites.
pip install scrapy - Installation
scrapy version - Version prüfen

language-tool-python - Python-Bindings für LanguageTool: Rechtschreib-, Grammatik- und Stilprüfungen, u.a. für Deutsch.
pip install language-tool-python - Installation
Python:
import language_tool_python
print(language_tool_python.__version__) - Version prüfen

spaCy - Schnelles NLP-Toolkit mit Tokenisierung, POS-Tagging und Named Entity Recognition. Deutsch verfügbar.
pip install spacy - Installation
Python:
import spacy
print(spacy.__version__) - Version prüfen

TextBlob-de - Einfache NLP-Bibliothek für deutschsprachige Textverarbeitung (POS, Sentiment).
pip install textblob-de - Installation
Python:
import textblob_de
print(textblob_de.__version__) - Version prüfen

pandas - DataFrame-basierte Bibliothek zur Datenanalyse und -verarbeitung. Standard in Data Science.
pip install pandas - Installation
Python:
import pandas as pd
print(pd.__version__) - Version prüfen

numpy - Bibliothek für numerische Berechnungen mit Arrays und Mathefunktionen.
pip install numpy - Installation
Python:
import numpy
print(numpy.__version__) - Version prüfen

openpyxl - Lesen und Schreiben von Excel-Dateien (.xlsx) in Python.
pip install openpyxl - Installation
Python:
import openpyxl
print(openpyxl.__version__) - Version prüfen

pytest - Flexibles Python-Testframework für Unit- und Integrationstests.
pip install pytest - Installation
pytest --version - Version prüfen

unittest - Eingebautes Python-Modul für Unit-Tests. Kein extra Install nötig.
(Standard in Python) - Version prüfen:
python -m unittest --version

tox - Führt Tests in verschiedenen Python-Versionen und Umgebungen automatisiert aus (CI/CD-Tool).
pip install tox - Installation
tox --version - Version prüfen

venv - Python-Standardtool für isolierte virtuelle Umgebungen.
(Standard ab Python 3.3) - Version prüfen:
python -m venv --help

virtualenv - Alternative virtuelle Umgebungen mit mehr Features, auch für ältere Python-Versionen.
pip install virtualenv - Installation
virtualenv --version - Version prüfen

black - Automatischer Code-Formatter für Python. Vereinheitlicht Stil und Layout.
pip install black - Installation
black --version - Version prüfen

flake8 - Tool zur statischen Codeanalyse: Syntax, Stil und Fehlerwarnungen.
pip install flake8 - Installation
flake8 --version - Version prüfen

mypy - Statischer Typprüfer für Python. Erkennt Typfehler vor der Laufzeit.
pip install mypy - Installation
mypy --version - Version prüfen