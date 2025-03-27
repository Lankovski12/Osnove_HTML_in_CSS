Uvod v HTML in CSS
Kazalo:
Osnovni HTML elementi
Primer enostavne HTML strani
Seznami v HTML
Neurejeni seznam (ul)
Urejen seznam (ol)
Tabele v HTML
Kaj je CSS?
Osnovni CSS elementi
Postavitev elementov
Uporaba display: flex
Uporaba display: grid
Vaje za učence
1. Naloga

Osnovni HTML elementi
Vsaka spletna stran je sestavljena iz različnih delov, ki jih napišemo v posebnih oznakah (tagih). Nekaj osnovnih oznak:
<html> - označuje začetek in konec spletne strani
<head> - vsebuje informacije o strani (naslov, ikone)
<title> - določa naslov strani
<body> - glavni del strani, kjer so besedila, slike itd

<h1> - naslov največje velikosti (gre do števila 6)
<p> - odstavek s tekstom
<a> - povezava do druge strani
<img> - vstavi sliko
<button> - ustvari gumb
<strong> - poudari besedilo
<b> - naredi besedilo krepko
<br> - prelom vrstice

Pomagaj si s to stranjo: https://www.w3schools.com/html/default.asp
Primer enostavne HTML strani
<!DOCTYPE html>
<html>
<head>
    <title>Moja prva stran</title>
</head>
<body>
    <h1>Pozdravljeni!</h1>
    <p>To je moja prva spletna stran.</p>
    <a href="https://www.google.com">Klikni tukaj</a>
    <br>
    <img src="slika.jpg" alt="Primer slike">
    <br>
    <button>Pritisni me</button>
</body>
</html>






Seznami v HTML
Seznami so uporabni za prikazovanje podatkov v obliki točk ali številk.
Neurejeni seznam (ul)
Neurejeni seznam prikazuje elemente s točkami.
<ul>
    <li>Jabolko</li>
    <li>Hruška</li>
    <li>Banana</li>
</ul>
Urejen seznam (ol)
Urejen seznam prikazuje elemente s številkami.
<ol>
    <li>Priprava sestavin</li>
    <li>Mešanje testa</li>
    <li>Peka</li>
</ol>












Tabele v HTML
Tabele se uporabljajo za prikazovanje podatkov v vrsticah in stolpcih.
<table border="1">
    <tr>
        <th>Ime</th>
        <th>Starost</th>
    </tr>
    <tr>
        <td>Miha</td>
        <td>12</td>
    </tr>
    <tr>
        <td>Eva</td>
        <td>11</td>
    </tr>
</table>






















O divih, classih in id
Element <div> je uporaben za organizacijo in strukturiranje vsebine na spletni strani. Predstavljamo si lahko kot škatlo v katero postavljamo stvari, da postanejo neka celota.
class: Uporablja se za skupino elementov, ki imajo enak stil.
id: Uporablja se za en specifičen element na strani.

<body>
    <div class="okvir">
        <h1 id="glavni-naslov">Moj naslov</h1>
        <p class="poudarjen">To je pomembno besedilo.</p>
        <p>To je navadno besedilo.</p>
    </div>
</body>

.okvir { -> class
            border: 2px solid black;
            padding: 20px;
            margin: 10px;
            background-color: lightgray;
 }

 .poudarjen { -> class
 	font-weight: bold;
color: red;
 }

 #glavni-naslov { -> id
 	font-size: 24px;
            text-align: center;
            color: blue;
 }





Kaj je CSS?
CSS (Cascading Style Sheets) je jezik za oblikovanje spletnih strani. Z njim določimo barve, pisave, razmike in druge oblikovne lastnosti.
Osnovni CSS elementi
CSS pravila določimo tako, da napišemo, kateri element oblikujemo in kako naj izgleda.
color - določa barvo besedila.
background-color - določa barvo ozadja.
font-size - določa velikost pisave.
text-align - poravnava besedila.
padding - notranji razmik elementa.
margin - zunanji razmik elementa.
border - rob okoli elementa.
display - določa način prikaza elementa (flex, grid).
background-image: slika v ozdaju;
Postavitev elementov
Uporaba display: flex
Flexbox omogoča enostavno poravnavo elementov v vrsticah ali stolpcih.
.container {
    display: flex;
    justify-content: center; /* Poravnava elementov na sredino */
    align-items: center; /* Poravnava elementov po višini */
    height: 100vh;
}

.item {
    background-color: lightcoral;
    padding: 20px;
    margin: 10px;
}

<div class="container">
    <div class="item">Element 1</div>
    <div class="item">Element 2</div>
    <div class="item">Element 3</div>
</div>


Uporaba display: grid
Grid omogoča enostavno postavitev elementov v mrežo.
<div class="grid">
        <div class="pozdrav"><p>Živjo</p></div>
        <div class="vprasanje"><p>Kako si?</p></div>
        <div class="dan"><p>Danes je lep dan</p></div>
        <div class="sonce"><p>Zunaj je sonce</p></div>
        <div class="naloga"><p>Si naredil domačo nalogo?</p></div>
        <div class="test"><p>Jutri je test</p></div>
    </div>

.grid {
    display: grid;
    grid-template-areas: 
    "zombi vprasanje"
    "dan sonce"
    "naloga test"; 
    grid-template-columns: 1fr 1fr;
    margin: auto;
    width: 30%;
    gap: 10px;
}

.pozdrav{
    grid-area: zombi;
}
.vprasanje{
    grid-area: vprasanje;
}
.dan{
    grid-area: dan;
}
.sonce{
    grid-area: sonce;
}
.naloga{
    grid-area: naloga;
}
.test{
    grid-area: test;
}
p{
    border: solid 1px black;
}

Povezovanje CSS z HTML
CSS lahko vključimo v <head> s tagom <style> ali pa uporabimo zunanjo datoteko in jo povežemo s <link>.
Primer povezave CSS z HTML:
<head>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>




































Vaje za učence
1. Naloga
Ustvari nov dokument index.html v novi mapi poimenovani nal1
Dodaj vsaj eno sliko, vsaj eno besedilo, en seznam (lahko ul ali ol), vsaj eno povezavo. Ostalo po želji.
Tema naj bo živali, šport, potovanje ali igre.
Nardi css datoteko in jo poimenuj style.css. Ne pozabi je povezati z html.
Uporabi display grid ali flex.
Naredi vsaj dva diva. (to moraš zaradi display)
Naj bo veliko barvu. Spremeni barvo ozadja ali pa celo dodaj sliko.
V css dodaj vsaj en border, preizkusi padding in margin. Sliki dodaj border-radius.



