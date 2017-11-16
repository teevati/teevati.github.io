---
id: 39
title: 'Uusi kone tai vanha henkiin&#8230;'
date: 2008-07-09T14:44:07+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=39
permalink: /2008/07/09/uusi-kone-tai-vanha-henkiin/
categories:
  - tietokoneet
tags:
  - muisti
  - näytönohjain
  - ongelma
  - RAM
  - tietokoneet
  - USB
  - Windows
  - Windows XP
  - XP
---
Jo useita vuosia olen toistuvasti miettinyt uuden koneen hankkimista. Koneenihan on ollut jonkin verran rikki jo kolmesta viiteen vuotta. [Viime vuoden alkupuolelta](/mww/blogalike/?fi&bid=2007_01#p1300 "blogAlike : Kiireitä + kameran hankinta + tietokoneen hankinta") lähtien vikoja on alkanut olla kertyneenä sen verran paljon, että koneen vaihtaminen oli tarkoitus hoitaa jo viimeistään tänä keväänä. Koska kuitenkin törsäsin uuteen kameraan, lykkäsin koneen päivittämisen (alku)syksyyn.

Eilen kuitenkin keskustelin erään kaverini kanssa koneista ja innostuin tutkailemaan [Huuto.net](http://www.huuto.net "Huuto.net - Huutokauppa")istä, jos joku vaikka kauppaisi samanlaista emolevyä kuin omani ([MSI KT3 Ultra-ARU eli MS-6380E](http://global.msi.com.tw/index.php?func=proddesc&prod_no=273&maincat_no=1 "MSI -- Microstar Int'l Co., Ltd. -  Home  > Products  > Mainboard : KT3 Ultra/ Ultra-ARU"), VIA Apollo 266A -piirisarja, AMD Socket A, ATA133 RAID, USB 2.0 [NEC], 6.1 SPDIF koksi ja optinen lähtö). Ihan samaa ei löytynyt, mutta päädyin edelleen [FAQ](http://global.msi.com.tw/index.php?func=faqIndex "MSI -- Microstar Int'l Co., Ltd. - FAQ"):n kautta [käyttäjäfoorumiin](http://forum.msi.com.tw/ "MSI HQ User to User Forum"), jossa törmäsin kuvauksiin samoista ongelmista, joita minullakin on ollut.

Ensimmäisenä ilmennyt ongelmani on [USB2.0:n toimiminen vain USB1.1:n nopeudella](http://forum.msi.com.tw/index.php?topic=13160.0 "MSI HQ User to User Forum > Mainboards > Retired motherboards > Topic: Problem with USB2 on KT3 Ultra ARU") (vain yksi esimerkkiketju, sama ongelma tuntuu olevan melko yleinen). Joitakin ratkaisujakin tarjotaan ja aionkin kokeilla niitä. Lainaanpa tähän pari ratkaisuehdotusta:

> [I solved my problem
  
> When i use my usb 2.0 ports i must have nohting in the usb 1.1 ports
  
> I now put all my usb devices in the usb 2.0 ports
  
> This comes because my chipset has a major bug](http://forum.msi.com.tw/index.php?topic=67284.msg470265#msg470265 "MSI HQ User to User Forum > Mainboards > Retired motherboards > Topic: usb 2.problem on ms-6830 kt3 ultra aru v1.0 : Reply #4")

Toinen vaihtehto: Poista kaikki USB:hen liittyvät ajurit, boottaa ja anna Windowsin tunnistaa ne uudelleen. Toista, kunnes USB2.0 toimii&#8230;

Seuraava ongelma tuli [ATI Radeon 9600XT:n kanssa lisämuistien myötä](http://teevati.net/btw/?p=7 "Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Error") (osat [2](http://teevati.net/btw/?p=8 "Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Error, osa 2") ja [3](http://teevati.net/btw/?p=10 "Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Error, osa 3")). Catalyst-ajurit nimittäin kaatuvat, jos muistia on enemmän kuin 2 gigaa. Syy voi tietysti olla esim. muistiavaruuden loppuminen kesken, jos näytönohjaimen 512Mt:n varaus lasketaan yhteen kolmen gigan keskusmuistin kanssa, mutta näin ei mielestäni pitäisi olla. Myös tähän tarjotaan foorumilla joitakin ratkaisuja (lähinnä ajuripeliä) ja niitäkin aion kokeilla. Voi olla, että näytönohjaimella on jotain tekemistä myös koneen buuttausongelman kanssa, joka kyllä on ilmennyt toisinaan jo pitkään ja muistaakseni myös ennen tätä näytönohjainta. Kone siis käynnistyy Windowsin aloitteluun asti, mutta sitten tule BSOD. Ja toisinaan kone myös jumiutuu kesken kaiken ja se on pakko sammuttaa väkisin. USB2.0-ongelman jälkeen tämä on ikävin. Ehkä jopa ikävämpi, sillä USB2.0:aa vaativat massasiirrot esim. kamerasta voin hoitaa läppärillä ja synkata verkkolevyn kautta. Silloin varmuuskopiotkin tulee tehtyä samalla. (Focus on Positive!) Lopuksi vielä [eräs ratkaisuehdotus](http://forum.msi.com.tw/index.php?topic=28377.msg163054#msg163054 "MSI HQ User to User Forum > Mainboards > Retired motherboards > Topic: Radeon 9600 Pro Problems") näihin Radeon 9600 ongelmiin:

> For those of you having trouble getting your radeon 9600 pro video card working well (lock-ups, serious errors, mouse pointer problems, corrupted craphics), and especially lock-ups with certain games (ie. c&c generals) try the following:
> 
> My kt333 based msi kt3 ultra-aru mobo (and maybe others) can now be run at full hardware acceleration and 100% stable perfromance by:
  
> 1) download and install latest via chipset driver from via site.
  
> 2) download and install latest (soundblaster live!) sound card driver
  
> 3) download and install latest catalyst 3.7 driver/control panel/samartgart from ati.
  
> 4) disable vga fast-write in bios..
  
> 5) go to c:programsati technologyati\_control\_panel and execute smartgart link
  
