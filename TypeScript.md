
TypeScript ist eine von Microsoft entwickelte Programmiersprache, die auf JavaScript aufbaut und diesem statische Typisierung 
hinzufügt, also Typen für Variablen, Funktionen und Objekte definiert. Es erweitert JavaScript um Features wie Interfaces, 
Klassen und Typprüfungen schon beim Schreiben des Codes, was Fehler frühzeitig verhindert. TypeScript wird letztlich in normales 
JavaScript kompiliert, sodass es in allen Umgebungen läuft, die auch JavaScript unterstützen.

// 🚀 Grundsyntax & Variablen

// Variablen werden mit Typen deklariert, z.B. string, number, boolean
let name: string = "Rene";                 - Variable mit Typ String definieren
const age: number = 30;                    - Konstante mit Typ Number definieren
let isStudent: boolean = true;             - Boolean Variable (true/false)
let anyVar: any = 5;                       - Variable ohne festen Typ (dynamisch)
let unknownVar: unknown = "Hallo";          - Variable mit unbekanntem Typ (strenger als any)



// 📦 Funktionen & Typen

// Funktionen haben Eingabeparameter und Rückgabewerte mit Typen
function greet(name: string): string {      
  return "Hallo " + name;                   - Funktion mit Parameter- und Rückgabetypen
}

const add = (a: number, b: number): number => a + b;  - Arrow-Funktion mit Typen

function printMessage(message?: string): void {         - Optionaler Parameter (message kann fehlen)
  console.log(message || "Keine Nachricht");
}



// 🧩 Interfaces & Typ-Definitionen

// Interfaces beschreiben die Form von Objekten mit festgelegten Typen
interface Person {
  name: string;
  age: number;
  isStudent?: boolean;                      - Optionales Feld (kann fehlen)
}

const person: Person = {
  name: "Anna",
  age: 25
};



// 🗂️ Arrays & Tuples

// Arrays sind Listen von Werten eines Typs, Tuples sind feste Listen mit verschiedenen Typen
let numbers: number[] = [1, 2, 3, 4];        - Array aus Zahlen
let names: Array<string> = ["Rene", "Anna"]; - Alternative Array-Schreibweise
let tuple: [string, number] = ["Rene", 30];  - Tuple mit festem Typ und Länge



// 🌀 Klassen & Objekte

// Klassen sind Baupläne für Objekte mit Eigenschaften und Methoden
class Student {
  name: string;
  age: number;

  constructor(name: string, age: number) {
    this.name = name;
    this.age = age;
  }

  greet(): string {
    return `Hallo, ich heiße ${this.name} und bin ${this.age} Jahre alt.`;
  }
}

const student = new Student("Lena", 22);



// 🔄 Enums

// Enums sind Aufzählungstypen, die eine Gruppe von benannten Konstanten darstellen
enum Color {
  Red,
  Green,
  Blue
}

let favColor: Color = Color.Green;

// 🔧 Type Assertions (Type Casting)
// Erzwingt den Typ eines Werts, z.B. wenn TypeScript nicht automatisch ableiten kann
let someValue: any = "Das ist ein Text";
let strLength: number = (someValue as string).length;



// 🔍 Union Types & Type Guards

// Variablen können mehr als einen Typ haben (Union Types), Type Guards helfen bei Typunterscheidung
let id: number | string = 123;

function printId(id: number | string) {
  if (typeof id === "string") {
    console.log("ID als String: " + id.toUpperCase());
  } else {
    console.log("ID als Zahl: " + id);
  }
}



// 🎯 Generics

// Generische Typen ermöglichen wiederverwendbare Funktionen/Klassen für verschiedene Typen
function identity<T>(arg: T): T {
  return arg;
}

let output = identity<string>("Hallo");



// 🛠️ Utility Types (Beispiele)

// Eingebaute Typen, die existierende Typen abwandeln (optional, readonly, etc.)
type PartialPerson = Partial<Person>;       - Alle Felder optional
type ReadonlyPerson = Readonly<Person>;     - Alle Felder readonly (nicht änderbar)



// 📜 Module & Exports (kurz)

// Code wird in Module unterteilt und kann exportiert/importiert werden
export function helper() { /* ... */ }             - Funktion exportieren
import { helper } from "./helper";                   - Funktion importieren
