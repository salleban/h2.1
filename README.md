# h2.1
Missing piece

## Uusi yritys

Lähden uudelleen h2 osioon ja nyt huomattuani teen oikeat osiot kyseisestä tehtävästä. 

Asiaan, aloitan avaamalla tehtävän annon ja tutkin, että teen varmasti kaiken oikein. Sitten Virtuaalikone auki ja micro editoria latailemaan. 
Syötetään terminaaliin komento: 

        curl https://getmic.ro | bash
        
-KUVA-

Tämän jälkeen listasin testaamani koneen raudan kirjoittamalla seuraavan komennon terminaaliin: 

        $ sudo lshw -short -sanitize
        
-KUVA-

Kuvan perusteella huomasin, että lshw komentoa ei löydetty, joten jatkoin asentamalla lshw:n terminaaliin:

        $ sudo apt-get install lshw
        
Nyt kun kirjoitin komennon uudelleen, tulee haettu näkymä. 

-KUVA-

Analyysi kertoo, että oma koneeni pitää sisällään Inter(R) Core(TM) i5-1035G1 CPU @ 1.00GHz prossun. Tämän lisäksi löydän tiedon asettamastani 4GiB muistista,
jonka asetin Virtuaalikoneelleni. Tästä listauksesta löytyy myös paljon muuta tietoa, mutta nämä olen kokenut tärkeimmiksi mainita. 

## Komentoriviohjelmat

Seuraavaksi pääsin tutustumaan eri komentoriviohjelmiin. Tähän löysin hyvän sivuston, mistä otin kolme mieleistä esimerkkiä näytille. 
Asentelin nämä ohjelmistot erikseen. 

        $ sudo apt install rig
        $ rig
        
Rig luo satunnaisesti väärennetyt henkilöntiedot. Tähän ei sen isompaa selitystä ole, mutta huomaan, että tällainenkin on olemassa!

-KUVA-

Seuraavana mennään nostalgian maailmaan ja -90 luvun lopun yhden isoimman elokuvan sisältöön! Tätä tuskin sen enempää täytyy perustella, miksi tämä on valittu!

        $ sudo apt install cmatrix
        $ cmatrix
        
-KUVA-

Viimeisimpänä valitsin keskelle ruutua tulevat silmät, jotka seuraavat hiireni liikettä! Mukavia pikku lisäyksiä terminaaliin. 

        $ sudo apt install x11-apps
        $ xeyes
        
-KUVA-

## Important directories

Ensimmäisenä mikä tuli mieleen oli Root directory eli juurihakemisto. Tämän alta löytyy kansiot ja tiedostot kaikkeen. 

          $ ls
          
-KUVA- 

Toisena otin esille oman home hakemiston. Täältä löytyy käyttäjän tiedostoja. Myös käyttäjä voi luoda uutta sisältöä home hakemistoon. 

          $ cd /home
          $ ls
          
-KUVA-

Viimeisimpänä ajattelin tuoda esille Etc kansiot, joka käytännössä pitää sisällään järjestelmään liittyvät tiedostot ja asetukset. 

        $ cd /etc
        $ ls
        
-KUVA- 

Kuten huomaa, etc kansion sisältö ei aivan edes mahtunut koko screenshottiin.. 




        

## Lähteet
https://micro-editor.github.io/
https://www.makeuseof.com/fun-linux-command-line-programs/
https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/
https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited
Muut sekalaiset youtube videot aiheeseen liittyen. 


