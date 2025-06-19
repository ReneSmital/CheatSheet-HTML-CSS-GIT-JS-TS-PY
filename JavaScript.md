


// 💻 Variablen & Datentypen

let name = "Max";                  // Variable, änderbarer Wert  
const PI = 3.14;                   // Konstante, nicht änderbar  
var alter = 25;                    // Variable (ältere Variante)  
typeof name                       // Datentyp ermitteln (z.B. "string")  


// 🔢 Zahlen & Operatoren

let summe = 5 + 3;                // Addition  
let differenz = 10 - 4;           // Subtraktion  
let produkt = 2 * 3;              // Multiplikation  
let quotient = 10 / 2;            // Division  
let rest = 10 % 3;                // Modulo (Rest bei Division)  
x++;                             // Inkrement (x + 1)  
x--;                             // Dekrement (x - 1)  


// 📝 Strings (Text)

let text = "Hallo";               // String mit Doppel-Anführungszeichen  
let text2 = 'Welt';               // String mit einfachen Anführungszeichen  
let lang = text.length;           // Länge des Strings  
text.toUpperCase();               // String zu Großbuchstaben  
text.toLowerCase();               // String zu Kleinbuchstaben  
text.includes("ll");              // Prüfen ob Text Teilstring enthält (true/false)  


// 📋 Arrays (Listen)

let arr = [1, 2, 3, 4];           // Array erstellen  
arr.push(5);                     // Element ans Ende anhängen  
arr.pop();                       // Letztes Element entfernen  
arr.length;                      // Länge des Arrays  
arr.includes(3);                 // Prüfen ob Wert enthalten ist  
arr.indexOf(2);                  // Index eines Elements  
arr.concat([5,6]);               // Arrays zusammenfügen  


// 🔁 Schleifen

for (let i = 0; i < 5; i++) {     // for-Schleife  
  console.log(i);  
}


let i = 0;  
while (i < 5) {                   // while-Schleife  
  console.log(i);  
  i++;  
}

arr.forEach(element => {          // forEach Schleife für Arrays , Die forEach()-Schleife ist eine Methode für Arrays, mit der du eine Funktion für jedes Element im Array ausführst. 
                                    Sie ersetzt die klassische for-Schleife, wenn du nur über alle Elemente iterieren möchtest, ohne den Index manuell zu verwalten. Dabei bekommst du automatisch Zugriff auf das aktuelle Element (und optional den Index), was den Code oft klarer und kürzer macht.
  console.log(element);  
});

// 🔧 Funktionen
function begruessung(name) {       // Funktion definieren  
  return "Hallo " + name;  
}

let sum = function(a, b) {         // Funktion als Variable  
  return a + b;  
}

let quadriere = (x) => x * x;      // Arrow-Funktion (kurz)  

console.log(begruessung("Max"));   // Funktion aufrufen  


// ⚖️ Bedingungen

if (alter >= 18) {                 // if-Bedingung  
  console.log("Volljährig");  
} else if (alter > 13) {  
  console.log("Teenager");  
} else {  
  console.log("Kind");  
}


let ergebnis = (alter >= 18) ? "Erwachsen" : "Kind";   // Ternary Operator  ( Wenn DIES, dann SO, otherwise DAS)


// 🧩 Objekte

let person = {                    // Objekt mit Eigenschaften  
  name: "Anna",  
  alter: 30,  
  begruessung: function() {  
    return "Hallo " + this.name;  
  }  
};


console.log(person.name);         // Zugriff auf Eigenschaft  
console.log(person.begruessung()); // Methode aufrufen  


// 📚 Weitere wichtige Methoden

JSON.stringify(person);            // Objekt in JSON-String umwandeln  
JSON.parse('{"name":"Anna"}');    // JSON-String in Objekt umwandeln  
Math.random();                    // Zufallszahl zwischen 0 und 1  
Math.floor(3.7);                 // Rundung nach unten  
parseInt("123");                 // String in Ganzzahl umwandeln  
parseFloat("3.14");              // String in Gleitkommazahl umwandeln  


// ⏳ Asynchrone Programmierung

setTimeout(() => {  
  console.log("Nach 2 Sekunden");  
}, 2000);                         // Verzögerung  

fetch("https://api.example.com")   // HTTP Request (API abrufen)  
  .then(response => response.json())  
  .then(data => console.log(data));  

async function ladeDaten() {  
  let response = await fetch("https://api.example.com");  
  let data = await response.json();  
  console.log(data);  
}


// 🛠️ Module & Import (modern)

// export.js  
// export function hallo() {  
//   console.log("Hallo Modul!");  
// }

// main.js  
// import { hallo } from './export.js';  
// hallo();  

