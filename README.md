# h2.1
Missing piece

## Uusi yritys

Lähden uudelleen h2 osioon ja nyt huomattuani teen oikeat osiot kyseisestä tehtävästä. 

Asiaan, aloitan avaamalla tehtävän annon ja tutkin, että teen varmasti kaiken oikein. Sitten Virtuaalikone auki ja micro editoria latailemaan. 
Syötetään terminaaliin komento: 

        curl https://getmic.ro | bash
        
[Kuva 1 1](https://user-images.githubusercontent.com/100162043/213925392-fedfae63-9ee0-4fb6-aabc-94b65cef0039.jpg)


Tämän jälkeen listasin testaamani koneen raudan kirjoittamalla seuraavan komennon terminaaliin: 

        $ sudo lshw -short -sanitize
        
[Kuva 2 1](https://user-images.githubusercontent.com/100162043/213925395-cc83a35e-b9a6-45eb-bf5b-370b4f00b1c4.jpg)


Kuvan perusteella huomasin, että lshw komentoa ei löydetty, joten jatkoin asentamalla lshw:n terminaaliin:

        $ sudo apt-get install lshw
        
Nyt kun kirjoitin komennon uudelleen, tulee haettu näkymä. 

[Kuva 3 1](https://user-images.githubusercontent.com/100162043/213925401-986a758f-d4a0-4256-8a15-3fc1b4ddc6c6.jpg)


Analyysi kertoo, että oma koneeni pitää sisällään Inter(R) Core(TM) i5-1035G1 CPU @ 1.00GHz prossun. Tämän lisäksi löydän tiedon asettamastani 4GiB muistista,
jonka asetin Virtuaalikoneelleni. Tästä listauksesta löytyy myös paljon muuta tietoa, mutta nämä olen kokenut tärkeimmiksi mainita. 

## Komentoriviohjelmat

Seuraavaksi pääsin tutustumaan eri komentoriviohjelmiin. Tähän löysin hyvän sivuston, mistä otin kolme mieleistä esimerkkiä näytille. 
Asentelin nämä ohjelmistot erikseen. 

        $ sudo apt install rig
        $ rig
        
Rig luo satunnaisesti väärennetyt henkilöntiedot. Tähän ei sen isompaa selitystä ole, mutta huomaan, että tällainenkin on olemassa!

[Kuva 4 1](https://user-images.githubusercontent.com/100162043/213925408-5b56c88a-50a0-4d56-857f-2585ac82f366.jpg)


Seuraavana mennään nostalgian maailmaan ja -90 luvun lopun yhden isoimman elokuvan sisältöön! Tätä tuskin sen enempää täytyy perustella, miksi tämä on valittu!

        $ sudo apt install cmatrix
        $ cmatrix
        
[Kuva 5 1](https://user-images.githubusercontent.com/100162043/213925417-b6d0cfc8-f6ff-485e-acd8-243ec4d7e6c4.jpg)


Viimeisimpänä valitsin keskelle ruutua tulevat silmät, jotka seuraavat hiireni liikettä! Mukavia pikku lisäyksiä terminaaliin. 

        $ sudo apt install x11-apps
        $ xeyes
        
[Kuva 6 1](https://user-images.githubusercontent.com/100162043/213925466-a9a4645c-a000-452a-9690-c39accdcb0aa.jpg)


## Important directories

Ensimmäisenä mikä tuli mieleen oli Root directory eli juurihakemisto. Tämän alta löytyy kansiot ja tiedostot kaikkeen. 

          $ ls
          
[Kuva 7 1](https://user-images.githubusercontent.com/100162043/213925476-c46855a6-636f-430a-a926-ffa5af5939f1.jpg)


Toisena otin esille oman home hakemiston. Täältä löytyy käyttäjän tiedostoja. Myös käyttäjä voi luoda uutta sisältöä home hakemistoon. 

          $ cd /home
          $ ls
          
[Kuva 8 1](https://user-images.githubusercontent.com/100162043/213925483-ab2a707e-3483-40b3-a194-7c2a1277a8b4.jpg)


Viimeisimpänä ajattelin tuoda esille Etc kansiot, joka käytännössä pitää sisällään järjestelmään liittyvät tiedostot ja asetukset. 

        $ cd /etc
        $ ls
        
[Kuva 9 1](https://user-images.githubusercontent.com/100162043/213925491-470f9d09-f0fd-4bfa-b97e-bf7436cec9c1.jpg)


Kuten huomaa, etc kansion sisältö ei aivan edes mahtunut koko screenshottiin.. 


## grep

Lähdin tutkimaan aihetta eri sivustojen kautta sekä katselemalla parit youtube videot. Testailin hetken ja en meinannut alkaa saada onnistumisia. 
Kuitenkin kokeilin kuinka käyttää grep komentoa eri tarkoituksissa. 

Ensimmäisenä esimerkkinä oli lähde listauksen mukaisesti katsottu grep komento IP-osoitteen perusteella. 

        $ grep -r "192.168.1.5" /etc/
        
[Kuva 10 1](https://user-images.githubusercontent.com/100162043/213925495-729be8e3-33fb-47ee-960e-fa632e5452ee.jpg)


Toisena ja viimeisempänä käytin grep komennon avulla värimuutosta. 

        $ GREP_COLOR='1;35' grep --color=always nobody /etc/passwd
        
[Kuva 11 1](https://user-images.githubusercontent.com/100162043/213925501-2e3b5390-6d69-4fa6-8ec1-629a25bd1adb.jpg)


## Tiivistelmä

On hauska huomata kuinka paljon eri asioita terminaalin avulla voikaan tehdä. Ei pelkästään antaa komentoja vaan myös luoda ulkoasua Terminaalin sisällä. 
Linux on vienyt minun huomioni täysin. Pitkään olen miettinyt asentavani Linux käyttöjärjestelmän raudalle, mutta toistaiseksi näin ei ole vielä tapahtunut. 
Nyt kyllä ajatus alkaa muuttua toteutuksen puolelle kuitenkin tämän suhteen. Kohti seuraavaa!
        

## Lähteet
https://micro-editor.github.io/
https://www.makeuseof.com/fun-linux-command-line-programs/
https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/
https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited
Muut sekalaiset youtube videot aiheeseen liittyen. 


