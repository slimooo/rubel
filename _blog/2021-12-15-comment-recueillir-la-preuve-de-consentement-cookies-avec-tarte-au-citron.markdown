---
layout: post
title: "Comment recueillir la preuve de consentement cookies avec Tarte au Citron ?"
authors: Slim TOUHAMI, Charly G.
date:   2021-12-15 12:31:35 +0300
image:  "assets/images-blog/tarte-au-citron-cookies-google-analytics.webp"
tags:   [consentement CNIL]
---

À l'article 4 de ses recommandations sur les cookies et traceurs, la CNIL demande à l'éditeur d'un site de *"démontrer, à tout moment, que les utilisateurs ont donné leur consentement"*. En d'autres termes, en cas de contrôle ou de litige, il faudra apporter la preuve que l'on a bien mis en place une fenêtre cookies et que celle-ci est bien conforme aux recommandations de la CNIL.

Lorsqu'on utilise un [Consent Management Plateform](https://www.axeptio.eu/post/quels-sont-les-cookies-exemptes-de-consentement) (CMP), c'est le prestataire en tant que tiers de confiance qui peut apporter la preuve de l'existence de la collecte de consentement.

NB : lorsque vous utilisez que des [outils exemptés de consentement comme Abla Analytics](https://abla.io), et aucun autre service utilisant des traceurs, la mise en place d'un CMP devient facultative.

## La collecte de la preuve cookies avec Tarte au Citron

Avec [Tarte au Citron](https://tarteaucitron.io/fr/), c'est un peu plus complexe. En effet, il s'agit d'une solution libre et autohébergée. Par nature, il est possible de démontrer l'existence de la collecte de consentement au jour du contrôle, mais, par défaut, il n'y a aucun moyen de prouver son implémentation la semaine dernière, le mois dernier ou il y a 5 ans.

Parmi les solutions proposées par la CNIL :

<blockquote class="quote quote--article">
        <p class="m-0">
            “Les différentes versions du code informatique utilisé par l’organisme recueillant le consentement peuvent être mises sous séquestre auprès d’un tiers, ou, plus simplement, un condensat (ou « hash ») de ce code peut être publié de façon horodatée sur une plate-forme publique, pour pouvoir prouver son authenticité a posteriori”
        </p>
        <cite>
            Commission Nationale de l'Informatique et des Libertés
        </cite>
     </blockquote>


Le service gratuit [Wayback Machine](https://web.archive.org/) de l'Internet Archive peut être envisagé pour sauvegarder vos applications et être en mesure de prouver qu'elles utilisent une version correctement configurée de Tarte au citron pour recueillir le consentement.

## La configuration de Wayback Machine pour recueillir la preuve de consentement

Wayback Machine est un service proposé par la fondation Internet Archive. L'objectif de cet outil est d'archiver les contenus publiés sur le net à des fins historiques et de conservation des patrimoines numériques.

L'utilisation de cette solution a pour avantages sa gratuité et la possibilité d'apporter une preuve qualitative sur l'existence à un instant T d'un dispositif de collecte de consentement correctement configuré.

La procédure pour sauvegarder une application web est relativement simple, il suffit de :

1. Se rendre sur le site [Wayback Machine](https://web.archive.org/save/)
2. Rentrer l’URL d'une page où se trouve la fenêtre cookies dans le formulaire « SAVE PAGE NOW »
3. Cliquer sur le bouton "Save Page"
4. Conserver le lien généré par la « Wayback Machine » afin d’être en mesure de consulter la version archivée ultérieurement

<div class="article__video mb-2" data-video="true">
    <div class="fluid-width-video-wrapper" style="padding-top: 56.25%;">
        <iframe src="https://abla.io/assets/videos/webbackmachine.mp4" loading="lazy" frameborder="0" allowfullscreen></iframe>
    </div>
</div>

Pour obtenir un bon niveau de preuves que le consentement est correctement effectué par Tarte au citron sur l'ensemble de l'application, il peut également être pertinent de sauvegarder un échantillon représentatif des différentes pages des applications, en particulier, les pages qui nécessitent le recueil du consentement (les pages avec des vidéos YouTube, Dailymotion, des réseaux sociaux, etc.).

Cette approche a cependant un inconvénient majeur, elle nécessite des moyens humains significatifs pour sauvegarder les différentes pages d’une application et archiver les liens de la « Wayback Machine » pour une utilisation ultérieure.
