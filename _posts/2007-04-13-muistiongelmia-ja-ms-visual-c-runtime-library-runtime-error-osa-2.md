---
id: 8
title: 'Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Error, osa 2'
date: 2007-04-13T22:35:40+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=8
permalink: /2007/04/13/muistiongelmia-ja-ms-visual-c-runtime-library-runtime-error-osa-2/
categories:
  - tietokoneet
tags:
  - Google
  - muisti
  - näytönohjain
  - RAM
  - tietokoneet
  - Windows
  - Windows XP
  - XP
---
Tuhrasin sekä eilen että tänään rutkasti aikaa keskiviikkona ilmenneen ja [eilen pohdiskelemani](/btw/?p=7 "Muistiongelmia ja MS Visual C++ Runtime Library: Runtime Errorr") Runtime Errorin debuggaamiseen. Etsin ratkaisuja verkosta ja mietin, mikä niistä voisi toimia ja mikä ei &#8211; lähinnä sen perusteella, mitä ohjelmia olin juuri asentanut ja mitkä olivat olleet käytössä jo pitempään ja toisaalta mitä minulla ei ollenkaan ole. Syypääksi osoittautui lopulta käyttämäni imurointiapuohjelma [Free Download Manager (FDM)](http://www.freedownloadmanager.org/index.htm "Free Download Manager - absolutely free download accelerator and manager"). Sen poistaminen korjasi ongelman heti eikä uudelleen asentaminen aiheuttanut niitä uudelleen. Ilmeisesti muistisekoilu ja näytönohjaimen ajurien kanssa puljaaminen sekä muu virittely (mm. selaimen) oli onnistunut jotenkin sotkemaan FDM:n dll:t tjsp., mistä seurasi sitten ongelmia. Nyt kaikki kuitenkin tuntuu olevan tältä osin kunnossa, joten huomenissa menen vielä neuvottelemaan, jos saisin kolmannen muistin vaihdettua saman merkkiseen kuin kaksi muuta. Sitten varmaan kokonaisuus on tasapainossa.

Niin, en muuten tosiaan keksinut syyllistä itse, vaan mainitsemani nettihaut tuottivat tulosta. Tiivistetyimpänä oikea ratkaisu löytyy toisesta vastauksesta, joka on annettu [MSDN Forumsin ketjuun](https://forums.microsoft.com/MSDN/ShowPost.aspx?PostID=822452&SiteID=1 "microsoft visual c++ runtime library runtime error c:\windows\explorer.exe abnormal program termination - MSDN Forums").
  
Kysymys kuuluu:

> I am facing problem as follows in my PC having windows xp pro as OS.
  
> When I am clicking C drive icon folders are opened. When I next click any folder I get the message as Run Time error C:\windows\explorer.exe abnormal program termination&#8211;microsoft visual C++ runtime Library. Kindly arrange to help me to solve this problem.

Ja vastaus:

> OK I had the same problem and for the people that might have this problem in the future to make it easier becouse I had to look for an answer for this in the tiniest lines on every forum and I found the solition. So what might help you is one of this or all of them try them all until it works:
> 
> 1. Uninstall Google Toolbar
  
> 2. Uninstall IE 6.0 and reinstall, unistall IE 6.0 and install IE 7.0
  
> 3. Scan with Ad-aware, spybot Search & Destroy in SAFE mode
  
> 4. Downloaded BHO Captor, ran the program(usually helps all the time)
  
> 5. Disable McAfee spam killer
  
> 6. Unistall McAfee Security Centre
  
> 7. Unistall FREE DOWNLOAD MANAGER(helped me to fix the problem and many others)

Kohta 7. siis ratkaisi ongelman minun kohdallani, kuten useat muutkin ovat sekä tässä ketjussa että muualla kommentoineet. Myös muut kohdat ovat osoittautuneet ratkaisuiksi toisilla, mutta tämä siis minulla. Viimeisimmän kerran löysin tämän ratkaisun luokse MS:n Live Searchin kautta haulla [Microsoft Visual C++ Runtime Library error explorer.exe abnormal program termination](http://search.microsoft.com/results.aspx?q=Microsoft+Visual+C%2B%2B+Runtime+Library+error+explorer.exe+abnormal+program+termination&qsc0=0&FORM=QBME2&l=2&mkt=fi-FI "Microsoft Live Search - Haun tulokset : Microsoft Visual C++ Runtime Library error explorer.exe abnormal program termination"), vaikka lähdinkin liikkeelle Yahoo!:n ja Googlen kautta. Niistä löytämäni viestiketjut ohjasivat Microsoftin sivuille, joiden kautta sitten päädyin hakemaan Knowlegde Basesta ja Live Searchilla ja päädyin lopulta viittaamalleni sivulle.

Kun nyt kokeilin tätä täsmälleen samaa halua [Google löysi](http://www.google.fi/search?q=Microsoft+Visual+C%2B%2B+Runtime+Library+error+explorer.exe+abnormal+program+termination&hl=fi&btnG=Google-haku&lr=lang_fi&sourceid=mozilla-search "Microsoft Visual C++ Runtime Library error explorer.exe abnormal program termination - Google-haku") huomattavasti epäselvempiä vaihtoehtoja, mutta [Yahoo! löysi](http://search.yahoo.com/search?p=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination&ei=UTF-8 "Microsoft Visual C++ Runtime Library error explorer.exe abnormal program termination - Yahoo! Search Results") ensimmäiseksi juuri tämän viittaamani MSDN Forumsin ketjun. Useimmiten käytän hauissani Googlea, mutta tässä tapauksessa osoittautui jälleen kerran, että jos ratkaisua ei löydy heti, kannattaa hakutermien parantelun lisäksi koettaa muita hakukoneita. Juuri tätä varten lisäsin selaimeeni (Firefox) [CustomizeGoogle](http://www.customizegoogle.com/ "CustomizeGoogle : Improve Your Google Experience -- Firefox Extension")&#8211;[laajennuksen](https://addons.mozilla.org/en-US/firefox/addon/743 "CustomizeGoogle :: Firefox Add-ons"), joka tarjoaa hakutulosten alkuun linkit &#8220;Kokeile hakuasi muilla hakukoneilla: [Yahoo](http://search.yahoo.com/search?p=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination&ei=UTF-8), [Ask](http://web.ask.com/web?q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [AllTheWeb](http://www.alltheweb.com/search?q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination&cs=utf-8), [MSN](http://search.msn.com/results.aspx?q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [Lycos](http://search.lycos.com/default.asp?query=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [Technorati](http://www.technorati.com/cosmos/search.html?url=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [Feedster](http://www.feedster.com/search.php?q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [Bloglines](http://www.bloglines.com/search?t=1&q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination), [Altavista](http://www.altavista.com/web/results?q=Microsoft%20Visual%20C%2B%2B%20Runtime%20Library%20error%20explorer.exe%20abnormal%20program%20termination)&#8220;. Näistä Yahooo!:n lisäksi AllTheWeb ja Altavista palauttavat tuon mielestäni hyödyllisimmän tuloksen ensimmäisten joukossa. Muissa tulos on huonompi &#8211; etenkin blogeihin keskittyvissä hauissa, jotka eivät palauta mitään hyödyllistä.