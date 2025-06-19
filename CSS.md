Übersicht 

color: red;                          - Textfarbe auf Rot setzen
background-color: lightblue;        - Hintergrundfarbe eines Elements setzen
font-size: 16px;                    - Schriftgröße auf 16 Pixel setzen
font-family: Arial, sans-serif;    - Schriftart festlegen
margin: 10px;                      - Außenabstand rundherum 10 Pixel
margin-top: 20px;                  - Außenabstand oben 20 Pixel
padding: 5px 10px;                 - Innenabstand oben/unten 5px, links/rechts 10px
border: 2px solid black;           - Schwarzer, 2px breiter, durchgehender Rahmen
border-radius: 8px;                - Abgerundete Ecken mit Radius 8px
width: 100%;                      - Breite 100% des Elternelements
height: 50px;                     - Höhe 50 Pixel
display: block;                   - Element als Block-Element darstellen
display: inline;                  - Element inline darstellen
display: flex;                    - Flexbox-Layout aktivieren
justify-content: center;          - Flexbox-Inhalt horizontal zentrieren
align-items: center;              - Flexbox-Inhalt vertikal zentrieren
position: relative;               - Position relativ zum normalen Fluss
position: absolute;               - Position relativ zum nächsten positionierten Vorfahren
top: 10px;                       - Abstand von oben 10 Pixel (bei position absolute/relative)
left: 20px;                      - Abstand von links 20 Pixel (bei position absolute/relative)
overflow: hidden;                - Überlaufenden Inhalt abschneiden
z-index: 10;                    - Stapelreihenfolge (höher = weiter vorne)
opacity: 0.5;                   - Transparenz 50%
text-align: center;             - Text zentrieren
line-height: 1.5;               - Zeilenhöhe auf 1.5 setzen
box-shadow: 2px 2px 5px gray;  - Schatten um das Element
cursor: pointer;                - Mauszeiger wird zur Hand beim Überfahren
visibility: hidden;             - Element bleibt im Layout, ist aber unsichtbar
float: left;                   - Element wird nach links ausgerichtet und Text fließt darum
clear: both;                   - Verhindert, dass Elemente neben gefloateten Elementen stehen
transition: all 0.3s ease;     - Sanfte Übergangseffekte bei Änderungen
transform: rotate(10deg);      - Element um 10 Grad drehen

/* Transform Eigenschaften */

    transform: translateX(50px);                 - Verschiebt das Element 50px nach rechts auf der X-Achse

    transform: translateY(-30px);                - Verschiebt das Element 30px nach oben auf der Y-Achse

    transform: scale(1.5);                       - Vergrößert das Element um das 1,5-fache (150%)

    transform: scaleX(2);                        - Vergrößert das Element nur horizontal doppelt

    transform: scaleY(0.5);                      - Verkleinert das Element nur vertikal auf die Hälfte

    transform: rotate(45deg);                    - Dreht das Element um 45 Grad im Uhrzeigersinn

    transform: skew(20deg, 10deg);               - Kipt das Element horizontal um 20 Grad und vertikal um 10 Grad



////* Animationen */

    @keyframes fadeIn {                         - Animation, die ein Element langsam einblendet
    from { opacity: 0; }                      - Start: komplett durchsichtig
    to { opacity: 1; }                        - Ende: komplett sichtbar
    }

animation: fadeIn 1s ease forwards;        - fadeIn 1 Sekunde, sanft, bleibt sichtbar

    @keyframes bounce {                         - Animation, die ein Element auf- und abprallen lässt
    0%, 100% { transform: translateY(0); }   - Anfang und Ende: normale Position
    50% { transform: translateY(-20px); }    - Mitte: 20px nach oben springen
    }

animation: bounce 0.7s infinite;            - Bounce in 0.7 Sekunden, unendlich wiederholen

    @keyframes rotate360 {                      - Volle 360° Drehung
    from { transform: rotate(0deg); }        - Start bei 0 Grad
    to { transform: rotate(360deg); }        - Ende bei 360 Grad (volle Drehung)
    }

animation: rotate360 2s linear infinite;    - Drehung 2 Sekunden linear und endlos

////* Pseudoklassen */
    a:hover {                                  - Styles für Link, wenn Maus darüber ist (Hover)
    color: green;                            - Textfarbe grün beim Hover
    }

    input:focus {                              - Styles wenn ein Eingabefeld aktiv/fokussiert ist
    border-color: blue;                      - Rahmenfarbe Blau bei Fokus
    }

////* Media Queries für responsive Design */
    @media (max-width: 600px) {                 - Abweichende Styles bei max. Bildschirmbreite 600px
    body { 
        background-color: lightgray;           - Hintergrundfarbe ändern auf hellgrau
    }
    nav { 
        display: none;                         - Navigation ausblenden bei kleinen Bildschirmen
    }
    }
