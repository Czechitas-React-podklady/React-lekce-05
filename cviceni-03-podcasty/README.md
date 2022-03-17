# Cvičení 3 - Podcasty

Vytvoř aplikaci, která bude zobrazovat seznam epizod tvého oblíbeného podcastu.

1. Jako podklady pro toto cvičení si stáhni [nastylovanou stránku](https://github.com/Czechitas-React-podklady/React-lekce-05/raw/main/cviceni-03-podcasty/podcasty-zadani.zip). Obsahuje ukázkové HTML a CSS, jak má výsledná stránka vypadat. Z tohoto HTML a CSS si můžeš vykousnout, cokoliv budeš potřebovat a použít ve svých komponentách.

2. Známým postupem si založ nový React projekt pomocí `create-czechitas-app` a nazvi ho třeba `podcasty`.

3. Vytvoř komponentu `Episode`, která bude zobrazovat jednu edpizodu podcastu. Jako `props` do komponenty předej `num` (číslo epozody), `title` (název epizody) a `guest` (host, se kterým se hovoří).

4. Ze stažených podkladů vykousni CSS týkající se jedné epizody a udělej z něj samostatný CSS soubor ve složce s komponentou, ať je hezky pohromadě vše, co komponenta potřebuje.

5. Komponentu vyzkoušej tak, že ji v `App` třeba dvakrát za sebou použij a manuálně do ní předej potřebná data (třeba ta, co jsou uvedena na vzorové stránce).

6. Pokud ti komponenta funguje, tak na místo napevno napsaných props si seznam epizod podcastu budeme brát z následujícího pole:

	```js
	const episodes = [
		{ num: 126, title: 'Robot, který snědl koblihu', guest: 'Radovan Siwek' },
		{ num: 127, title: 'Hledání plyšového Yettiho', guest: 'Vojtěch Ryba' },
		{ num: 128, title: 'Moderní hrachová polévka', guest: 'Kamila Štancová' },
		{ num: 129, title: 'Poloautomatické zrcadlo', guest: 'Janka Janovská' },
		{ num: 130, title: 'Máčené hlavy parlamentu', guest: 'Jonáš Daněk' },
		{ num: 131, title: 'Služby na hraně přívěsu', guest: 'Tereza Křivánková' },
		{ num: 132, title: 'Klasifikace sněžných klokanů', guest: 'Josef Stix' },
		{ num: 133, title: 'Rybolov v Oceánu bouří', guest: 'Ludmila Gajová' },
	];
	```

7. Toto pole přemapuj na komponenty `Episode` a zobraz na stránce všechny epizody podcastu. Promysli, jaká vlastnost se nejlépe hodí jako klíč a použij ji, aby React k konzoli prohlížeče přestal vyhrožovat, že mu chybí prop `key`.
