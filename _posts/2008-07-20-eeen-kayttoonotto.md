---
id: 312
title: Eee:n käyttöönotto
date: 2008-07-20T22:55:18+00:00
author: grove
layout: post
guid: http://teevati.net/btw/?p=312
permalink: /2008/07/20/eeen-kayttoonotto/
categories:
  - harrastukset
  - tietokoneet
tags:
  - USB
---
<figure style="width: 184px" class="wp-caption alignleft">[<img title="Asus Eee 4g + Ubuntu Eee 8.04 Hardy Heron" src="http://farm4.static.flickr.com/3229/2684575009_7febf528c5_m.jpg" alt="Asus Eee 4g + Ubuntu Eee 8.04 Hardy Heron" width="184" height="240" />](http://farm4.static.flickr.com/3229/2684575009_643f26f99f_o.jpg "Asus Eee 4g + Ubuntu Eee 8.04 Hardy Heron")<figcaption class="wp-caption-text">Asus Eee 4g + Ubuntu Eee 8.04 Hardy Heron</figcaption></figure> 

Uuden Eee-pc:ni käyttöönotto ei ollutkaan ihan niin suoraviivainen juttu kuin oikeastaan oletin. Alkuperäinen Linux-distro heräsi kyllä ihan nätisti, mutta heti ensimmäiseksi WLANin kanssa ilmeni ongelmia. Systeemi ei nimittäin tue WPA2:ta out-of-the-box, vaan se vaatii joidenkin päivitysten lataamista.

Tästä alkaa sen verran pitkä toimenpideketju, että pudotan jatkon pois etusivulta. Jos Linuxin virittäminen yleensä ja [SSD](http://fi.wikipedia.org/wiki/SSD "SSD - Wikipedia")-kiintolevylliseen [UMPC](http://fi.wikipedia.org/wiki/Ultrakevyt_tietokone "Ultrakevyt tietokone - Wikipedia")-tyyppiseen laitteeseen erityisesti kiinnostaa, kannattaa jatkaa lukemista. Kerron, mitä itse sovelsin ja kokoan vastaisen varalle linkit kaikkiin käyttämiini ja muihinkiin löytämiini relevantteihin  resursseihin.

<!--more-->

### WPA2 ratkaisee kaiken

Etsiskelin hetken Asuksen sivuilta ja törmäsin foorumeilla ketjuun, joka oli otsikoitu [[Problem] Connection to WPA2 solved on 4G/linux](http://vip.asus.com/forum/view.aspx?id=20080614055134328&board_id=20&model=Eee+PC+4G%2FLinux&SLanguage=en-us&page=1 "ASUSTeK Computer Inc.-Forum- Connection to WPA2 solved on 4G/linux"). Kyseisen ketju avausviestissä tarjotaan ratkaisu:

> <span class="content">Today i bought my eeePc and tried to connect to my wireless lan which is encrypted using WPA2 but it failed with &#8220;No DHCP offer&#8221; .<br /> I tried to update the system, after connecting with cable, but there where no real system updates to install, rather than a sype & speech commands update.</span>
> 
> But the eeePc is a Debian derivative so i connected the lan cable and enabled the cable connection, then i opened the **File Manager**, then clicked on menu **Tools &#8211;> Open console window** (be aware that this is a translation of my italian labels, so it can be really named slightly differently in english, so maybe look for synonims)
> 
> The shell appeared and then i updated the system using the debian way, running those commands:
> 
> <pre lang="bash">/home/user&gt; sudo apt-get update</pre>
> 
> [The program read some indexes from the internet and complains about some missing sources, specifically the source for special italian-edition packages, but i don&#8217;t care]
> 
> <pre lang="bash">/home/user&gt; sudo apt-get dist-upgrade</pre>
> 
> This time the program prints the list of the packages that will be updated, and in the list there are many core packages, including atheros wireless, yay!:-)
  
> It ask two confirmation, the first for the update, the second because it seems that asus repositories have changed their crypthografic keys since the linux was installed in my eeePc, so i do not care to this either so i&#8217;ve written  &#8216;yes&#8217; to let it proceed with the upgrade.
> 
> After completion (it took 5 five minutes), i  rebooted the pc  (disconnected the cable) and  then retried eith the usual wireless procedure and this time it worked !
> 
> Fantastic!
> 
> I now have also many more system updates on the update manager, so i loaded them also.
> 
> Hope it helps, good luck!

Ketjun muutamassa muussa viestissä pääosin kehuttiin toimnpiteen auttaneen, joten kokeilin sitä itsekin. Uudelleen käynnistykseen saakka kaikki näytti menevän hyvin. Sen jälkeen näkyviin tuli kuitenkin järjestelmän alapalkki ja musta työpöytä, jolla ei elänyt mikään. Tutkailin ja pohdiskelin jonkin aikaa, mitä  tehdä. Harkitsin palautustoimenpiteitä, mutta CD-asemattomassa koneessa niiden työläys johti siihen, että päätin kokeilla samalla vaivalla jotain muuta.

### Ubuntu Eee (8.04 Hardy Heron)<figure style="width: 100px" class="wp-caption alignright">

[<img title="Asus Eee 4G + Ubuntu Eee 8.04 Hardy Heron" src="http://farm4.static.flickr.com/3097/2685391476_bf2dea2b34_t.jpg" alt="Asus Eee 4G + Ubuntu Eee 8.04 Hardy Heron" width="100" height="67" />](http://farm4.static.flickr.com/3097/2685391476_e69ca4b10f_o.jpg "Asus Eee 4G + Ubuntu Eee 8.04 Hardy Heron")<figcaption class="wp-caption-text">Asus Eee 4G + Ubuntu Eee 8.04 Hardy Heron</figcaption></figure> 

Ensimmäinen hakukohteeni oli mahdollinen Ubuntun Eee-versio. Ensin ei meinannut löytyä mitään vakuuttavaa, mutta sitten tärppäsi. Ja lopulta vielä helppokäyttöisesti.  Suurimman osan seuraavista toimenpiteistä tarjosi yhdessä paikassa [UbuntuEee.com](http://www.ubuntu-eee.com "Ubuntu Eee").

Ensin täytyy [hankkia Ubuntu Eee](http://www.ubuntu-eee.com/index.php5?title=Get_Ubuntu_Eee "Get Ubuntu Eee - Ubuntu Eee"). Sitten siirtää se USB-tikulle, buutata ja asentaa. Tähän tapaan:

> <div style="float: left; font-size: 30px; font-weight: bold; min-height: 100px; height: 100px; width: 60px;">
>   <p>
>     1st
>   </p>
> </div>
> 
> <div style="padding: 5px; margin-left: 65px; background-color: #ffe1a2; min-height: 100px;">
>   <p>
>     <strong>DIRECT DOWNLOAD</strong>
>   </p>
>   
>   <ul>
>     <li>
>       <a class="external free" title="http://sourceforge.net/project/showfiles.php?group_id=213463" rel="nofollow" href="http://sourceforge.net/project/showfiles.php?group_id=213463">http://sourceforge.net/project/showfiles.php?group_id=213463</a>
>     </li>
>   </ul>
>   
>   <p>
>     <strong>TORRENT DOWNLOAD</strong>
>   </p>
>   
>   <ul>
>     <li>
>       <a class="external free" title="http://www.mininova.org/tor/1488818" rel="nofollow" href="http://www.mininova.org/tor/1488818">http://www.mininova.org/tor/1488818</a>
>     </li>
>   </ul>
>   
>   <p>
>     We recommend the Torrent Download.
>   </p>
>   
>   <p>
>     Filename: <tt>ubuntu-eee-804.iso</tt> MD5 checksum: <tt>5803c9e7a7af50d525fb55459766e026</tt></div> 
>     
>     <div style="float: left; font-size: 30px; font-weight: bold; min-height: 100px; height: 100px; width: 60px;">
>       <p>
>         2nd
>       </p>
>     </div>
>     
>     <div style="padding: 5px; margin-left: 65px; background-color: #e7d5ae; min-height: 100px;">
>       <p>
>         <strong>MOVE TO USB STICK</strong> &#8211; Optional: <a title="Install Ubuntu gutsy" href="http://www.ubuntu-eee.com/index.php5?title=Install_Ubuntu_gutsy">Install from CD or SD</a>
>       </p>
>       
>       <p>
>         Connect your USB Stick (1GB or more) to your computer and use this application to move Ubuntu Eee over to your USB stick:<br /> <a class="external text" title="http://downloads.sourceforge.net/unetbootin/unetbootin-eeeubuntu-windows-238.exe?modtime=1214975248&big_mirror=0" rel="nofollow" href="http://downloads.sourceforge.net/unetbootin/unetbootin-eeeubuntu-windows-238.exe?modtime=1214975248&big_mirror=0">Windows</a><br /> <a class="external text" title="http://downloads.sourceforge.net/unetbootin/unetbootin-eeeubuntu-linux-238?modtime=1214975255&big_mirror=0" rel="nofollow" href="http://downloads.sourceforge.net/unetbootin/unetbootin-eeeubuntu-linux-238?modtime=1214975255&big_mirror=0">Ubuntu / Linux</a> &#8211; <a title="How to: Using Unetbootin" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_Using_Unetbootin#Using">How do I use this?</a></div> 
>         
>         <div style="float: left; font-size: 30px; font-weight: bold; min-height: 100px; height: 100px; width: 60px;">
>           <p>
>             3rd
>           </p>
>         </div>
>         
>         <div style="padding: 5px; margin-left: 65px; background-color: #fff3c3; min-height: 100px;">
>           <p>
>             <strong>BOOT AND INSTALL</strong>
>           </p>
>           
>           <ol>
>             <li>
>               Insert the stick into your Asus Eee PC, start and press ESC a couple of times while the Asus boot screen is displayed. Select your USB stick from the list of bootable devices.
>             </li>
>             <li>
>               Select your language and follow the installation instructions.
>             </li>
>             <li>
>               Read the <a title="User Guides" href="http://www.ubuntu-eee.com/index.php5?title=User_Guides">user guides</a> for additional help and information
>             </li>
>             <li>
>               Enjoy! <a title="Ubuntu Eee:Site support" href="http://www.ubuntu-eee.com/index.php5?title=Ubuntu_Eee:Site_support">Like Ubuntu Eee? Please donate</a>
>             </li>
>           </ol>
>         </div></blockquote> 
>         
>         <p>
>           Ensimmäinen toimenpide lienee helppo. Toinenkaan ei tuota vaikeuksia, koska siihen tarjotaan valmis työkalu ja hyvät ohjeet. Ainoa, mikä pitää järjestää itse, on sopiva USB-tikku tai &#8211; kuten minun tapauksessani &#8211; esim. muistikortti ja USB-lukija. Latasin Windows XP -koneella Ubuntu Eee:n Live/asennus-paketin muistikortille, jonka sitten asetin Eee:n kortinlukijaan. Kolmannessa vaiheessa sitten vain startataan kone ja noudatetaan ohjeita.
>         </p>
>         
>         <p>
>           Kolmannen vaiheen kohta kolme (3.3) &#8220;Read the <a title="User Guides" href="http://www.ubuntu-eee.com/index.php5?title=User_Guides">user guides</a> for additional help and information&#8221; vaatiikin sitten hieman enemmän pohdiskelua. Ubuntu Eee:hän ei toki ole alunperin Eee:lle suunniteltu &#8211; tai pikemminkin Eee:tä ei ole suunniteltu sille &#8211; joten se on vielä selvästi keskeneräinen toisin kuin Ubuntu 8.04 Hardy Heron normaalissa työasemassa olisi. Myös SSD-järjestelmälevynä ja CD-aseman puuttuminen sekä alhainen näytön resoluutio tuottavat omat rajoituksensa tai haasteensa. Seuraavaksi kerron, mihin niistä itse olen tähän mennessä ehtinyt puuttua.
>         </p>
>         
>         <h3>
>           Asetukset kohdalleen: pidä SSD elossa
>         </h3>
>         
>         <p>
>           Ensimmäisenä tartuin siihen seikkaan, että SSD:tä ja Flashia käyttävällä koneella kannattaa minimoida turhat kirjoitustoimenpiteet levylle. Siispä <a title="How to: reduce swappiness - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_reduce_swappiness">How to: reduce swappiness</a>:
>         </p>
>         
>         <blockquote>
>           <p>
>             Open up run (Alt+F2) and write:
>           </p>
>           
>           <pre lang="bash">gksudo gedit /etc/sysctl.conf</pre>
>           
>           <ul>
>             <li>
>               At the bottom of the file, add this line:
>             </li>
>           </ul>
>           
>           <pre lang="bash">vm.swappiness=0</pre>
>           
>           <ul>
>             <li>
>               Save and close
>             </li>
>           </ul>
>           
>           <ul>
>             <li>
>               You can put a comment above it like this, to remind yourself at a later date why you changed it:
>             </li>
>           </ul>
>           
>           <pre lang="bash"># To reduce wear of flash disk, added Joe Bloggs 22/05/2008</pre>
>           
>           <p>
>             NOTE: This does not disable swapping completely
>           </p>
>         </blockquote>
>         
>         <p>
>           Seuraava toimenpide (<a title="How to: make the fstab changes - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_make_the_fstab_changes">How to: make the fstab changes</a>) koskee samaa tavoitetta ja selittää ensin:
>         </p>
>         
>         <blockquote>
>           <h1>
>             <span class="mw-headline">Why make fstab changes</span>
>           </h1>
>           
>           <p>
>             Ubuntu&#8217;s standard installation doesn&#8217;t take <a class="external text" title="http://en.wikipedia.org/wiki/Solid-state_drive" rel="nofollow" href="http://en.wikipedia.org/wiki/Solid-state_drive">SSDs</a> (aka flash drives) into account. Flash drives are faster than regular hard drives, but their life time is reduced by the number of times it&#8217;s written to. Ubuntu likes writing to the hard drive all the time: temporary files and just a little write here and there in between, to keep the drive alive. This behavior is not wanted by SSD owners though. These changes here fixes that. Other changes that reduce the number of writes are:
>           </p>
>           
>           <ul>
>             <li>
>               Use ext2 instead of ext3 for the partition
>             </li>
>             <li>
>               <a title="How to: reduce swappiness" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_reduce_swappiness">Reduce swapiness</a>
>             </li>
>           </ul>
>         </blockquote>
>         
>         <p>
>           Ensimmäistä mainituista muista toimenpiteistä en aio tehdä, koska perusteluja on myös toiseen suuntaan. Jälkimmäisen puolestaan jo tähän tein, kuten edeltä selviää. Mutta Hardy Heronin tapauksessa seuraavaksi näin:
>         </p>
>         
>         <blockquote>
>           <ul>
>             <li>
>               Open up a terminal and write:
>             </li>
>           </ul>
>           
>           <pre lang="bash">gksudo gedit /etc/fstab</pre>
>           
>           <p>
>             [Tästä jätin Gutsya koskevan osuuden pois&#8230;]
>           </p>
>           
>           <ul>
>             <li>
>               Add these lines to the end of the file (<strong>Hardy and Gutsy</strong>)
>             </li>
>           </ul>
>           
>           <pre lang="bash">tmpfs     /var/log       tmpfs     defaults,noatime        0 0
tmpfs     /tmp           tmpfs     defaults,noatime        0 0
tmpfs     /var/tmp       tmpfs     defaults,noatime        0 0</pre>
>           
>           <ul>
>             <li>
>               That will send most log and temporary stuff, which changes a lot, into a temporary file system in RAM, which will be lost every time you shut down or reboot. Typically, that is not important, and does avoid a lot of write cycles to the flash disk.
>             </li>
>           </ul>
>         </blockquote>
>         
>         <p>
>           Tämän jälkeen on muiden tviikkausten vuoro.
>         </p>
>         
>         <h3>
>           Virranhallinta
>         </h3>
>         
>         <p class="firstHeading">
>           Koska Eee on ihan oma alustansa (Intelin Atom jne&#8230;), ei Ubuntu oletuksena osaa sammuttaa sitä kunnolla. Näyttö menee pimeäksi, mutta virrat jäävät päälle. Siispä <a title="Fix: The shutdown on hardy - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=Fix:_The_shutdown_on_hardy">Fix: The shutdown on hardy</a>:
>         </p>
>         
>         <blockquote>
>           <h2>
>             Fixing the shutdown hardy (may work on older versions of ubuntu)
>           </h2>
>           
>           <p>
>             When you install, Ubuntu doesn&#8217;t shut down properly. Shutting down your Eee will make the screen turn off, but does not cut the power. So
>           </p>
>           
>           <p>
>             Add:
>           </p>
>           
>           <pre lang="bash">rmmod snd-hda-intel</pre>
>           
>           <p>
>             at the beginning of the <strong>/etc/init.d/halt</strong> script in order to make the Eee shutdown properly.
>           </p>
>           
>           <p>
>             <a name="A_slightly_cleaner_solution"></a>
>           </p>
>           
>           <h3>
>             A slightly cleaner solution
>           </h3>
>           
>           <p>
>             Create a new script as <strong>/etc/init.d/eeepc</strong>, with the following contents:
>           </p>
>           
>           <pre lang="bash"> #!/bin/bash
 case $1 in
 stop)
 rmmod snd-hda-intel

 ;;
 *)
 esac</pre>
>           
>           <p>
>             Don&#8217;t forget to make it executable (chmod +x)
>           </p>
>           
>           <p>
>             Now in /etc/rc0.d (scripts run at shutdown), create a symbolic link named <strong>K60eeepc</strong>, pointing to <em>../init.d/eeepc</em> By renaming the symbolic link, one can control exactly when the module is removed.
>           </p>
>           
>           <pre lang="bash">ln -s /etc/init.d/eeepc /etc/rc0.d/K60eeepc</pre>
>           
>           <p>
>             That script can also be used for running other Eee-specific stuff at startup, shutdown&#8230;
>           </p>
>         </blockquote>
>         
>         <p>
>           Koetin näistä jälkimmäistä eli tuota hieman puhtaampaa tai elegantimpaa ratkaisua. Ainakaan äskeisellä sammutuskerralla se ei tosin näyttänyt toimivan, mutta tarkistan viekä toimineeni oikein ja etsin muita ratkaisuja vasta sitten. Oletetavasti tämä on kuitenkin pätevä tekniikka. On myös mahdollista, että en vain odottanut tarpeeksi kauan.
>         </p>
>         
>         <p>
>           On hyvä, että kone sammuu kunnolla, jottei se vahingossa jää kuluttaman akkuaan tyhjäksi. Sen lisäksi lienee kuitenkin toivottavaa, että turhaan virtaa kuluttavia toimenpiteitä tehdään mahdollisimman vähän. Siksi seuraaavaksi noudatin ohjetta <a title="Get the most of the battery - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=Get_the_most_of_the_battery">Get the most of the battery</a>:
>         </p>
>         
>         <blockquote>
>           <p>
>             These changes allow the CPU to sleep for longer when idle, saving power. For more information see the website for the &#8220;powertop&#8221; tool, <a class="external free" title="http://www.lesswatts.org/projects/powertop/" rel="nofollow" href="http://www.lesswatts.org/projects/powertop/">http://www.lesswatts.org/projects/powertop/</a>
>           </p>
>           
>           <p>
>             [Tästä jätin pois osuuden, joka ei ilmeisesti ole valmiiksi viritetyllä Ubuntu Eee:llä tarpeen.]
>           </p>
>           
>           <h2>
>             15 sec dirty_writeback_centisecs
>           </h2>
>           
>           <p>
>             This reduces how often linux writes data to HDD. The value is in 100&#8217;ths of a second. Thus 1500 is 15 seconds. See <a class="external free" title="http://www.westnet.com/~gsmith/content/linux-pdflush.htm" rel="nofollow" href="http://www.westnet.com/%7Egsmith/content/linux-pdflush.htm">http://www.westnet.com/~gsmith/content/linux-pdflush.htm</a>
>           </p>
>           
>           <ul>
>             <li>
>               Open up a terminal and write:
>             </li>
>           </ul>
>           
>           <pre lang="bash">sudo gedit /etc/sysctl.conf</pre>
>           
>           <ul>
>             <li>
>               Add the line:
>             </li>
>           </ul>
>           
>           <pre lang="bash">vm.dirty_writeback_centisecs=1500</pre>
>           
>           <ul>
>             <li>
>               This takes effect next time you restart the laptop
>             </li>
>           </ul>
>           
>           <h2>
>             15 sec ext3 commit interval
>           </h2>
>           
>           <p>
>             This is useful if you use the EXT3 filesystem. EXT3 is a journaling filesystem, which means it will write its journal to the disk by default every 5 seconds.
>           </p>
>           
>           <p>
>             See man mount. commit=nrsec &#8211; Sync all data and metadata every nrsec seconds. The default value is 5 seconds. Zero means default.
>           </p>
>           
>           <ul>
>             <li>
>               Open /etc/fstab
>             </li>
>           </ul>
>           
>           <pre lang="bash">  sudo gedit /etc/fstab</pre>
>           
>           <ul>
>             <li>
>               Find root filesystem. It is something like:
>             </li>
>           </ul>
>           
>           <pre lang="bash">  UUID=e50b7067-d585-49e0-af2b-167649dda172 / ext3 defaults,errors=remount-ro 0</pre>
>           
>           <ul>
>             <li>
>               Add the commit option &#8220;<strong>commit=15</strong>&#8220;
>             </li>
>           </ul>
>           
>           <pre lang="bash">  UUID=e50b7067-d585-49e0-af2b-167649dda172 / ext3 defaults,errors=remount-ro,commit=15 0</pre>
>         </blockquote>
>         
>         <p>
>           Tästä osuudesta kannattaa huomata, että helpommalla saattaa päästä, jos kirjoittaa ensimmäisen komennon kummassakin tapauksessa Suorita (Run) -kehotteeseen muodossa:
>         </p>
>         
>         <pre lang="bash">gksudo gedit</pre>
>         
>         <p>
>           Tietysti, jos terminaali on jo auki, niin mikäpä siinä.
>         </p>
>         
>         <p>
>           Sitten vielä yksi toimenpide, joka ei varsinaisesti koske virranhallintaa, mutta koneen käynnistämistä kyllä. Lienee tarpeetonta odottaa joka kerta kolme sekuntia, kun GRUB odottelee, jos haluaisit tehdä jotain. Tällä koneellahan tuskin on multiboot-asetelmaa. Siispä <a title="How to: optimize boot speed - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_optimize_boot_speed">How to: optimize boot speed</a>:
>         </p>
>         
>         <blockquote>
>           <h2>
>             <span class="mw-headline">Boot Time Optimizations </span>
>           </h2>
>           
>           <p>
>             <a name="Skip_GRUB_loader.283_sec_waiting.29"></a>
>           </p>
>           
>           <h3>
>             <span class="editsection"><a title="Edit section: Skip GRUB loader(3 sec waiting)" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_optimize_boot_speed&action=edit&section=2"></a></span><span class="mw-headline">Skip GRUB loader(3 sec waiting) </span>
>           </h3>
>           
>           <ul>
>             <li>
>               Open up the Terminal and open a file
>             </li>
>           </ul>
>           
>           <pre lang="bash">sudo gedit /boot/grub/menu.lst</pre>
>           
>           <ul>
>             <li>
>               Edit where it says
>             </li>
>           </ul>
>           
>           <pre lang="bash">timeout 3</pre>
>           
>           <p>
>             to
>           </p>
>           
>           <pre lang="bash">timeout 0</pre>
>           
>           <ul>
>             <li>
>               Save and close
>             </li>
>           </ul>
>           
>           <h3>
>             Read Ahead Optimization
>           </h3>
>           
>           <ol>
>             <li>
>               Add the boot option &#8220;profile&#8221; when starting up the computer <ol>
>                 <li>
>                   Hit &#8220;Esc&#8221; when it says &#8220;GRUB loading&#8221;
>                 </li>
>                 <li>
>                   Hit &#8220;e&#8221; to edit
>                 </li>
>                 <li>
>                   Hit &#8220;down arrow&#8221; once until you&#8217;re on the &#8220;kernel&#8221; line
>                 </li>
>                 <li>
>                   Hit &#8220;e&#8221; to edit
>                 </li>
>                 <li>
>                   You should now be editing a long line of text. Add a space and &#8220;profile&#8221; at the end
>                 </li>
>                 <li>
>                   Hit &#8220;Enter&#8221; to use this new option for this boot
>                 </li>
>                 <li>
>                   Hit &#8220;b&#8221; to boot
>                 </li>
>               </ol>
>             </li>
>           </ol>
>           
>           <p>
>             Do this only once when changing kernels. It tries to optimize boot time but this process takes a while.
>           </p>
>         </blockquote>
>         
>         <p>
>           Näistä toimenpiteistä jälkimmäistä en vielä tehnyt. Osasyy on se, että ilman kolmen sekunnin viivettä GRUB ehti ohi ennen kuin ehdin painaa mitään. Ehkäpä tämä siis kannattaisi oikeastaan tehdä ensin ja poistaa viive vasta sitten.
>         </p>
>         
>         <h3>
>           Muuta
>         </h3>
>         
>         <p>
>           Vielä yksi toimenpide on tullut tehtyä. Näytön ollessa pieni, ikkunoiden koko voi välillä olla ongelma. Siispä helpotetaan niiden siirtelyä totetutamalla <a title="How to: disable Y constraint - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=How_to:_disable_Y_constraint">How to: disable Y constraint</a>:
>         </p>
>         
>         <blockquote>
>           <p>
>             Disable the vertical constraint of windows so you can reach the buttons at the bottom of tall dialog boxes and such by holding the <alt> key and dragging windows around!
>           </p>
>           
>           <p>
>             Write this in Terminal:
>           </p>
>           
>           <pre lang="bash">gconftool-2 --type bool --set /apps/compiz/plugins/move/allscreens/options/constrain_y 0</pre>
>         </blockquote>
>         
>         <p>
>           Kovin paljoa tämän enempää en ole vielä ehtinyt tehdä. Ubuntu Eee:n asensin vasta tänä aamuna ja sen jälkeen olin poissa kotoa pitkälle aamusta alkuiltapäivään. Firefoxia kyllä kerkesin jo alkaa viritellä. Fission, Flashblock, Stop-or-Reload Button ja Tiny Menu tuli asennettua. Kaksi viimeistä pyrkii erityisesti näyttöpinta-alan säästämiseen. Luultavasti samasta syystä estän myös välilehtien käytön, vaikka muuten käytän niitä intensiivisesti. Tai sitten pitää surffata koko näytöllä, jotta mitkään palkit eivät syö tilaa.
>         </p>
>         
>         <p>
>           Logitech VX Revolution pikkuhiireni toimii Eee:n kanssa ongelmitta, joten sitä luultavasti tulee hyödynnettyä jonkin verran. Pikkuisen nimittäin on tunnoton tuo kosketuslevy ja sama pätee myös sen alla olevaan yksiosaan nappiin, joka palvelee kahden napin virkaa.
>         </p>
>         
>         <p>
>           Vielä pari pientä huomiota. Canonical <a title="Canonical Showcases Ubuntu Netbook Remix at Computex | Ubuntu" href="http://www.ubuntu.com/news/netbook-remix">on jo jokin aika sitten julkaissut</a> esiversion UMPC-käyttöön sovitetusta Ubuntun <a title="Ubuntu Netbook Remix in Launchpad" href="https://launchpad.net/netbook-remix">Netbook Remix -käyttöliittymä</a>stä. Lainaus <a title="Interview: Mark Shuttleworth, founder of Ubuntu | Technology | The Guardian" href="http://www.guardian.co.uk/technology/2008/may/22/internet.software">Mark Shuttleworthin haastattelusta</a>:
>         </p>
>         
>         <blockquote>
>           <p>
>             <strong>TG: Will you be coming out with a tailored version of Ubuntu for the ultraportable sector?</strong>
>           </p>
>           
>           <p>
>             <strong>MS</strong> We&#8217;re announcing it in the first week of June. It&#8217;s called the Netbook Remix. We&#8217;re working with Intel, which produces chips custom-made for this sector.
>           </p>
>         </blockquote>
>         
>         <p>
>           Toistaiseksi sitä ei vielä suositella &#8220;tuotantokäyttöön&#8221;, vaan vain testattavaksi, mutta hyvältä silti vaikuttaa. Ehkäpä testaan sitä tässä lähipäivinä (<a title="How to install and use the Netbook Remix interface - Ubuntu Eee" href="http://www.ubuntu-eee.com/index.php5?title=How_to_install_and_use_the_Netbook_Remix_interface">How to install and use the Netbook Remix interface</a>).
>         </p>
>         
>         <p>
>           Ja lopuksi:
>         </p>
>         
>         <p>
>           Ilmeisesti <a title="eee.ricey.co.uk" href="http://eee.ricey.co.uk/">Riceyn skriptin</a> suorittamat toimenpiteet on Ubuntu Eee:ssä jo hoidettu, mutta siltä varalta, ettei ole, tarjoan tämänkin resurssin tässä koosteessa itse kullekin tutkittavaksi. Nyt sen sivuja juuri vilkaistessani muistin taas, että kannattanee tarkistaa, ettei Ubuntu Eee turhaan etsi CD-asemaa, jota ei ole. Taidanpa siis vielä käydä Riceyn ohjeet läpi siltä varalta, että skriptissä tai lisäohjeissa on jotain, mitä en ole tehnyt, mutta kannattaisi. Palataan asiaan, jos jotain löytyy ja joka tapauksessa, kunhan käyttökokemusta kertyy.
>         </p>
>         
>         <p>
>           Tämän viestin kuvat Flickrissä: <a title="R0016882 on Flickr" href="http://flickr.com/photos/teevati/2684575009">R0016882</a>, <a title="R0016888 on Flickr" href="http://flickr.com/photos/teevati/2685391476">R0016888</a>.
>         </p>