> 6) enable &#8211; pci read/write and agp read.
  
> 7) disable &#8211; agp write (default in my case was &#8220;on&#8221; causing the problem).
  
> 8) &#8220;apply&#8221;, reboot, then &#8220;ok&#8221;.
> 
> If you are feeling lucky, just try steps 3 through 8&#8230;..

Kolmas ongelma ilmaantui jossain vaiheessa ja on tavallaan vain pikkuseikka, mutta pahimmillaan melkoisen häiritsevä. [Äänet nimittäin särisevät ja särkyvät](http://forum.msi.com.tw/index.php?topic=46328.0 "MSI HQ User to User Forum > Mainboards > Retired motherboards > Topic: MS-6380E and sound problems") varsinkin leffoja katsellessa. Ongelma ei ole liitännässä, koska sama ilmiö on myös optisessa lähdössä. Syyttäisin siis joko äänikorttia tai ajureita. Tätäkin koetan varmaan ratkoa ajuripäivityksillä tai uusimpien ajurien asentamisella uudelleen.

Jos saisin USB2.0-ongelman ratkaistua, olisi konetta huomattavasti mukavampi käyttää. Jos käynnistymis- ja kaatumisongelmat ratkeaisivat, saisi kone varmsti lisäaikaa ja ääniongelman poistuminen parantaisi fiilistä entisestään. Jos sitten saisin vielä näytönohjaimen hyväksymään kolmannen gigan muistia kenkkuilematta, olisi kone taas melkein kuin uusi. Uuden koneen hankkiminen on toki kivaa, mutta budjetin lisäksi jarruttaisin sitä edelleen mielelläni siksi, että nykyisen koneen käyttiksen ja softat olen viritellyt niin mittojen mukaan, että uudella koneella pääsisin samaan vasta kuukausien (tai vuosien) kuluttua. Enkä saisi kaikkea (etenkään meta)dataakaan siirrettyä tai synkattua uudelle koneelle sellaisenaan. Ainakin kuva-arkiston osalta menettäisin jonkin verran oheisinformaatiota. Jos voisin vain vaihtaa emolevyn ja pitää kaiken muuten ennallaan, en jarruttelisi, mutta yhteensopivuus emojen välillä ei ikävä kyllä ole niin hyvällä tasolla (imageyhteensopivuus&#8230;).