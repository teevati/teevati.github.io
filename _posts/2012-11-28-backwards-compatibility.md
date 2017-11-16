---
id: 1914
title: Backwards compatibility
date: 2012-11-28T15:04:53+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=1914
permalink: /2012/11/28/backwards-compatibility/
categories:
  - blogi
  - ylläpito
tags:
  - FancyBox
  - FancyZoom
  - Flickr
  - jQuery
  - Photonic
  - ShortCode
---
Eilen poistin käytöstä Flickr Photo Album -pluginin, koska sitä ei oltu päivitetty yli kahteen vuoteen. Sen sijaan otin käyttöön [Photonic](http://wordpress.org/extend/plugins/photonic/ "WordPress › Photonic Gallery for Flickr, Picasa, SmugMug and 500px « WordPress Plugins") -pluginin, jotta saan jatkossakin kivasti linkitettyä kuvani [Flickristä](http://flickr.com/photos/teevati "Flikcr: Teevati's Photostream"). Photonicin käyttöönoton myötä huomasin, että aiemmin käyttämäni WP-FancyZoom ei ollut yhteensopiva sen kanssa. Sen olisi tietysti voinut vain poistaa käytöstä, mutta en halunnut muokata kaikkia vanhoja merkintöjä. Siksi mieluummin muokkasin itse FancyZoomia siten, että se ohittaa kaikki Photonicin vastuulla olevat kuvat.

Tämä ei ollut ensimmäinen kerta, kun jouduin huolehtimaan siitä, että kaikki vanha materiaali toimisi edelleen, vaikka uusi materiaali käsitellään eri tavalla. Kaikissa tapauksissa tämä ei tietenkään ole mahdollista, mutta kannattaa mielestäni aina, kun se vain suinkin teknisesti onnistuu kohtuullisella vaivalla. Nämä ovat toki vain henkilökohtaiset sivuni, mutta jos joskus samanlaisia tilanteita tulisi vastaan jollain kriittisemmillä sivuilla, olen ainakin pitänyt taitoja yllä. Tästä aiheesta pitäisikin ehkä kirjoitella jotakin myös opettajan roolissa, mutta tällä erää jätän asian hautumaan.

Tähän vielä kuva kahdella eri tavalla linkitettyinä em. asian demonstroimiseksi:

Ensin vanhalla tavalla:<figure style="width: 500px" class="wp-caption aligncenter">

[<img class="" title="My Everyday Stetson" src="http://farm9.staticflickr.com/8200/8171456182_29fddde3ea_d.jpg" alt="My Everyday Stetson" width="500" height="375" />](http://farm9.staticflickr.com/8200/8171456182_29fddde3ea_b_d.jpg "10.11.2012: 1024x768, Sketchbook PRO on iPad"){.}<figcaption class="wp-caption-text">10.11.2012: 1024x768, Sketchbook PRO on iPad</figcaption></figure> 

Sitten Photonic ShortCode (photos -asetuksella tagilla kohdistettuna ja yhteen kuvaan rajattuna &#8211; kikkailun makua, mihin selitys jäljempänä):

<p style="">
  Näistä esimerkeistä näkee, miten FancyZoom ja Photonicin oletuksena käyttämä <a style="" href="http://fancybox.net/" class="">FancyBox</a> eroavat toisistaan. Voi olla, että koetan virittää jälkimmäisen käyttöön myös vanhoihin kuviin, koskapa FancyZoomia ei enää kehitetä ja ominaisuudet ovat eittämättä melko rajoittuneet (se tosin olikin aikaan keskeinen syyni sen käyttöönottoon &#8211; yksinkertainen ja toimiva on monipuolista hankalaa ratkaisua parempi). Photonicin yksittäiselle kuvalle tarjoama kuvakoko ei kuitenkaan oikein miellytä minua. Asetuksissa selitetään jotakin &#8220;Flickrin tarjoamista kokovaihtoehdoista&#8221;, mutta minä en olekaan näyttämässä varsinaisesti thumbnailia, vaan kunnollisen katsottavan kuvan, jonka voi vielä klikata hieman suuremmaksi. Toki tämä onnistuu käyttämällä single photo -asetusta, mutta silloin klikkaus vie suoraan Flickriin eikä käytä Fancyboxia. Säätämisen tarvetta siis vielä. Yksi vaihtoehto on myös ottaa käyttöön FancyBox erikseen ja jokin Flickr-plugari erikseen. Katsotaan&#8230;<br style="" class="aloha-end-br" />
</p>

Hyvää päivänjatkoa!

<p style="">
  <b>Edit 29.11.2012 to 12:45</b>: Näköjään tekemäni muutos FancyZoomin koodin ei ainakaan täysin toimi tarkoitetulla tavalla. Koetetaan paikkailla siis vielä, ellen kerkiä sitten jo vaihtamaan johonkin muuhun skriptiin. Ensi viikolle varmaan joka tapauksessa jää. Työt ja muutto vievät loppuviikon.<br style="" />
</p>