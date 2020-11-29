---
title: Utiliser votre téléphone comme rétroprojecteur
date: 2020-04-07
image: /phone/bricolage.jpg
tags:
- visio
- android
- obs
- screencast
- youtube
---


# L'idée

L'idée est très simple : posez votre téléphone à une vingtaine de centimètres au-dessus du bureau (par exemple sur un tas de livres) et utilisez-le comme rétroprojecteur pour filmer et transmettre sur internet ce que vous écrivez.

{{< card-deck >}}
  {{< card-img src="/phone/idea2.jpg" descr="Installation avec des livres comme support" class="figure">}}
  {{< card-img src="/phone/idea1.jpg" descr="La distance idéale est de l'ordre de 20 cm" class="figure">}}
{{< /card-deck >}}

# Utilisations possibles

{{< videotag src="/phone/possible.mp4" class="col-8 offset-2 float-lg-right ml-lg-5 col-lg-4" >}}

On peut utiliser le téléphone ainsi installé pour :

- transmettre en direct ce qu'on écrit à un collaborateur ou à un groupe d'étudiants ;
- enregistrer des vidéos montrant ce qu'on écrit tout en commentant nos écrits ;
- dessiner sur des figures pré-imprimées ;
- alterner des présentations en pdf et des écritures faites à la main ;
- afficher des passages de livres ;
- prendre une photo d'une formule, d'un dessin, et la poster sur un chat ;

et ainsi de suite.

## Le téléphone seul

Si vous n'avez pas d'ordinateur, ou si vous n'avez pas envie de vous embêter à renvoyer l'image de votre téléphone sur votre écran d'ordinateur *(voir plus bas)* vous pouvez utiliser le téléphone seul.

### Visio-conférence

