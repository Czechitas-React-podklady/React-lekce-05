Založte si obyčejnou stránku s JavaScriptem, bez Webpacku i bez Reactu. Do souboru `index.js` si zkopírujte následující pole.

```js
const weekdays = [
  'pondělí',
  'úterý',
  'středa',
  'čtvrtek',
  'pátek',
  'sobota',
  'neděle',
];

const months = [
  {
    name: 'leden',
    days: 31,
  },
  {
    name: 'únor',
    days: 28,
  },
  {
    name: 'březen',
    days: 31,
  },
  {
    name: 'duben',
    days: 30,
  },
  {
    name: 'květen',
    days: 31,
  },
  {
    name: 'červen',
    days: 30,
  },
  {
    name: 'červenec',
    days: 31,
  },
  {
    name: 'srpen',
    days: 31,
  },
  {
    name: 'září',
    days: 30,
  },
  {
    name: 'říjen',
    days: 31,
  },
  {
    name: 'listopad',
    days: 30,
  },
  {
    name: 'prosinec',
    days: 31,
  },
];
```

Všechny body níže vyřešte pomocí metody `map`. Tam, kde je to možné, použijte zkrácený zápis pomocí arrow funkcí. Výsledky vypisujte do konzole pomocí `console.log`.

1.  Z pole `weekdays` vyrobte pole obsahující všechny názvy dnů napsané VELKÝMI PÍSMENY.
1.  Z pole `weekdays` vyrobte pole obsahující pouze první dvě písmena každého dne, tedy

    ```js
    ['po', 'út', 'st' /* atd. */];
    ```

1.  Z pole `months` vyrobte pole obsahující pouze počty dní v každém měsíci.
1.  Z pole `months` vyrobte pole obsahující pro každý měsíc datum jeho prvního dne v roce 2020, tedy
    ```js
    ['1. leden 2022', '1. únor 2022' /* atd. */];
    ```