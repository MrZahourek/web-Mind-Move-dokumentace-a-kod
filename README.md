# <=============== • Mind Move web • ===============>

~ ===-===-===-===-===-===-===-===-===-=== = ~ _**Dokumentace**_ ~ = ===-===-===-===-===-===-===-===-===-=== ~

<span id="zmena_textu"></span>
 **#1 Změna textu**
Text se v HTML mění velmi snadným způsobem. Jako každý element v HTML je text vložen mezi dvěma "příkazy" v případě textu to budou :

    // Nadpisy - čím nižší číslo, tím větší nadpis (nejde víc jak 6)
    <h1> </h1>
    <h2> </h2>
    <h3> </h3>
    <h4> </h4>
    <h5> </h5>
    <h6> </h6>
	
	// Paragrafy - segmenty textu 
	<p> </p>
	
	// Zvýraznění - text mezi těmito "příkazy" bude následně zvýrazněn
	Kurzíva -> <em> </em> nebo <i> </i>
	Tlusté písmo -> <strong> </strong> nebo <b> </b>

Pokud bude potřeba pokročilejší editace textu není problém napsat správci webu (v tuto chvíli je to  Vojtěch Kotlík - email: [Žahour](mailto:zahour959@gmail.com)). Jakýkoli text který bude mezi "příkazy" které byly výše zmíněny dostane náležité vlastnosti. Rozdíl mezi paragrafem a nadpisem není nutně ve velikosti (Př.: <h3>Velikost 3 </h3> <h4> Velikost 4 </h4> <h6>Velikost 6</h6> 
<p> paragraf </p> <em>text s označující velikost je nadpis</em>). Jak lze vidět rozdíly mezi paragrafy a nadpisy je velikost (i když ne vždy) a tloušťka,  to co nevidíme je to že nadpis si automaticky vezme vlastní řádek - nadpis je vždy v řádku sám.
    
<br>
<br>

<span id="zmena_obrazku"></span>
**#2 Změna obrázku**

Pokud bude potřeba změnit obrázek budeme muset předem udělat několik věcí:

1.  Prvně se ujistíme že známe všechny lokace kde budeme obrázek měnit. Toto děláme čistě pro konzistenci (zároveň je dobré vědět co bylo změněno kdyby nastal problém).
    
2.  Obrázek který se pokusíme vyměnit uložíme. Je praktické mít uložené původní obrázky v případě chyby. Není nutné ukládat obrázky ze všech verzí, stačí jedna nebo dvě vězte zpět.
    
3.  Uložíme poslední verzi kódu ještě před editací aby v případě problému byla blízka verze po ruce.
    

Pokud jsme splnili všechny tyto kroky může přejít k editaci. Obrázek je v HTML označen `<img>`, taky bych v jeho okolí hledal komentář označující specifický obrázek. Část kódu ovlivňující o jaký obrázek se jedná je source. Source najdeme v kódu schovaný v `<img>` příkazu. Místo slova source bude použita jeho zkratka src a bude u něj znaménko =, doprovázené uvozovkami(" "). Abychom změnili obrázek budeme muset změnit zdroj (source), konkrétně budeme měnit jeho cestu k obrázku. Všechny obrázky se nacházejí ve složce Images (cesta do složky Images(pro počítač) - /www/Images , cesta do Images(pro telefon) /www/Mobile/Images). Abychom nahradily obrázek nahrajeme nový obrázek do složky Images (a zapamatujeme se jeho jméno včetně koncovky za tečkou (př.: .png .jpg). Následně se vrátíme do kódu a přepíšeme zdroj všech obrázků které chceme změnit. Změna zdroje je vlastně snadná ale také se dá snadno zkazit, to co musíme udělat je vlastně jen změnit posledních pár slov ve zdroji. Smažeme původní název obrázku (ten je na konci odkazu a bude končit jedou z koncovek pro obrázky (př.: .png) a nahradíme ho názvem našeho nového obrázku (př.: …/slozka1/slozka2/příklad.png -> …/slozka 1/slozka 2/novyobrazek.jpg). Pokud tento kód nefunguje zkontrolujte tyto věci:

1.  Je název obrázku správně napsaný?
    
2.  Nesmazali jsme omylem i část odkazu (př.: slozka1/slozka2novyobrazek.png)?
    
3.  Je odkaz napsaný v src?
    
4.  Je celý odkaz v uvozovkách?
    
5.  Je obrázek nahraný do složky Images? Není jenom v jedné z nich?
    

To co může snadno nastat je to že obrázek bude vypadat špatně (př.: bude roztažený, nebo naopak smáčknutý) to je způsobeno tím že je příliš malý/velký. V případě že nastane tato nebo jiná chyba stačí kontaktovat programátora který je v současnosti jeho správcem (v tuto chvíli je to Vojtěch Kotlík - email: [Žahour](mailto:zahour959@gmail.com)).

  <br>
  <br>

<span id="uprava_pop_up"></span>
**#3 Úprava pro pop up**

Pop up má několik sekcí:

 1. Nadpis a popis
 2. Obrázky a odkaz na více obrázků
 3. Spodní sekci (obrázky, čas, cena, atd...)
 4. Technicky taky tzv. *Teleporter* 

	**1 - Nadpis a popis**
		Tato část je asi ta nejlehčí na pochopení. Je to pouze nadpis (název) ateliéru a jeho popis. Vše se dá snadno změnit (viz.: [Změna textu](#zmena_textu)) a prakticky nemá místo pro chybu.
		**2 - Obrázky a odkaz na více obrázků**
		Každý váš ateliér je doplněn i obrázky z předchozích akcí jako promo materiál (to jak se mění obrázky se dozvíme na [Změna obrázku](#zmena_obrazku)). Musíme mít na paměti že tři které jsou vystaveny na popupu jako takovém jsou velmi malé a detaily nelze rozeznat takže nemá smysl moc se rýpat v jejich kvalitě.
		**3 - Spodní sekce**
		Spodní sekce popisuje informace které nebývají popsané v popisu (tedy cena, lektor, čas, lokace atd... Každá informace je na vlastním řádku a oddělena vodorovnou čárou.  Abychom docílili tohoto efektu stačí se držet následovné šablony:
<em> 	Nedokázal jsem vložit sem nějakou dobrou šablonu - bude to ve složce materiály pod názvem pop up spodek sablona</em>
		**4 - Teleporter**
		Teleportery slouží pro organizaci a samočinné posouvání po stránce webu. Ve skutečnosti jsou to schované neviditelné obdélníčky . Tyto obdélníčky slouží jako odkaz aby se pohled návštěvníka posunul tam kam si přeji. Není důvod si s nimi nějak hrát, pokud to neuzná současný správce webu za potřebné (v tuto chvíli je to Vojtěch Kotlík - email: [Žahour](mailto:zahour959@gmail.com)).
