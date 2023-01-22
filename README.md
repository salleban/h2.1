# h2.1
Missing piece

## Uusi yritys

Lähden uudelleen h2 osioon ja nyt huomattuani teen oikeat osiot kyseisestä tehtävästä. 

Asiaan, aloitan avaamalla tehtävän annon ja tutkin, että teen varmasti kaiken oikein. Sitten Virtuaalikone auki ja micro editoria latailemaan. 
Syötetään terminaaliin komento: 

        curl https://getmic.ro | bash
        
![Kuva 1 1](https://user-images.githubusercontent.com/100162043/213925771-872b480f-d0c7-4d20-9d2a-62e215afe36c.jpg)


Tämän jälkeen listasin testaamani koneen raudan kirjoittamalla seuraavan komennon terminaaliin: 

        $ sudo lshw -short -sanitize
        
![Kuva 2 1](https://user-images.githubusercontent.com/100162043/213925784-e5f4d8ec-9f49-401e-9444-413a46a58a66.jpg)



Kuvan perusteella huomasin, että lshw komentoa ei löydetty, joten jatkoin asentamalla lshw:n terminaaliin:

        $ sudo apt-get install lshw
        
Nyt kun kirjoitin komennon uudelleen, tulee haettu näkymä. 

![Kuva 3 1](https://user-images.githubusercontent.com/100162043/213925792-bd93cc91-43de-43c4-a45f-bf197d46c07b.jpg)



Analyysi kertoo, että oma koneeni pitää sisällään Inter(R) Core(TM) i5-1035G1 CPU @ 1.00GHz prossun. Tämän lisäksi löydän tiedon asettamastani 4GiB muistista,
jonka asetin Virtuaalikoneelleni. Tästä listauksesta löytyy myös paljon muuta tietoa, mutta nämä olen kokenut tärkeimmiksi mainita. 

## Komentoriviohjelmat

Seuraavaksi pääsin tutustumaan eri komentoriviohjelmiin. Tähän löysin hyvän sivuston, mistä otin kolme mieleistä esimerkkiä näytille. 
Asentelin nämä ohjelmistot erikseen. 

        $ sudo apt install rig
        $ rig
        
Rig luo satunnaisesti väärennetyt henkilöntiedot. Tähän ei sen isompaa selitystä ole, mutta huomaan, että tällainenkin on olemassa!

![Kuva 4 1](https://user-images.githubusercontent.com/100162043/213925797-3ac69f0f-e66d-4d80-bcbe-11eed3d3c1d6.jpg)



Seuraavana mennään nostalgian maailmaan ja -90 luvun lopun yhden isoimman elokuvan sisältöön! Tätä tuskin sen enempää täytyy perustella, miksi tämä on valittu!

        $ sudo apt install cmatrix
        $ cmatrix
        
![Kuva 5 1](https://user-images.githubusercontent.com/100162043/213925801-b4363f25-6b3b-488a-9aa7-33cb0ecd4512.jpg)



Viimeisimpänä valitsin keskelle ruutua tulevat silmät, jotka seuraavat hiireni liikettä! Mukavia pikku lisäyksiä terminaaliin. 

        $ sudo apt install x11-apps
        $ xeyes
        
![Kuva 6 1](https://user-images.githubusercontent.com/100162043/213925807-c6632889-2f09-42cb-a61e-fa252ad3bb32.jpg)



## Important directories

Ensimmäisenä mikä tuli mieleen oli Root directory eli juurihakemisto. Tämän alta löytyy kansiot ja tiedostot kaikkeen. 

          $ ls
          
![Kuva 7 1](https://user-images.githubusercontent.com/100162043/213925815-48effa24-2c87-45ca-9662-eeed6b6c0c3e.jpg)



Toisena otin esille oman home hakemiston. Täältä löytyy käyttäjän tiedostoja. Myös käyttäjä voi luoda uutta sisältöä home hakemistoon. 

          $ cd /home
          $ ls
          
![Kuva 8 1](https://user-images.githubusercontent.com/100162043/213925822-9e39b692-3a09-4697-b508-206995d3b436.jpg)



Viimeisimpänä ajattelin tuoda esille Etc kansiot, joka käytännössä pitää sisällään järjestelmään liittyvät tiedostot ja asetukset. 

        $ cd /etc
        $ ls
        
![Kuva 9 1](https://user-images.githubusercontent.com/100162043/213925824-cf4b71e4-a99c-4bf4-881d-20bd8bc1a58d.jpg)


Kuten huomaa, etc kansion sisältö ei aivan edes mahtunut koko screenshottiin.. 


## grep

Lähdin tutkimaan aihetta eri sivustojen kautta sekä katselemalla parit youtube videot. Testailin hetken ja en meinannut alkaa saada onnistumisia. 
Kuitenkin kokeilin kuinka käyttää grep komentoa eri tarkoituksissa. 

Ensimmäisenä esimerkkinä oli lähde listauksen mukaisesti katsottu grep komento IP-osoitteen perusteella. 

        $ grep -r "192.168.1.5" /etc/
        
![Kuva 10 1](https://user-images.githubusercontent.com/100162043/213925831-51534b48-9e4c-4aa7-872b-53936b9bf51a.jpg)



Toisena ja viimeisempänä käytin grep komennon avulla värimuutosta. 

        $ GREP_COLOR='1;35' grep --color=always nobody /etc/passwd
        
![Kuva 11 1](https://user-images.githubusercontent.com/100162043/213925834-38687fee-7944-407d-b805-16a091ad7617.jpg)



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