Tous les logiciels de visio comme [Jitsi Meet](https://jitsi.org/downloads/) (utilisé par [Renater Rendez-vous](https://rendez-vous.renater.fr/) et par [Framatalk](https://framatalk.org/)), Skype, Duo, WhatsApp, Whereby, Zoom, Webex ... vous permettront de partager vos écrits avec vos collaborateurs et avec vos étudiants en direct.

Je n'ai pas testé, mais probablement BigBlueButton (utilisé par [PLM webconf](https://plmwebconf.math.cnrs.fr) et Moodle) fonctionne aussi.

{{< card-deck >}}
  {{< card-img src="/phone/RdV.jpg" descr="Jitsi sur Rendez-vous" class="figure">}}
  {{< card-img src="/phone/Skype.jpg" descr="Skype" class="figure">}}
  <div class="w-100 d-none d-sm-block d-lg-none"><!-- passage à la ligne jusqu'à lg --></div>
  {{< card-img src="/phone/WhatsApp.jpg" descr="WhatsApp" class="figure">}}
  {{< card-img src="/phone/Duo.jpg" descr="Duo" class="figure">}}
{{< /card-deck >}}

**Avantage :** la simplicité.

**Inconvénients :** la qualité des vidéos transmises (aucun de ces logiciels n'autorise la mise au point fixe ni les ajustements de la luminosité, de plus la résolution souvent n'est pas au top).

**Conseils :**

- écrivez gros et laissez l'image « se stabiliser » entre deux écritures ;
- fixez l'orientation en « portrait ».

### Diffuser sur des plates-formes vidéo

Vous pouvez diffuser en direct votre caméra sur des services vidéo tels YouTube, Viméo, Dailymotion... en utilisant des logiciels spécialisés comme [Streamlabs](https://streamlabs.com/mobile-app) *(la version mobile de OBS)* ou autres.

**Avantages :**

- la qualité de la vidéo est meilleure qu'en visio (par exemple 1280×720);
- la vidéo peut être vue en simultané par plusieurs dizaines de personnes sans problème de connexion ;
- la vidéo peut être visionnée en différé.

**Inconvénients :**

- il faut maîtriser le service vidéo utilisé ;
- la majorité de ces plates-formes sont payantes pour diffuser dessus ;
- la prise en main des logiciels mobiles de streaming n'est pas toujours évidente.

**Conseils :** si vous pouvez passer par un ordinateur dans ce cas, c'est fortement préférable.

### Enregistrer une vidéo

Vous pouvez simplement enregistrer une vidéo avec ce que vous écrivez et commenter en même temps. Il peut s'agir d'une longue vidéo de cours ou d'un exposé, ou d'une vidéo de quelques secondes pour illustrer quelque chose de façon dynamique.

{{< youtube id="jYCSzVA4Y6U" class="col-8 mx-auto text-center float-lg-right ml-lg-5 col-lg-4" descr="Cette vidéo de 23 secondes pèse 1Mb, car elle a été enregistrée avec 10 images/s et un débit de 350Kbps sans son." >}}

**Avantages :**

- convient aux vidéos très courtes d'illustration ;
- l'application caméra fournie avec le téléphone peut convenir, surtout si la mise au point fixe est possible.
- Vous pouvez éditer (couper des morceaux) la vidéo avant de l'envoyer ou de la publier.

**Inconvénients :**

- ne convient pas aux communications en direct ;
- les fichiers ainsi produits risquent d'être gros ;

**Conseils :**

- utiliser un logiciel qui permet la mise au point fixe (tels [HedgeCam 2](https://play.google.com/store/apps/details?id=com.caddish_hedgehog.hedgecam2) ou [Open Camera](https://play.google.com/store/apps/details?id=net.sourceforge.opencamera) pour Android);
- utiliser un logiciel qui permet de fixer la mesure de la lumière ;
- régler la dimension de la vidéo à 1280×720 ;
- régler le nombre d'images par seconde à moins de 15 (si possible entre 5 et 10);
- régler le débit à moins de 1Mo/s (si possible);
- si vous allez faire une vidéo très courte d'illustration, couper le son.

### Prendre une photo

Vous pouvez ainsi insérer un dessin fait à la main dans un PDF, poster une formule sur un chat ou prendre en photos vos écrits pendant un cours en direct pour diffuser après les notes.

**Conseil :** régler la résolution à 1-2Mo et la qualité du jpeg à 35/100 (c'est suffisant).

## Via l'ordinateur

Une fois affiché sur l'ordinateur vous pouvez partager l'écran de votre téléphone comme vous partagez toute autre application (PDF, GeoGebra, Jupyter Notebook...). La seule chose à savoir est comment afficher l'écran du téléphone sur son ordinateur.

### Afficher l'écran d'un smartphone Android sur ordinateur

Il y a essentiellement deux méthodes : par câble USB ou via Wi-Fi.

#### Par câble USB

Je connais une seule application qui permet de faire ça, le [scrcpy](https://github.com/Genymobile/scrcpy). Les instructions pour son installation, ainsi que du débogueur `adb`, sont sur la page du projet : pour [Linux](https://github.com/Genymobile/scrcpy#linux), pour [Mac](https://github.com/Genymobile/scrcpy#macos) ou pour [Windows](https://github.com/Genymobile/scrcpy#windows).

Une fois installé, vous devez :
1. [Autoriser votre smartphone Android à être débogué par USB](https://www.google.fr/search?q=android%20autoriser%20le%20debogage%20usb).
2. Brancher votre téléphone avec un câble USB à votre ordinateur.
3. Lancer `scrcpy` : normalement une fenêtre affichant l'écran de votre téléphone s'ouvre.

#### Via Wi-Fi

Il existe plusieurs logiciels pour diffuser l'écran de votre smartphone via le réseau. Moi j'utilise [Screen Stream over HTTP](https://play.google.com/store/apps/details?id=info.dvkr.screenstream).

Pour les téléphones sous Android j'ai fait un tutoriel :

Une fois installé, vous devez :
1. Connecter votre téléphone sur le même réseaux que votre ordinateur (sans ça la suite ne fonctionnera pas).
2. Lancer `Screen Stream over HTTP` sur votre téléphone, puis activer la diffusion.
3. Ouvrer dans votre navigateur l'adresse indiqué dans `Screen Stream over HTTP` qui devrait être de la forme ` http://192.168.X.XX:8080`.

L'avantage de cette méthode par rapport à la connexion par USB est ça simplicité (pas besoin d'activer le mode développeur du téléphone ni d'installer un logiciel sur l'ordinateur). Son principal inconvénient est l'utilisation d'une bonne partie de la bande passante et l'obligation d'avoir l'ordinateur et le téléphone connectés sur le même réseaux.

#### Le tutoriel vidéo

Ces deux méthodes pour afficher l'écran de votre smartphone Android sur un PC sous Windows sont présentés dans ce tutoriel :

<div class="row">
  <div class="col-6 offset-3 mb-4">
  {{< card-video id="JfWcBVhYmt4" descr="Cette vidéo parle de tablette, mais c'est la même démarche pour un téléphone sous Android." class="">}}
  </div>
</div>

### Afficher l'écran d'un iPhone sur un Mac

Je n'ai pas d'iPhone mais je sais que [c'est possible](https://www.google.com/search?q=mirror+iphone+screen+on+mac).

### Partage direct d'écran ou de fenêtre

Comme déjà dit, une fois l'écran de votre téléphone affiché sur l'ordinateur, vous pouvez :

- partager l'écran tout entier (en mettant par exemple côte-à-côte votre un PDF et le téléphone);
- ou partager juste la fenêtre de votre téléphone.

{{< card-deck >}}
  {{< card-img src="/phone/phone_and_pdf.jpg" descr="Partage du bureau avec PDF et écriture à la main." class="figure">}}
  {{< card-img src="/phone/jupyter_and_phone.jpg" descr="Partage du bureau avec Jupyter Notebook et écriture à la main." class="figure">}}
{{< /card-deck >}}


**Avantages :**

- vous pouvez utiliser une application qui permet d'avoir une mise au point manuelle et autres réglages qui permettent d'améliorer la qualité de l'image (tels [HedgeCam 2](https://play.google.com/store/apps/details?id=com.caddish_hedgehog.hedgecam2) ou [Open Camera](https://play.google.com/store/apps/details?id=net.sourceforge.opencamera) pour Android) ;
- vous avez la possibilité de partager d'autres applications en plus de votre écriture.

**Inconvénients :**

- il faut apprendre comment afficher l'écran de son téléphone sur son ordinateur ;
- si vous le faites par USB (ce que je vous conseille), il y a encore un câble qui traîne.

**Conseils :**

- utilisez une application qui vous permet de fixer la mise au point et faites-le ;
- si nécessaire activez la lampe de votre téléphone pour éclairer la feuille ;
- fixez la rotation de votre téléphone en « paysage ».

### Partage avec OBS

[OBS Studio](https://obsproject.com/), abrégé en OBS, est un logiciel libre et open source de capture d'écran et de streaming pour Linux, MacOS et Windows. Vous pouvez l'utiliser pour diffuser votre écran et/ou votre webcam sur un serveur comme YouTube.

Il vous permet de :

- composer sur un seul écran plusieurs fenêtres (votre écriture à la main, votre webcam, un fichier pdf ...) ;
- appliquer des filtres sur vos fenêtres, comme « transformer en noir et blanc », « augmenter le contraste », « n'afficher qu'une portion de la fenêtre » et ainsi de suite ;
- préparer en avance des dispositions des fenêtres que vous pouvez utiliser lors de vos cours ;
- diffuser en direct et/ou enregistrer votre cours.

Voici quelques tutoriels sur OBS que j'ai faits ces dernières semaines :

{{< card-deck >}}
  {{< card-video id="VmQBG8oVWWg" descr="Préparation d'un cours en ligne avec OSB Studio" >}}
  {{< card-video id="O97yAReIz9Y" descr="Configuration OBS Studio pour l'enseignement en ligne" >}}
  {{< card-video id="SQtmb2gP32I" descr="Faire un cours en direct sur YouTube avec OBS studio" >}}
{{< /card-deck >}}


# Conseils

- Le téléphone ne doit pas être placé trop haut (à part si vous zoomez), car sinon le texte sera trop petit. La partie visible doit être de l'ordre de A6 (1/4 de A4).
- Si possible il faut fixer le focus et la mesure de la lumière, sinon chaque fois que votre main va rentrer dans le champ de vision ça va entraîner une perte du focus et un changement de la luminosité.
- Vous pouvez agrafer plusieurs 1/4 de feuille en un livret et scotcher la dernière à la table, pour que ça ne bouge pas quand vous écrivez.
- Il est préférable d'utiliser des feuilles blanches, car les feuilles à carreaux gènent la lisibilité et augmentent la taille de la vidéo.
- Si vous écrivez au crayon à papier, privilégiez les mines souples (2B), plus visibles. Sinon, utilisez des stylos Frixion (effaçables).
- Si vous décidez d'utiliser [HedgeCam 2](https://play.google.com/store/apps/details?id=com.caddish_hedgehog.hedgecam2), j'ai mis en ligne une [vidéo qui montre comment la configurer](https://youtu.be/841pDbmKNW0).

{{< card-deck >}}
  {{< card-img src="/phone/idea4.jpg" descr="Couper des feuilles A4 en 4 pour fabriquer un carnet." class="">}}
  {{< card-img src="/phone/idea3.jpg" descr="Scotcher la dernière page du carnet pour que ça ne bouge pas quand vous écrivez" class="">}}
  {{< card-img src="/phone/idea5.jpg" descr="Vous pouvez aussi délimité la partie visible dans le téléphone." class="">}}
  <div class="w-100 d-none d-sm-block"><!-- passage à la ligne jusqu'à lg --></div>
  {{< card-img src="/phone/supports.jpg" descr="À la place des livres on peut utiliser des supports dédiés." class="">}}
  {{< card-img src="/phone/bricolage.jpg" descr="Vous pouvez aussi bricoler un support qui prend moins de place est fait moins d'ombre que le tas de livres." class="">}}
{{< /card-deck >}}
