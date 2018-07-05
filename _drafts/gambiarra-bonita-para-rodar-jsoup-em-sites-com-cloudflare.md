---
title: Gambiarra bonita para rodar Jsoup em sites com Cloudflare
categories:
  - Android
  - Libraries
author_staff_member: kelvin-tesche-ievenes
show_comments: true
date: 2018-07-05 00:00:00
---

<div style="width:100%;height:0;padding-bottom:48%;position:relative;"><iframe src="https://giphy.com/embed/V6R9thgW7fimI" style="position:absolute" class="giphy-embed" allowfullscreen="" width="100%" height="100%" frameborder="0"></iframe></div>

[via GIPHY](https://giphy.com/gifs/creepy-beard-zach-galifianakis-V6R9thgW7fimI)

> E ai meus rouxinóis do alasca

Lá estava eu fazendo meus minis projetos que provavelmente nunca irei terminar, quando de repente me deparo com um problema que talvez ja passaram.

**Usar Jsoup em páginas o o diabo do Cloudflare!**

Sim! há salvação para esse destruidor de apps da gambiarreira. A princípio eu pensava que não mas depois de muito tempo pesquisando descobri que um usuário do github chamado [zhkrb](https://github.com/zhkrb){: target="_blank"} criou uma [classe](https://github.com/zhkrb/cloudflare-scrape-Android) para resolver esse problema utilizando um [projeto](https://github.com/Anorov/cloudflare-scrape){: target="_blank"} do [Anorov](https://github.com/Anorov){: target="_blank"}.

<div style="width:100%;height:0;padding-bottom:55%;position:relative;"><iframe src="https://giphy.com/embed/l0HlFZ3c4NENSLQRi" style="position:absolute" class="giphy-embed" allowfullscreen="" width="100%" height="100%" frameborder="0"></iframe></div>

[via GIPHY](https://giphy.com/gifs/snl-saturday-night-live-snl-2016-l0HlFZ3c4NENSLQRi)

Massssss, nãi satisfeito com isso, quis ajudar ainda mais, então fiz uma biblioteca pra galero \\õ/ Então sem mais enrolações, como usar? como funfa? Bom.. primeiro você irá no meu repositório do GitHub [aqui](https://github.com/Kelvao/CloudflareScrape){: target="_blank"}.

Adicione o Jitpack no seu Gradle do projeto:

<script src="https://gist.github.com/Kelvao/cb797f53e4069e369a6a54cbbda75108.js"></script>

Agora adicione a biblioteca no seu Gradle do app:

<script src="https://gist.github.com/Kelvao/1261b490a30fae753a26be1371facecd.js"></script>