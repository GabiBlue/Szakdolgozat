Általános célú menetrendnyilvántartó rendszer
=============================================

Bevezetés
---------

* Ezt elég lesz majd csak a végén összerakni.
* Itt arról kell meggyőzni az olvasót, hogy milyen jó lesz neki, ha végigolvassa az egész dolgozatot. :)
* Majd az elkészült eredményekből látszik, de tetszetős lehet majd itt hangoztatni, hogy mennyire rugalmas, szabványoknak megfelelő, és átvihető megoldásról van szó.

Menetrend alkalmazások
----------------------

* Le kell írni, hogy milyen típusú menetrendek vannak, milyen jellegű problémák merülnek fel a menetrendi adatok nyilvántartásánál.
* Érdemes minél több hasonló alkalmazást megemlíteni, bemutatni, és össze is hasonlítani őket, ahol lehet.

Az adatok hozzáférhetőségével, és az alkalmazások közötti adatátvitellel kapcsolatban is érdemes összeszedni pár dolgot.

Az alkalmazás felépítése
------------------------

Le kell írni majd nagyvonalakban, hogy mik az alkalmazás fő részei és azok hogyan kapcsolódnak egymáshoz. Gyakorlatilag egy kliens-szerver-es ábrát kell csinálni, kiemelve rajta a sajátos megoldásokat.

Itt lehet leírni azt is, hogy az egyes keretrendszerek és library-k választását mi indokolta. Annak kell érződnie, hogy minden funkcióhoz megfelelően lettek kiválasztva az eszközök. 

Az API kialakításával kapcsolatos alapvető tudnivalókat is itt érdemes közölni. A részleteibe elég lesz majd csak az adott funkciókat bemutató fejezetekben belemenni.

GTFS adatbázisok
----------------

Ez itt az adatmodell részletezésével foglalkozó fejezet. Ide jöhet majd az ER vagy relációs diagram, illetve a séma részletezése.

A Python-os GTFS library-t is itt érdemes közelebbről bemutatni. Több alternatíva esetén azokról készülhet ide egy összehasonlító elemzés.

Felhasználói felület
--------------------

A cím itt is lehet majd beszédesebb, de gyakorlatilag azt kellene itt kifejteni, hogy a felhasználó szemszögéből mi és hogy látszik majd a rendszerben. Még ez is inkább a tervezés részhez tartozik, tehát elsősorban specifikáció jellegű.

A komplikáltabb kliens oldali megoldásokat (például térképek megjelentése, vagy egyéb vizualizáció féle) majd akár külön fejezetben is lehet részletezni.

Útvonalak keresése
------------------

Egyelőre ez tünik az a menetrendalkalmazás elsődleges funkcionalitásának. Az adatmodellnek megfelelően le kellene majd írni implementációtól független (kvázi matematikai jelölésekkel), hogy milyen optimalizálási feladatot old meg az alkalmazás a keresés közben.

Ezt a fejezetet fel lehet építeni például úgy is, hogy először a naív, irányított gráfban való keresés kerül bemutatásra, és utána fokozatosan kerülnek bele a további feltételek (megszorítások/constraints). Mindegyikhez érdemes lesz majd minél több ábrát, minimálpéldát is készíteni, illetve becsléseket adni a számítási időkre vonatkozóan.

* További funkciók
------------------

Külön fejezetekbe kerülhetnek a további funkciók, vagy komplikáltabb megoldások. Csak ötlet szintjén:
- Következő ajánlott útvonal számítása az aktuális idő, kiindulópont és a célállomás ismeretében. (Az útvonalkereső is gyakorlatilag ezt csinálja, itt annyi a különbség, hogy kvázi kiírja a felhasználónak, hogy merre érdemes indulnia, és vált, ha közben megváltozik a javaslat az eltelt idő miatt.)
- Menetrend mentése valamilyen nyomtatható formában.
- Minimalizálás az átszállások számára vonatkozóan.
- Kieső járattal kapcsolatos számítások.
- Várakozási idők minimalizálása, vagy limit az átszállásra vonatkozóan (például több legyen, mint 3 perc, hogy biztos legyen idő átszállni).

Amit nagyon érdekes lenne még belerakni, hogy ismert megállók és az azokat összekötő útvonalak esetében kiszámolni egy lehetséges, valamilyen szempontból optimális menetrendet. Ez tehát az előző, keresési problémának a megfordítása lenne.

Tesztelés
---------

Itt már a rendszer egészére, illetve a felhasználásra vonatkozó tesztekre kell kitérni.
Egységtesztekről már a tervezés és implementációs részekben is érdemes beszélni.
Össze kell majd gyűjteni lehetőleg minél több (publikus :)) GTFS adatbázist, és az eredményeikről lehet valamilyen összehasonlító elemzés félét is csinálni (táblázatok, grafikonok).

Összefoglalás
-------------

* Ezt elég lesz majd csak a végén megcsinálni.
* Ebben már csak át kell majd tekinteni az elkészült dolgokat.
* 1-2 oldalnál (a bevezetéshez hasonlóan) ennek sem kell hosszabbnak lennie.

Hivatkozások
------------

* Webalkalmazások fejlesztéséhez kapcsolódó irodalmak
* Szabványokkal kapcsolatos hivatkozások
* Az elérhető megoldások hivatkozásai
* A menetrendek adatainak kezelésével kapcsolatos algoritmusok irodalmai
