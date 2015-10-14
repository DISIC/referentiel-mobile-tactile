# Guide d'application du RGAA&nbsp;3 en contexte mobile/tactile pour du contenu web

## Introduction

### Avertissement
Cette ressource doit être utilisée en complément du [RGAA 3](http://references.modernisation.gouv.fr/rgaa-3-0), notamment son [référentiel technique](http://references.modernisation.gouv.fr/referentiel-technique-0), sans lequel la prise en compte de l'accessibilité ne peut pas être mesurée.

### À propos de cette ressource

Les plateformes mobiles/tactiles (téléphones ou tablettes) peuvent nécessiter un certain nombre d'adaptations spécifiques aux problématiques rencontrées par les utilisateurs en situation de handicap notamment.

Ce document présente, sous la forme d'une liste de critères, les adaptations applicables aux contenus web dans le contexte d'une consultation via un périphérique mobile/tactile.

Ces recommandations s'ajoutent aux critères applicables du RGAA&nbsp;3 qu'elles complètent ou corrigent, le cas échéant.

Elles tiennent compte de l'étude attentive de l'état de l'art. Néanmoins les plateformes mobiles/tactiles évoluant très rapidement, ces recommandations n'ont pas de caractère normatif.

Il appartient à chaque organisation de juger de l'opportunité de les appliquer, en fonction du contexte de consultation spécifique à chaque site ou application web concerné.

Dans le cas d'exigences contraignantes ou de l'existence d'une politique d'accessibilité prenant en compte les plateformes mobiles/tactiles, les plateformes visées devraient être ajoutées à la base de référence utilisée lors des tests et faire partie, à titre informatif, de la déclaration de conformité.

## Contenus applicables

Les plateformes mobiles/tactiles peuvent proposer trois types génériques de contenu à l'utilisateur&nbsp;:

- des contenus faisant appel exclusivement à des technologies web comme HTML et JavaScript&nbsp;;
- des contenus faisant appel exclusivement à des technologies non-web, c'est-à-dire des langages de développement spécifiques comme objective-C ou Java par exemple&nbsp;;
- Des contenus hybrides qui peuvent mélanger des contenus fournis via des technologies web et des contenus fournis via des technologies non-web. C'est le cas par exemple des <i lang="en">"webviews"</i>, composants embarqués dans une application non-web permettant d'afficher et d'interagir avec du contenu web.

**La [liste des critères](./refentiel-mobile-liste-criteres.md) présentée ici concerne exclusivement les contenus consultables à travers un navigateur web, il exclut donc les applications natives**.

Des guides méthodologiques adaptés aux applications non-web seront mis à disposition dans les [ressources fournies en application du RGAA&nbsp;3](http://references.modernisation.gouv.fr/ressources).

## WCAG, l'état de l'art et le mobile/tactile

WCAG ne propose pas de critères ou de techniques spécifiques aux situations de consultation sur les plateformes mobiles/tactiles. C'est la raison pour laquelle le RGAA&nbsp;3, qui est une méthode d'application des WCAG, ne prend pas en charge de manière spécifique cette problématique.

En février 2015, un groupe de travail a publié la première ébauche d'une note (<a href="http://www.w3.org/TR/mobile-accessibility-mapping/" lang="en">Mobile Accessibility&nbsp;: How WCAG 2.0 and Other W3C/WAI Guidelines Apply to Mobile</a>) qui se propose de préciser l'application des WCAG, ou d'autres recommandations issues de WAI, au contexte des plateformes mobiles/tactiles.

Par ailleurs, WCAG propose également une sélection de techniques applicables en contexte mobile/tactile (<a href="http://www.w3.org/WAI/GL/mobile-a11y-tf/MobileTechniques/" lang="en">WCAG 2.0 Techniques that Apply to Mobile</a>).

Néanmoins, les plateformes mobiles/tactiles, indépendamment de leur niveau de prise en charge des problématiques d'accessibilité, constituent un parc encore trop hétérogène et soumis à des évolutions ou des régressions importantes.

Leur prise en charge, et plus encore l'objectif de conformité réglementaire, apparaît comme une exigence déraisonnable, conséquence des difficultés encore trop importantes de constituer un bloc de contrôle pérenne et efficace.

En revanche, cette problématique a fortement mobilisé des acteurs importants de l'industrie ou du domaine de l'accessibilité numérique qui ont proposé un certain nombre de ressources, tutoriaux ou liste de recommandations applicables en contexte mobile/tactile.

La note produite par W3C/WAI et les éléments issus de l'état de l'art ont servi de socle à l'élaboration de la [liste des critères applicables aux plateformes mobiles/tactiles](./refentiel-mobile-liste-criteres.md) présentée dans ce document.

Il serait déraisonnable d'en faire une exigence réglementaire, cependant il est fortement recommandé de pouvoir appliquer ces recommandations dans le cas d'applications web ou de déclinaisons de sites web dédiés à la consultation sur plateforme mobile/tactile.

## Les plateformes mobiles/tactiles

Le paysage des plateformes mobiles/tactiles est constitué de deux types de périphériques différents&nbsp;: les téléphones proprement dits et les tablettes, auquel s'ajoute un type de téléphone hybride à large écran, qui propose certaines fonctionnalités propres aux tablettes.

Du point de vue de l'accessibilité web, même si des variations peuvent exister, il s'agit d'un même contexte technique que ce soit sur téléphone ou sur tablette. Les contenus sont consultés de la même manière au travers des mêmes systèmes d'exploitation. La différence se situe au niveau des équipements ou périphériques d'interaction, particulièrement pour la saisie.

Par exemple une tablette pourra accueillir un clavier physique, un téléphone hybride à large écran pourra faire appel à un stylet alors que sur un téléphone la méthode d'interaction repose quasi exclusivement sur une interface tactile.

Bien que ces différents modes d'interaction puissent faire varier considérablement la consultation, les recommandations ne font pas de différence entre ces différents types de périphérique, particulièrement dans le cas de périphériques hybrides comme les tablettes sur lesquelles le recours à un clavier physique ne modifie pas, fondamentalement, les besoins d'adaptation liées à l'utilisation d'une surface tactile, par exemple.

### L'accessibilité sur un ordinateur de bureau <i>versus</i> l'accessibilité sur une plateforme mobile/tactile

Il n'y a aucune différence, du point de vue des technologies employées, entre la prise en charge de l'accessibilité sur un ordinateur de bureau et sur une plateforme mobile/tactile.

Ces deux contextes font appel aux mêmes éléments, qui sont gérés de la même manière, pour le contenu web au moins.

Dans les deux cas, l'accessibilité dépend d'un système d'exploitation, d'une ou plusieurs APIs d'accessibilité, d'un navigateur, associé ou non à une technologie d'assistance.

Cela explique pourquoi il est apparu inutile de produire un référentiel, considéré comme une méthode d'application des WCAG, spécifique aux plateformes mobiles/tactiles.

Cela signifie, concrètement, que **tous les critères du RGAA&nbsp;3 sont applicables à du contenu web consulté via une plateforme mobile/tactile**.

**Seules certaines problématiques liées à l'utilisation d'*écrans de taille réduite* et au *mode d'interaction tactile* sont applicables de manière spécifique aux plateformes mobiles/tactiles**.

Ce sont ces problématiques, en nombre limité car très spécifiques, qui sont l'objet de ce document.

## Base de référence en contexte mobile/tactile

Il n'est pas possible, actuellement, de définir une base de référence par défaut, telle que proposée par RGAA&nbsp;3 pour la consultation via un ordinateur de bureau.

Cela tient au fait que, comme expliqué précédemment, le parc installé est encore trop hétérogène et trop évolutif. Particulièrement lors des opérations de mise à jour des systèmes d'exploitation qui peuvent donner lieu à des régressions importantes, comme à des évolutions majeures.

Par ailleurs, dans une même gamme de périphériques liés à un même système d'exploitation, il peut subsister des différences importantes entre un téléphone et une tablette, ou entre deux téléphones identiques mais proposés par un fournisseur différent, du fait de la mise à disposition de fonctionnalités spécifiques, d'optimisation ou de personnalisation des interfaces.

Néanmoins, selon l'[étude Gartner de 2014](http://www.gartner.com/newsroom/id/2996817), deux systèmes d'exploitation dominent le marché, ce qui peut constituer une amorce de base de référence. Ces deux systèmes d'exploitation sont <span lang="en">i</span>OS d'Apple et Android de Google.

<span lang="en">i</span>OS d'Apple est fortement optimisé en fonction du périphérique (téléphone ou tablette) et propose un lecteur d'écran évolué (<span lang="en">Voice Over</span>) ainsi que des fonctionnalités d'adaptation comme le réglage des contrastes et des retours d'action ou des fonctionnalités d'agrandissement.

Android de Google est publié sous licence libre et est donc très utilisé par les différents fabricants qui optimisent ou personnalisent les interfaces. Android fournit également un lecteur d'écran (<span lang="en">Talkback</span>) dont la qualité n'égale pas encore <span lang="en">Voice Over</span> au moment où nous rédigeons ce guide (juillet 2015), ainsi que des fonctionnalités d'adaptation similaires aux produits d'Apple.

À noter que Google propose également un système d'exploitation (Chrome&nbsp;OS).

D'autres fournisseurs sont également présents sur le marché comme Microsoft (Windows phone et Windows 10), la fondation Mozilla (Firefox&nbsp;OS), RIM (Blackberry&nbsp;OS), Samsung (Bada)...

Mais ces plateformes représentent une part encore minoritaire en 2015.

Toujours selon l'[étude Gartner (2014)](http://www.gartner.com/newsroom/id/2996817), Android domine largement le parc installé avec 80% environ des installations. <span lang="en">i</span>OS d'Apple représente, quant à lui, 15% environ des installations. Les autres systèmes d'exploitation représentent donc à peine 5%.

Ces deux systèmes d'exploitation constituent de fait une base de référence, mais il faut la nuancer pour les utilisateurs aveugles notamment.

En effet, l'ensemble <span lang="en">i</span>OS/Safari/<span lang="en">Voice Over</span> est très présent chez les utilisateurs aveugles du fait de la forte implication d'Apple dans l'accessibilité.

L'enquête WEBAIM&nbsp;: <a href="http://webaim.org/projects/screenreadersurvey5/" lang="en">Screen Reader User Survey #5 Results (2014)</a> fait apparaître que plus de la moitié des utilisateurs de lecteurs d'écran (63&nbsp;%) utilisent la plateforme Apple. Attention cependant, ces chiffres peuvent évoluer rapidement d'une année sur l'autre.

## Licence
Ce document est la propriété du Secrétariat général à la modernisation de l'action publique français (SGMAP). Il est placé sous la [licence ouverte 1.0 ou ultérieure](http://wiki.data.gouv.fr/wiki/Licence_Ouverte_/_Open_Licence), équivalente à une licence <i lang="en">Creative Commons BY</i>. Pour indiquer la paternité, ajouter un lien vers la version originale du document disponible sur le [compte <span lang="en">Github</span> de la DISIC](https://github.com/DISIC).
