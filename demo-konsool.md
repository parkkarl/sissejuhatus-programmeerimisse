# Live-demo konsoolis — kopeeri-kleebi snippetid

Hindamine nõuab, et **kõik mõisted on demonstreeritud reaalajas brauseri DevTools konsoolis**.
Ava brauser → vajuta **F12** → vali **Console** → kleebi alljärgnev rida-realt ja vajuta Enter.

> Soovitus: ava sama brauseri vahekaardil ka esitlus (`index.html`), ja teisel ekraanipoolel konsool.
> Iga slaidi juures kleebi vastav plokk ja näita tulemust.

---

## Andmetüübid
```js
let täisarv = 42;
let tekst = "Tere";
let tõene = true;
console.log(täisarv, tekst, tõene);
console.log(typeof täisarv, typeof tekst, typeof tõene);
```

## Muutujad
```js
let vanus = 18;
const PI = 3.14;
vanus = 19;
console.log(vanus, PI);
// PI = 4;   // proovi seda ka -> konsool annab vea "Assignment to constant variable"
```

## Tehted
```js
let a = 5, b = 2;
console.log(a + b, a / b, a % b);
console.log(5 > 3, 5 === 5, true && false);
```

## Tingimused
```js
let v = 17;
if (v >= 18) { console.log("Täisealine"); } else { console.log("Alaealine"); }
```

## Kordused
```js
for (let i = 0; i < 5; i++) { console.log("i = " + i); }

let x = 0;
while (x < 3) { console.log("x = " + x); x++; }
```

## Funktsioonid
```js
function tervita(nimi) { console.log("Tere, " + nimi + "!"); }
tervita("Mari");
tervita("Juhan");

const korrutaKahega = (x) => x * 2;
console.log(korrutaKahega(5));
```

## Massiivid
```js
let õpilased = ["Mari", "Juhan", "Kati"];
console.log(õpilased[0], õpilased.length);
for (let i = 0; i < õpilased.length; i++) { console.log(õpilased[i]); }
```

## Andmestruktuurid (objekt)
```js
let arvud = [1, 2, 3];
let inimene = { nimi: "Mari", vanus: 20 };
console.log(arvud);
console.log(inimene.nimi, inimene.vanus);
```

## Sisend ja väljund
```js
console.log("Tere maailm!");
alert("Hoiatusaken!");
let nimi = prompt("Sisesta oma nimi:");
console.log("Tere, " + nimi + "!");
```

## Klass
```js
class Auto {
  constructor(mark, aasta) { this.mark = mark; this.aasta = aasta; }
}
let auto = new Auto("Toyota", 2020);
console.log(auto);
console.log(auto.mark, auto.aasta);
```
