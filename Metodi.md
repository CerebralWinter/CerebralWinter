## oggetto document
document.write("Hello, world!"); //sconsigliato

## numeri

parseFloat("34acb") //restituisce 34.


parseInt("3eac34") //restituisce 3.


isNaN("123") //restituisce false o 0.


isNaN("abc") //restituisce true o 1.

## browser
prompt("Introdurre la temperatura in gradi Fahrenheit",100); //il secondo argomento è un valore di default

alert(" "); 

## stringhe
var t1 = new String ("TeStO");

var t2 = t1.toLowerCase() //restituisce "testo" 

var t3 = t1.toUpperCase() //Restituisce "TESTO" 
___

var testo = prompt("Inserisci un testo", "Hello, world!");


var primoCarattere = testo.charAt(0); //prima posizione


var quartoCarattere = testo.charAt(3); //quarta posizione


var ultimoCarattere = testo.charAt(testo.length - 1); //ultima posizione

___
var testo = "Hello, world!";

testo.charCodeAt(1); //mostra il codice ASCII del carattere "e", ovvero 101

___
``` javascript
var stringa;


for (codice = "0".charCodeAt(0); codice <= "9".charCodeAt(0); codice ++ )

 {
 stringa = stringa + String.fromCharCode(codice);
 }
``` 
___

var stringa = "Ma la volpe col suo balzo ha raggiunto il quieto fido" 

var posiz = stringa.indexOf("v"); //contiene il valore 6)


var posiz2 = stringa.indexOf("k"); // restituisce -1

___
var stringa = "Questo è un esempio";


var str2 = stringa.substr(0, 6); //restituisce "Questo"


var str3 = stringa.substr(7); //restituisce "è un esempio"

___
var s = "L'utente Pinco ha modificato questa pagina"


var s2 = s.replace("Pinco", "Pallino"); //s2 ora contiene "L'utente Pallino ha modificato questa pagina"