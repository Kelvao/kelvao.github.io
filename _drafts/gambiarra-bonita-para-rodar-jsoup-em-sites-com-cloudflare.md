---
title: Gambiarra bonita para rodar Jsoup em sites com Cloudflare
categories:
  - Android
  - Libraries
author_staff_member: kelvin-tesche-ievenes
show_comments: true
date: 2018-06-27 00:00:00
---

<div style="width:100%;height:0;padding-bottom:48%;position:relative;"><iframe src="https://giphy.com/embed/V6R9thgW7fimI" style="position:absolute" class="giphy-embed" allowfullscreen="" width="100%" height="100%" frameborder="0"></iframe></div>

[via GIPHY](https://giphy.com/gifs/creepy-beard-zach-galifianakis-V6R9thgW7fimI)

> E ai meus rouxin&oacute;is do alasca

L&aacute; estava eu fazendo meus minis projetos que provavelmente nunca irei terminar, quando de repente me deparo com um problema que talvez ja passaram.

**Usar Jsoup em p&aacute;ginas o o diabo do Cloudflare!**

Sim! h&aacute; salva&ccedil;&atilde;o para esse destruidor de apps da gambiarreira. A princ&iacute;pio eu pensava que n&atilde;o mas depois de muito tempo pesquisando descobri que um usu&aacute;rio do github chamado [zhkrb](https://github.com/zhkrb){: target="_blank"} criou uma [classe](https://github.com/zhkrb/cloudflare-scrape-Android) para resolver esse problema utilizando um [projeto](https://github.com/Anorov/cloudflare-scrape){: target="_blank"} do [Anorov](https://github.com/Anorov){: target="_blank"}.

<div style="width:100%;height:0;padding-bottom:55%;position:relative;"><iframe src="https://giphy.com/embed/l0HlFZ3c4NENSLQRi" style="position:absolute" class="giphy-embed" allowfullscreen="" width="100%" height="100%" frameborder="0"></iframe></div>

[via GIPHY](https://giphy.com/gifs/snl-saturday-night-live-snl-2016-l0HlFZ3c4NENSLQRi)

Massssss, n&atilde;i satisfeito com isso, quis ajudar ainda mais, ent&atilde;o fiz uma biblioteca pra galero \\&otilde;/ Ent&atilde;o sem mais enrola&ccedil;&otilde;es, como usar? como funfa? Bom.. primeiro voc&ecirc; ir&aacute; no meu reposit&oacute;rio do GitHub [aqui](https://github.com/Kelvao/CloudflareScrape){: target="_blank"}.

Adicione o Jitpack no seu Gradle do projeto:

<script src="https://gist.github.com/Kelvao/cb797f53e4069e369a6a54cbbda75108.js"></script>

<link rel="stylesheet" href="https://assets-cdn.github.com/assets/gist-embed-87673c31a5b37b5e6556b63e1081ebbc.css" />

<div id="gist90554794" class="gist"><div class="gist-file"><div class="gist-data"><div class="js-gist-file-update-container js-task-list-container file-box"><div id="file-build-gradle" class="file"><div itemprop="text" class="blob-wrapper data type-gradle"><table class="highlight tab-size js-file-line-container" data-tab-size="8"><tbody><tr><td id="file-build-gradle-L1" class="blob-num js-line-number" data-line-number="1">&nbsp;</td><td id="file-build-gradle-LC1" class="blob-code blob-code-inner js-file-line"><span class="pl-k">..</span>.</td></tr><tr><td id="file-build-gradle-L2" class="blob-num js-line-number" data-line-number="2">&nbsp;</td><td id="file-build-gradle-LC2" class="blob-code blob-code-inner js-file-line"><span class="pl-en">allprojects</span> {</td></tr><tr><td id="file-build-gradle-L3" class="blob-num js-line-number" data-line-number="3">&nbsp;</td><td id="file-build-gradle-LC3" class="blob-code blob-code-inner js-file-line">repositories {</td></tr><tr><td id="file-build-gradle-L4" class="blob-num js-line-number" data-line-number="4">&nbsp;</td><td id="file-build-gradle-LC4" class="blob-code blob-code-inner js-file-line">google()</td></tr><tr><td id="file-build-gradle-L5" class="blob-num js-line-number" data-line-number="5">&nbsp;</td><td id="file-build-gradle-LC5" class="blob-code blob-code-inner js-file-line">jcenter()</td></tr><tr><td id="file-build-gradle-L6" class="blob-num js-line-number" data-line-number="6">&nbsp;</td><td id="file-build-gradle-LC6" class="blob-code blob-code-inner js-file-line">maven { url <span class="pl-s"><span class="pl-pds">'</span>https://jitpack.io<span class="pl-pds">'</span></span> }</td></tr><tr><td id="file-build-gradle-L7" class="blob-num js-line-number" data-line-number="7">&nbsp;</td><td id="file-build-gradle-LC7" class="blob-code blob-code-inner js-file-line">}</td></tr><tr><td id="file-build-gradle-L8" class="blob-num js-line-number" data-line-number="8">&nbsp;</td><td id="file-build-gradle-LC8" class="blob-code blob-code-inner js-file-line">}</td></tr><tr><td id="file-build-gradle-L9" class="blob-num js-line-number" data-line-number="9">&nbsp;</td><td id="file-build-gradle-LC9" class="blob-code blob-code-inner js-file-line"><span class="pl-k">..</span>.</td></tr></tbody></table></div></div></div></div><div class="gist-meta"><a style="float:right" href="https://gist.github.com/Kelvao/cb797f53e4069e369a6a54cbbda75108/raw/ba8251b29356c8f1148d683f6ab3802e736d4e53/build.gradle">view raw</a> <a href="https://gist.github.com/Kelvao/cb797f53e4069e369a6a54cbbda75108#file-build-gradle">build.gradle</a> hosted with ❤ by <a href="https://github.com">GitHub</a></div></div></div>

Agora adicione a biblioteca no seu Gradle do app:

<script src="https://gist.github.com/Kelvao/1261b490a30fae753a26be1371facecd.js"></script>

&nbsp;