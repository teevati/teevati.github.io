---
id: 305
title: 'Opetus: älä modaa corea (ellei ole aivan pakko)'
date: 2008-07-20T18:47:35+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=305
permalink: /2008/07/20/opetus-ala-modaa-corea-ellei-ole-aivan-pakko/
categories:
  - harrastukset
  - tietokoneet
  - ylläpito
tags:
  - WordPress
---
[Eilen päivitin Tarskin versioon 2.2](http://teevati.net/btw/2008/07/19/tarski-22/ "BTW : Tarski 2.2"). Tänään sitten huomasin uuden kuvallisen viestin lisättyäni, että FancyZoom ei toiminutkaan. Syyhän oli tietysti se, että olin lisännyt FancyZoomin javaskriptien latauksen käsin templaten headeriin. Samoin onLoadin body-tagiin.

Nytpähän sitten korjasin virheeni: skriptit hoituvat head-tagin sisälle pluginilla ja onloadille etsin jonkin elegantin ratkaisun myöhemmin. Käytin kyllä melko paljon aikaa erilaisten ratkaisujen etsimiseen, mutta WordPress tai Tarski eivät kumpikaan tunnu tarjoavan **helppoa** tapaa lisätä body-tagiin mitään muuta kuin id- tai class-tietoja. Siispä onLoad on yhä modattuna suoraan Tarskin coreen, kun en muutakaan saanut toimimaan.

Mahtava pluginini näyttää tältä:

<pre lang="php">/*
Plugin Name: Add FancyZoom
Plugin URI: http://teevati.net/
Description: Adds Fancy Zoom calls to html>head.
Version: 1.0
Author: Taavetti Lehtomäki
Author URI: http://teevati.net/
*/

function add_fancyzoom () {
    echo '
    
    
';

}

add_action('tvti_head', 'add_fancyzoom');</pre>