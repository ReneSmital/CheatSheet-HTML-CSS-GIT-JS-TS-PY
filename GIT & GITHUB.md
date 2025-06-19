GIT installieren

GUTHUB Account machen




////////// GIT ///////////


//NEUES PROJEKT SPEICHERN

git init
-> Version wird ausgespuckt,so checkt man obs klappt, passt

git add .
-> der punkt steht für ALLE Dateien werden geaddet, wenn man nur einzelne will, dann einfach Leerzeichen zwischen den filenames

git commit -m "first commit"
-> speichert local und gibt eine bezeichnung dafür

git branch -M main
-> ?? Ich vermute bestimmt eben den Branch , falls ich mehrere Branches habe

git remote add origin https://github.com/ReneSmital/TypeScript-CrashCourse-and-Notes.git
-> verbindet git mit der GitHub adresse , diese bekomme ich aus github selbst

git push -u origin main


//BESTEHENDES PROJEKT UPDATEN

git add .
-> speichert alles
git commit -m "hier schreibe ich was das update war"
-> speichert local mei update
git push





/////////GITHUB//////////

create new repository
-> commandlines werden angezeigt ( siehe oben )
-> einfach nachmachen , copy&paste




////// ein paar GIT flags :

-m	Commit-Nachricht direkt angeben
-M	Haupt-Branch umbenennen
-u	Remote-Tracking-Branch setzen
-v	Detaillierte Ausgabe („verbose“)
-a	Automatisch alle Änderungen adden
--amend	Letzten Commit bearbeiten
-f / --force	Push erzwingen (mit Gefahr)