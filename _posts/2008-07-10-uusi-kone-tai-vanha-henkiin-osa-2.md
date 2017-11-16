---
id: 40
title: 'Uusi kone tai vanha henkiin&#8230; &#8211; osa 2'
date: 2008-07-10T11:04:43+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=40
permalink: /2008/07/10/uusi-kone-tai-vanha-henkiin-osa-2/
categories:
  - tietokoneet
tags:
  - muisti
  - ongelma
  - RAM
  - tietokoneet
  - USB
  - Windows
  - Windows XP
  - XP
---
[Eilen kertoilin konetilanteestani](http://teevati.net/btw/?p=39 "Uusi kone tai vanha henkiin…") ja nyt voi ilokseni todeta, että ainakin osa toimenpiteistä vaikuttaisi tehonneen. En ehtinyt vielä kokeilla kaikkea, mutta käynnistys tuntuisi nyt onnistuvan kerralla (ilman vaihtelevaa määrä BSOD-kierroksia).

Suorittamani toimenpiteet olivat:

  1. kaikki USB-laitteet USB2.0-portteihin
  2. USB-ajureiden poistaminen ja uudelleen tunnistaminen laitehallinnassa
  3. uusimman ATI Catalystin asentaminen
  4. BIOS-asetusten tarkistus
  5. Catalystin asetusten säätäminen

Vaiheen 1 ja 2  jälkeen mikään ei vielä muuttunut. Vaiheessa 4 tarkistin kaikki asetukset, mutta oleellisista vga fast-write oli jo disabled, vaihdoin kuitenkin AGP-näytönohjaimen oletukseksi ja lisäksi disabloin quick bootin (ts. kone kelaa muistin läpi ennen kuin aloittaa muut toimet &#8211; kahdella gigalla se vie hetken aikaa). Vaiheet 3 ja 4 toivat kuitenkin mukanaan kaksi muutosta: ei BSODia buutissa eikä kolmas näyttö enää suostunut toimimaan (PCI-väylään kytketty ikivanha ATI Rage II -näytönohjain, joka ei ilmeisesti käynnisty ollenkaan, jos AGP on oletuksena). Vaiheen 5 jälkeen koetin vielä muuttaa pari BIOS-asetusta ennen kuin buuttasin Windowsiin asti. Plug&#8217;n&#8217;Play Aware OS -asetuksen enabloiminen ei kuitenkaan vaikuttanut kolmanteen näyttöön mitään. Catalystin asetuksissa disabloin agp writen molempien näyttöjen osalta.

 Kaiken tämän jälkeen päätin sitten vielä kokeilla olisiko USB:lle tapahtunut jotain &#8211; ja olihan sille! Kokeilin ensin tikulla, josta XP ei herjannut, notta se voisi toimia nopeammin USB2.0-portissa. Tästä yllättyneenä kokeilin vielä siirtää kuvia suoraan pokkarikamerastani ja ne siirtyivätkin rivakasti. Näyttäisi siis siltä, että kaksi ongelmaa tuli ratkaistuksi yhden illan aikana, vaikka aikaa ei ollut edes käytettävissä kovin paljon.

Tänään varmaankin irrotan PCI-näytönohjaimen koneesta kokonaan ja siirryn toistaiseksi &#8220;vain&#8221; kahden näytön käyttöön. Lisäksi, jos em. korjaukset tuntuvat edelleen olevan kohdallaan, kokeilen varmaan jälleen, jos kolmas giga muistia kelpaisi systeemille. Catalystin kaatuminenhan se ongelma aiemmin oli eli uusimman version ja asetusmuutosten jälkeen toivoa voisi olla. Quick bootin enablointiakin varmaan kokeilen jossain välissä nähdäkseni oliko sillä osansa BSODin katoamisessa vai ei. Kolmen gigan kanssa olisi kuitenkin kivempaa, jos sen läpikäyntiä ei startissa tarvitsisi odotella, mutta toki se on BSODia parempi, jos valita pitää. Jos vielä äänikortin särinäkin kaikkoaisi, niin vanha kone saisi varmasti lisäaikaa vielä melkoisesti. Uuden kyllä ehtii hankkia myöhemminkin, jos vanha vain toimii kunnolla.

Tiivistettynä tilanne eilen illalla: kone käynnistyy kerralla ilman BSODia ja USB2.0 toimii, mutta kolmas näyttö ei. Muiden ongelmien osalta testaus on vielä kesken.