---
id: 7
title: 'Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Error'
date: 2007-04-12T16:15:27+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=7
permalink: /2007/04/12/muistiongelmia/
categories:
  - tietokoneet
tags:
  - muisti
  - näytönohjain
  - ongelma
  - RAM
  - tietokoneet
  - Windows
  - Windows XP
  - XP
---
Ostin viime kuun lopulla gigan lisää muistia koneeseeni. Tarkoitus oli kasvattaa muistin määrä 2,5 gigaan. Muistin kuitenkin väärin sen, millaisia kampoja koneessani entuudestaan oli &#8211; 1024+512 sijasta 3&#215;512. Päälle päätteeksi tuurini oli vielä sen verran huono, että vanhat CL2,5 -luokitellut muistit aiheuttivat lieviä vakausongelmia uuden CL3-laatuisen muistin kanssa. Päädyin siis väliaikaisesti itse asiassa vähentämään muistia eli jätin koneeseen vain yhden 1024 Mt RAM-moduulin. Tähän en kuitenkaan ollut aikeissa tyytyä kovin pitkään.

Eilen sitten kävin hakemassa kaksi kappaletta gigaisia muisteja, jotka kuitenkin olivat eri valmistajan kuin ensimmäinen. Spekseiltään kyllä identtiset, joten niiden piti toimiman oikein yhdessä aiemman muistin kanssa. Kotona sitten laitoin muistit koneeseen ja starttasin. Muuten näytti hyvältä, mutta kun ei näyttänyt &#8211; resoluutio oli tipahtanut 800&#215;600-tilaan eli oletin näytönohjaimen ajurien jotenkin seonneen. Aloinkin sitten tyhmänä tutkia tilannetta tällä oletuksella ja tuhrasin jonkin aikaa, kunnes hoksasin, että kannattaisi eliminoida syiden joukosta muistit.

Sieltähän se syy sitten löytyikin. Pelkällä vanhalla gigaisella muistilla kone starttaisi vallan nätisti ihan oikealla resoluutiolla. Samaten pelkillä uusilla muisteilla kaikkia näytti toimivan vallan mainiosti. Yhdistelmä sotki sitten taas näytönohjaimen pasmat pahemman kerran, mistä onneksi pääsi takaisin ihan vain ottamalla erimerkkisen palikan pois. Jätin siis kaksi uutta gigaista muistia koneeseen toistaiseksi ja tutkin pohdin seuraavaa askelta vielä erikseen.

Asensin tämän sekoilun jälkeen yhden lisäohjelman, jonka asentamisen jälkeen huomasin muutamia ikäviä oireita (lähinnä sen, että resurssienhallinta kaatuu `MS Visual C++ Runtime Library: Run Time Error`iin<sup><a href="#a070412-1">(1</a></sup>, kun yritän mennä jollekin muulle kuin järjestelmän sisältävälle asemalle). Lienee mahdollista, että ne johtuvat kyseisestä ohjelmasta ([Yahoo! Desktop Search &#8211; X1](http://desktop.yahoo.com "Award-Winning Desktop Search from Yahoo! and X1"), tarkemmin varmaankin kyseisen ohjelman ensimmäisestä indeksointikierroksesta, jos se aiheuttaa kenties tarpeettoman ahkeraa levyn käyttöä tai lukitsee jotain väärin tjsp.), mutta jossain vaiheessa aloin miettiä, että jos ne johtuvatkin muisteista, enkä vain huomannut niitä ennen X1:n asentamista. Tätä aion testata, kunhan kerkiän. Tai on mahdollista, että systeri on ehtinyt testata asiaa puolestani, kun ilmeisesti on katsellut kämpässäni leffoja minun puurtaessani virtuaalisen &#8220;sorvin&#8221; ääressä. Siitä kuulen sitten tarvittaessa illemmalla. Toivottavasti tietysti kone ei ole kaatuillut kovin monta kertaa. (Viimeksi niin kävi tuon ensimmäisen muistien yhteensopimattomuuden takia kaksi kertaa yhden elokuvan aikana.)

Kaikean kaikkiaan &#8211; vaikka muistien hinnat ovatkin laskeneet melkoisen siedettävälle tasolle &#8211; kustannuksia kertyi sen verran, että aion palata liikkeeseen ([Mikromaja](http://mikromaja.fi "Mikromaja - entinen lähikauppani")) keskustelemaan, jos saisin vaihdettua joko ensimmäisenä ostamani muistin tai jälkimmäisenä ostamani muistit saman merkkisiin. Lisäksi kannattanee tietysti kysyä, jos heillä on tietoa mahdollisista yhteensopivuusongelmista esim. [Sapphiren ATI Radeon 9600 XT](http://www.sapphiretech.com/en/products/graphics_overview.php?gpid=49 "ATI RADEONâ„¢ 9600 XT Overview"):n (tuulettimeton ja siksi hiljainen) GPU:n tai kenties emolevyni (MSI KT3 Ultra-ARU + AMD Athlon XP 2600+ CPU) ja ostamieni muistien (400MHz DDR CL3 1024Mt, ensimmäinen M-Tec aka TwinMOS, jälkimmäiset Buffalo) kesken. Näytönohjainhan (ajurit) muisteista näytti sekoavan, mikä tietysti saattaa olla näennäistä, mutta sekin mahdollisuus täytyy pitää mielessä, kunnes toisin todistetaan. Ei kannata tuomita muisteja ennen aikojaan.

<sup><a id="a070412-1" title="alaviite">1)</a></sup><small>Tarkemmin lainattuna virheilmoituksia esiintyi kahta lajia:<br /> <code>&lt;strong>Microsoft Visual C++ Runtime Library&lt;/strong>&lt;br />
Runtime error!&lt;br />
C:\windows\explorer.exe&lt;br />
abnormal program termination</code><br /> ja<br /> <code>&lt;strong>Microsoft Visual C++ Runtime Library&lt;/strong>&lt;br />
Runtime Error!&lt;br />
Program C:\Windows\explorer.exe&lt;br />
This application has requested the Runtime&lt;br />
to terminate it in an unusual way.&lt;br />
Please contact the applications support&lt;br />
team for more information.</code></small>

<small>Jos ei ensimmäisen, niin ainakin toisen kerran jälkeen explorerin kaatuminen sitten kaatoi myös Active Desktopin. (Mitäs otin sen käyttöön saadakseni eri taustakuvat kahdelle näytölleni&#8230;)</small>

<p class="poweredbyperformancing">
  <small>Powered by <a href="http://scribefire.com/">ScribeFire</a>.</small>
</p>