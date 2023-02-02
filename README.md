
<a href="https://u-szeged.hu/">
    <img src="./paper/szte_uj.jpg" />
</a>

<h1>
    Szegedi Tudományegyetem <br/> Informatikai Intézet
</h1>
<h2>Ujjlenyomat analízis és párosítás képi adatbázisból</h2>
<p>
    <img src="./paper/fp.jpg" />
</p>
<p>
Az adatbázis 520 db képet (326×357 méretű) tartalmazott, mely 7 önkéntes ujjlenyomatait tartalmazza. Hat önkéntes mindkét kezéről, mind a 10 ujjáról 8 db felvétel készült (6*10*8=480), egy önkéntes egy keze került csak beolvasásra (1*5*8=40). Ez a későbbiekben 65 darab osztályt add meg. A képi adatokat egy optikai scanner segítségével gyűjtötték be.
</p>
<h3>Szegmentáció</h3>
<p>
    <img src="./paper/s1.jpg" />
</p>
<p>
Először a tényleges ujjlenyomatot kellett elválasztani a háttértől és egyéb információktól, ehhez először pár képet manuálisan szegmentálni kell, majd a megfelelő jellemzők alapján el lehet dönteni a kép adott részéről, hogy az releváns információt tartalmaz vagy sem.
</p>
<i>Osztályozott pontok érték alapján</i>
<img src="./paper/s5.jpg" />
<img src="./paper/s6.jpg" />

<table>
    <tr>
        <td><img src="./paper/s2.jpg" /></td>
        <td><img src="./paper/s3.jpg" /></td>
        <td><img src="./paper/s4.jpg" /></td>
    </tr>
</table>

<h3>Információ kinyerés</h3>
<p>
    Különböző irányú és értékű Gábor szűrők segítségével a barázdák kiegészíthetőek, hogy belőlük kinyerhetőek legyenek az úgynevezett minúciák. A Gábor szűrős felerősítés után a barázdák vázképét és heurisztikát használva különböző minúciákat tudunk kinyerni.
</p>
<table>
    <tr>
        <td><img src="./paper/g1.jpg" /></td>
        <td><img src="./paper/g2.jpg" /></td>
        <td><img src="./paper/g3.jpg" /></td>
    </tr>
</table>
<p>
Néhány esetben szükséges lehet a vázkép módosítására, hogy a felesleges minúciákat ellimináljuk. Ilyenek lehetnek olyan részek ahol a barázda vonalak megfelelő szögben állnak, de valami miatt megszakított, vagy ha egy barázda vonalból rövid elágazások indulnak ki.
</p>
<table>
    <tr>
        <td><img src="./paper/reduc1.jpg" /></td>
        <td><img src="./paper/reduc2.jpg" /></td>
    </tr>
</table>

<table>
    <tr>
        <td><img src="./paper/reduc3.jpg" /></td>
        <td><img src="./paper/reduc4.jpg" /></td>
    </tr>
</table>
<p>
Két féle típusú minúcia megjelenítése, a barázda lezáró minúciák elhagyásával.
</p>
<img src="./paper/kp.jpg" />


<table>
    <tr>
        <td><img src="./paper/corr.jpg" /></td>
    </tr>
        <tr>
        <td><img src="./paper/sift.jpg" /></td>
    </tr>
</table>

</hr>
<center>
<h2>
DIPLOMAMUNKA
<br>
Sári Gábor & Dr. Németh Gábor
<br>
2022
<br>
</h2>
</center>
