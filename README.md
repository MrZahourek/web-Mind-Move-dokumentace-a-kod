<====== • Mind Move web • ======>
~ Dokumentace ~

#1 Změna obrázku
Pokud bude potřeba změnit obrázek budeme muset  předem udělat několik věcí:
Prvně se ujistíme že známe všechny lokace kde budeme obrázek měnit. Toto děláme čistě pro konzistenci (zároveň je dobré vědět co bylo změněno kdyby nastal problém).
Obrázek který se pokusíme vyměnit uložíme. Je praktické mít uložené původní obrázky v případě chyby. Není nutné ukládat obrázky ze všech verzí, stačí jedna nebo dvě vězte zpět.
Uložíme poslední verzi kódu ještě před editací aby v případě problému byla blízka verze po ruce.
Pokud jsme splnili všechny tyto kroky může přejít k editaci. Obrázek je v HTML označen <img>, taky bych v jeho okolí hledal komentář označující specifický obrázek. Část kódu ovlivňující o jaký obrázek se jedná je source. Source najdeme v kódu schovaný v <img> příkazu. Místo slova source bude použita jeho zkratka src a bude u něj znaménko =, doprovázené uvozovkami(" "). Abychom změnili obrázek budeme muset změnit zdroj (source), konkrétně budeme měnit jeho cestu k obrázku. Všechny obrázky se nacházejí ve složce Images (cesta do složky Images(pro počítač) - /www/Images , cesta do Images(pro telefon) /www/Mobile/Images). Abychom nahradily obrázek nahrajeme nový obrázek do složky Images (a zapamatujeme se jeho jméno včetně koncovky za tečkou (př.: .png .jpg). Následně se vrátíme do kódu a přepíšeme zdroj všech obrázků které chceme změnit. Změna zdroje je vlastně snadná ale také se dá snadno zkazit, to co musíme udělat je vlastně jen změnit posledních pár slov ve zdroji. Smažeme původní název obrázku (ten je na konci odkazu a bude končit jedou z koncovek pro obrázky (př.: .png) a nahradíme ho názvem našeho nového obrázku (př.: …/slozka1/slozka2/příklad.png -› …/slozka 1/slozka 2/novyobrazek.jpg). Pokud tento kód nefunguje zkontrolujte tyto věci:
Je název obrázku správně napsaný?
Nesmazali jsme omylem i část odkazu (př.: slozka1/slozka2novyobrazek.png)?
Je odkaz napsaný v src?
Je celý odkaz v uvozovkách?
Je obrázek nahraný do složky Images? Není jenom v jedné z nich?
To co může snadno nastat je to že obrázek bude vypadat špatně (př.: bude roztažený, nebo naopak smáčknutý) to je způsobeno tím že je příliš malý/velký. V případě že nastane tato nebo jiná chyba stačí kontaktovat programátora který je v současnosti jeho správcem (v tuto chvíli je to Vojtěch Kotlík - email: Žahour).

#2 Úprava pro pop up
