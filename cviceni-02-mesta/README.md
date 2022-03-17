# Cvičení 2 - Česká města

Vytvoř aplikaci, která bude zobrazovat seznam všech českých měst.

1. Známým postupem si založ nový React projekt pomocí `create-czechitas-app` a nazvi ho třeba `ceska-mesta`.

2. Do hlavního souboru `index.jsx` vlož mimo komponentu `App` pole s názvy deseti největších českých měst:

	```js
	const cities = [
		'Praha',
		'Brno',
		'Ostrava',
		'Plzeň',
		'Liberec',
		'Olomouc',
		'České Budějovice',
		'Hradec Králové',
		'Ústí nad Labem',
		'Pardubice',
	];
	```

3. V samostatné složce vytvoř komponentu `City`, která se bude starat o zobrazování jednoho města. Komponenta zatím bude mít pouze jednu `prop` s názvem `name`, pomocí které budeme do komponenty předávat název města.

	Komponeta zatím bude generovat jen velmi jednoduchý kód:

	```jsx
	<div className="city">Název města</div>
	```

4. Uvnitř hlavní komponenty `App` přemapuj pole měst na pole komponent `City`, do kterých vždy předáš název města.

5. React bude v konzoli prohlížeče fňukat, že mu chybí prop `key`. Jako klíč použij znovu název města. Co také jiného, když je to zatím jediná věc, kterou o našem městě víme, že ano?

6. Zkusme projekt vylepšit o další data. Naše pole měst nazvané `cities` přepišme třeba takto:

	```js
	const cities = [
		{
			name: 'Praha',
			population: 1324277,
			area: 496.21,
		},
		{
			name: 'Brno',
			population: 381346,
			area: 230.18,
		},
		{
			name: 'Ostrava',
			population: 287968,
			area: 214.23,
		},
		{
			name: 'Plzeň',
			population: 174842,
			area: 137.67,
		},
		{
			name: 'Liberec',
			population: 104802,
			area: 106.09,
		},
		{
			name: 'Olomouc',
			population: 100663,
			area: 103.33,
		},
		{
			name: 'České Budějovice',
			population: 94463,
			area: 55.6,
		},
		{
			name: 'Hradec Králové',
			population: 92939,
			area: 105.69,
		},
		{
			name: 'Ústí nad Labem',
			population: 92716,
			area: 93.97,
		},
		{
			name: 'Pardubice',
			population: 91727,
			area: 82.66,
		},
	];
	```

7. Uprav kód aplikace tak, aby zobrazovala u každého města i počet obyvatel a rozlohu v kilometrech čtverečních. Budeš muset upravit komponentu `City`, její props, i to, jak ji používáš a předáváš do ní props uvnitř hlavní komponenty `App`.

8. Předpokládám, že komponentu máš hezky v samostatné složce. Přidej k ní do složky i její vlastní `style.css` a komponentu zkus trochu nastylovat, aby aplikace vypadala hezky.

9. Bohužel máš náročného zákazníka, který se nespokojí jen s deseti největšími městy, ale chce vidě **všechna** česká města. Naštěstí si můžeš stáhnout [ZIP soubor](https://github.com/Czechitas-React-podklady/React-lekce-05/raw/main/cviceni-02-mesta/ceska-mesta.zip), který obsahuje seznam všech českých měst aktuální k 1. lednu 2020. Naštěstí zákazník není zase tak náročný, aby potřeboval nejnovější údaje :)

10. Soubor `cz-cities.js` ze ZIPu si zkopíruj do složky `src` v našem projektu a podívej se, jak uvnitř vypadá.

11. V hlavním `index.js` smaž naše dříve vytvořené pole `cities` a místo něj si naimportuj `cities` ze zkopírovaného souboru `cz-cities.js`. V tu chvíli by už tvoje aplikace měla zobrazovat všechna česká města.

12. V datech jsou teď i další údaje navíc - například okres a obrázek města. Uprav aplikaci a naší komponentu `City` tak, aby zobrazovala i tyto další údaje.

13. Máš li čas a chuť, nastyluj komponentu tak, aby i tyto dodatečné údaje byly na stránce hezky prezentované. Můžeš zkusit různé podoby aplikace - třeba jako seznam, kde jsou všechna města pod sebou, nebo jako kartičky, kde jsou jednotlivá města v mřížce - např. 5 měst vedle sebe na řádku, každé město má fotku a pod ní název a další údaje. Zapoj vlastní fantazii :)
