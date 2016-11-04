# Liste des critères RGAA&nbsp;3, spécifiques aux plateformes mobiles/tactiles

## Introduction

### Avertissement
Cette ressource doit être utilisée en complément du [RGAA 3](http://references.modernisation.gouv.fr/rgaa/), notamment son [référentiel technique](http://references.modernisation.gouv.fr/rgaa/criteres.html), sans lequel la prise en compte de l'accessibilité ne peut pas être mesurée.

### Mode d'emploi

Cette liste reprend les formulations du RGAA&nbsp;3, elle a été élaborée en respectant les mêmes règles d'écriture et propose le même fonctionnement de validation par l'utilisation des 5 statuts du RGAA&nbsp;3&nbsp;:

1. conforme&nbsp;;
2. non-conforme&nbsp;;
3. non-applicable&nbsp;;
4. non-testé&nbsp;;
5. dérogé.

La liste des critères spécifiques aux plateformes mobiles/tactiles est pensée comme une extension du RGAA&nbsp;3, indépendante du reste du référentiel technique et non obligatoire.

Nous numéroterons les critères de cette thématique en commençant par 14 pour maintenir la cohérence avec le RGAA&nbsp;3.

## Liste des critères

### Thématique 14 - Mobile/tactile

Principes&nbsp;: Perceptible, Utilisable, Compréhensible, Robuste.

#### Recommandation
S'assurer que les <a href="#Zonesens">zones sensibles</a> ont une taille suffisante, que le zoom n'est pas interdit, simplifier les <a href="#intergest">interactions gestuelles</a> ou leur donner une alternative, s'assurer que le contenu reste lisible quelle que soit l'orientation de l'écran, grouper les <a href="#Elemadj">éléments interactifs adjacents</a> ayant la même fonction et optimiser la saisie via des <a href="#Typesaisie">types de saisie</a> pertinents.

#### 14.1 Chaque <a href="#Zonesens">zone sensible</a> a-t-elle une <a href="Taillsuf">taille suffisante&nbsp;</a>?

* Test 14.1.1&nbsp;: Chaque <a href="#Zonesens">zone sensible</a> respecte-elle ces conditions&nbsp;?
    * la largeur de la <a href="#Zonesens">zone sensible</a> fait 9 mm au moins&nbsp;;
    * la hauteur de la <a href="#Zonesens">zone sensible</a> fait 9 mm au moins&nbsp;;
    * la <a href="#Zonesens">zone sensible</a> a une <a href="#Margesuf">marge extérieure suffisante</a>.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#touch-target-size-and-spacing" lang="en">3.2 Touch Target Size and Spacing</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.2 [AA] La fonctionnalité de zoom du navigateur ne doit pas être supprimée ou limitée, cette règle est-elle respectée&nbsp;?

* Test 14.2.1&nbsp;: les valeurs utilisées par la métadonnée <code lang="en">viewport</code>, respectent-elles ces conditions&nbsp;?
    * la valeur de l'attribut <code lang="en">maximum-scale</code> est égale à 2.0 ou à 200&nbsp;%, au moins&nbsp;;
    * la valeur de l'attribut <code lang="en">user-scale</code> est égale à <code lang="en">yes</code>, si elle est présente.

* Test 14.2.2&nbsp;: les valeurs utilisées par la règle CSS <code lang="en">@viewport</code>, respectent-elles ces conditions&nbsp;?
    * la valeur de la propriété <code lang="en">max-zoom</code> est supérieure ou égale à 2.0 ou à 200&nbsp;%, au moins&nbsp;;
    * la valeur de la propriété <code lang="en">user-zoom</code> est égale à <code lang="en">zoom</code>, si elle est présente.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#zoom-magnification" lang="en">2.2 Zoom/Magnification</a> ;
- Critère de succès WCAG 2.0&nbsp;: <a href="http://www.w3.org/Translations/WCAG20-fr/#visual-audio-contrast-scale" title="critère de succès 1.4.1 des WCAG 2">1.4.4</a>.

#### 14.3 Pour chaque <a href="#Intergest">interaction gestuelle</a> déclenchant une action, l'action est-elle déclenchée de manière appropriée&nbsp;?

* Test 14.3.1&nbsp;: Chaque interaction  gestuelle déclenchant une action respecte-t-elle ces conditions&nbsp;?
    * l'action est déclenchée uniquement à la fin de l'interaction gestuelle&nbsp;;
    * l'action n'est pas déclenchée si l'élément déclencheur perd le focus.

Consulter la proposition de technique <a href="http://w3c.github.io/Mobile-A11y-TF-Note/Techniques/M003.html" lang="en">Activating elements via the mouseup or touchend event</a>.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#touchscreen-gestures" lang="en">3.3 Touchscreen Gestures</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.4 Chaque <a href="#Intergestcomplexe">interaction gestuelle complexe</a> a-t-elle une alternative&nbsp;?

* Test 14.4.1&nbsp;: chaque interaction gestuelle complexe respecte-t-elle une de ces conditions&nbsp;?
    * l'interaction gestuelle possède une alternative non-gestuelle&nbsp;;
    * un paramètre permet à l'utilisateur d'utiliser des <a href="#intergest">interactions gestuelles</a> simplifiées.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#touchscreen-gestures" lang="en">3.3 Touchscreen Gestures</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.5 [AAA] Les <a href="#intergest">interactions gestuelles</a> doivent être décrites au moyen d'une aide en ligne, cette règle est-elle respectée&nbsp;?

* Test 14.5.1&nbsp;: Les <a href="#intergest">interactions gestuelles</a> respectent-elles une de ces conditions&nbsp;?
    * l'interaction gestuelle est décrite avant son déclenchement&nbsp;;
    * l'interaction gestuelle est décrite via une aide en ligne.

##### Correspondances

- <span lang="en">W3C Mobile Accessibility</span>&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#provide-instructions-for-custom-touchscreen-and-device-manipulation-gestures" lang="en">4.6 Provide instructions for custom touchscreen and device manipulation gestures</a>&nbsp;;
- Critère de succès WCAG 2.0&nbsp;: <a href="http://www.w3.org/Translations/WCAG20-fr/#minimize-error-context-help" title="critère de succès 3.3.5 des WCAG 2">3.3.5</a>.

#### 14.6 Les <a href="#Intergest">interactions gestuelles</a> impliquant un changement d'orientation de l'écran (basculement, rotation, secouement...) ont-elles une alternative (<a href="#CP1">hors cas particulier</a>)&nbsp;?

* Test 14.6.1&nbsp;: Les <a href="#intergest">interactions gestuelles</a> impliquant un changement d'orientation de l'écran (basculement, rotation, secouement...) respectent-elles ces conditions&nbsp;?
    * une action gestuelle alternative utilise le tap (<i lang="en">touch</i> en anglais)&nbsp;;
    * une action alternative au clavier permettant d'accéder aux mêmes contenus et fonctionnalités est présente.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;:
    * <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#changing-screen-orientation-portrait-landscape" lang="en">4.1 Changing Screen Orientation (Portrait/Landscape)</a>&nbsp;;
    * <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#device-manipulation-gestures" lang="en">3.4 Device Manipulation Gestures</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.7 L'accès au contenu ne doit pas dépendre d'une orientation de l'écran (portrait ou paysage), cette règle est-elle respectée&nbsp;?

* Test 14.7.1&nbsp;: L'accès au contenu respecte-t-il une de ces conditions&nbsp;?
    * un paramètre permettant à l'utilisateur de choisir l'orientation de l'affichage du contenu, portrait ou paysage, est présent&nbsp;;
    * le contenu est consultable dans les deux orientations, portrait et paysage.

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#changing-screen-orientation-portrait-landscape" lang="en">4.1 Changing Screen Orientation (Portrait/Landscape)</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.8 Pour chaque champ de saisie, le format de saisie attendu est-il, si possible, associé à un <a href="#Typesaisie">type de saisie</a> pertinent&nbsp;?

* Test 14.8.1&nbsp;: Pour chaque champ de saisie, le format de saisie attendu est-il associé à un type de saisie pertinent&nbsp;?

<p>Consulter la <a href="#NT1">note technique au sujet des nouveaux types de formulaire</a>.</p>

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#set-the-virtual-keyboard-to-the-type-of-data-entry-required" lang="en">5.1 Set the virtual keyboard to the type of data entry required</a>.

###### Correspondance de niveau
<p>La [note W3C/WAI (en anglais)](http://www.w3.org/TR/mobile-accessibility-mapping/) sur laquelle s'appuie ce référentiel n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

#### 14.9 [A] Les <a href="#Elemadj">éléments interactifs adjacents</a>, déclenchant la même action, doivent être groupés en un seul élément, cette règle est-elle respectée&nbsp;?

* Test 14.9.1&nbsp;: Les <a href="#Elemadj">éléments interactifs adjacents</a>, déclenchant la même action, doivent être groupés en un seul élément, cette règle est-elle respectée&nbsp;?

Consulter la technique <a href="http://www.w3.org/WAI/GL/WCAG20-TECHS/H2.html" lang="en"> H2&nbsp;: Combining adjacent image and text links for the same resource</a>.

<p>Note&nbsp;: cette recommandation référence une technique WCAG, actuellement non prise en charge dans le référentiel technique du RGAA&nbsp;3. Cette exigence devrait être introduite dans RGAA&nbsp;3 à la prochaine mise à jour. Ce critère 14.9 sera alors supprimé pour éviter les doublons.</p>

##### Correspondances
- <span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#grouping-operable-elements-that-perform-the-same-action" lang="en">4.4 Grouping operable elements that perform the same action</a>.
- Critères de succès WCAG 2.0&nbsp;:
    * <a href="http://www.w3.org/Translations/WCAG20-fr/#navigation-mechanisms-refs" title="critère de succès 2.4.4 des WCAG 2">2.4.4</a>&nbsp;;
    * <a href="http://www.w3.org/Translations/WCAG20-fr/#navigation-mechanisms-link" title="critère de succès 2.4.9 des WCAG 2">2.4.9</a>.

## Recommandations complémentaires

Ces recommandations devraient également, dans la mesure du possible, être prises en compte pour optimiser l'expérience des utilisateurs en situation de handicap, notamment.

Il est à noter néanmoins que certaines d'entre elles peuvent poser des problèmes ou être complexes à respecter pour un contenu commun aux deux plateformes (ordinateur de bureau et plateformes mobiles/tactiles).

Dans ce cadre, nous avons mis en place une numérotation dédiée à ces critéres et les avons préfixé par le mot clé "RecoMT-".

### RecoMT-14.1 Chaque image porteuse d'information utilisée en propriété de fond d'élément a-t-elle une alternative visible&nbsp;?

* Test RecoMT-14.1.1&nbsp;: Chaque image porteuse d'information utilisée en propriété de fond d'élément via CSS, respecte-t-elle une de ces conditions&nbsp;?
    * l'image est accompagnée d'un texte visible&nbsp;;
    * un mécanisme permet de remplacer l'image par un texte visible.

#### Référence
- <span lang="en">BBC Mobile Accessibility Guidelines</span>&nbsp;&nbsp;: <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/images/background-images" lang="en">Background images</a>.

<p>La référence sur laquelle s'appuie cette recommandation n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

### RecoMT-14.2 Chaque alternative visible associée à une image en propriété de fond est-elle pertinente.&nbsp;?

* Test RecoMT-14.2.1&nbsp;&nbsp;: Chaque alternative visible associée à une image en propriété de fond est-elle pertinente&nbsp;?

#### Référence
- <span lang="en">BBC Mobile Accessibility Guidelines</span>&nbsp;&nbsp;: <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/images/background-images" lang="en">Background images</a>.

<p>La référence sur laquelle s'appuie cette recommandation n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau A**.</p>

### RecoMT-14.3 Chaque image est-elle optimisée pour la taille et la résolution de l'écran&nbsp;?

* Test RecoMT-14.3.1&nbsp;: Chaque image respecte-t-elle une de ces conditions&nbsp;?
    * l'image est optimisée pour la taille et la résolution de l'écran&nbsp;;
    * un mécanisme permet de remplacer l'image par une image optimisée pour la taille et la résolution de l'écran.

#### Référence
- <span lang="en"> W3C Mobile Web Best Practices 1.0</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-bp/#d0e1219" lang="en">5.3.5 Graphics</a>.

<p>La référence sur laquelle s'appuie cette recommandation n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau AA**.</p>

### RecoMT-14.4 L'ordre des contenus de la page est-il optimisé pour une consultation sur un écran de périphérique mobile/tactile&nbsp;?

* Test RecoMT-14.4.1&nbsp;: Les contenus les plus importants de la page sont-ils présentés en premier sans nécessiter de balayage&nbsp;?

#### Référence
- <span lang="en"><span lang="en">W3C Mobile Accessibility</span>&nbsp;&nbsp;: <a href="http://www.w3.org/TR/mobile-accessibility-mapping/#positioning-important-page-elements-before-the-page-scroll" lang="en">4.3 Positioning important page elements before the page scroll</a>.

<p>La référence sur laquelle s'appuie cette recommandation n'associe pas de niveau à ce critère. À titre indicatif, selon la note "<a href="http://www.w3.org/Translations/NOTE-UNDERSTANDING-WCAG20-fr/conformance.html#uc-levels-head">Comprendre les niveaux de conformité</a>", nous estimons qu'il s'agit d'un **critère de niveau AA**.</p>

## Glossaire

### <a name="Elemadj"></a>Éléments interactifs adjacents
Tous les éléments interactifs tels que des liens, des boutons etc., qui sont adjacents et qui réalisent une même action ou affichent une même ressource.

### <a name="intergest"></a>Interaction gestuelle
Toute interaction effectuée au moyen de gestes déclenchant une action, notamment via une surface tactile. Par exemple, les interactions de type tap (touché rapide équivalent d'un clic à la souris), touché (<span lang="en">touch</span> en anglais, touché plus long qu'un tap), balayage (<span lang="en">swipe</span>) ou pincement (<span lang="en">pinch</span>) sont des interactions gestuelles.

### <a name="Intergestcomplexe"></a>Interaction gestuelle complexe
Les interactions gestuelles complexes impliquent plusieurs mouvements successifs ou synchronisés. Par exemple, un balayage suivi de plusieurs taps.
Ces interactions peuvent présenter des difficultés insurmontables pour certains utilisateurs.

Note : Le terme "synchronisé" comprend à la fois les gestes simultanés et les gestes enchaînés sans pause.

### <a name="Margesuf"></a> Marge extérieure suffisante

Lorsque des contrôles, comme des boutons ou des textes activables, sont adjacents, il peut être difficile pour un utilisateur de les activer individuellement si leur taille n'est pas suffisante, notamment lorsque cette taille est proche du minimum requis (9mm X 9mm).

L'implémentation d'une marge permet de diminuer les erreurs d'activation d'éléments adjacents. Il n'y a pas de valeur fixe à cette marge car elle peut dépendre de la résolution et de la taille physique de l'écran.

Elle doit être suffisante néanmoins pour permettre, quelles que soient la résolution et la taille physique de l'écran, d'activer sans erreur chaque composant interactif.

À titre indicatif, voici quelques références de recommandation de marge :

* Les [BBC mobile accessibility guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/spacing) recommandent une marge de 1 pixel, au moins.

* [Google](https://www.google.com/design/spec/usability/accessibility.html#) recommande une marge de 8dp

* D'autres références peuvent être consultées sur le [blog de Luke Wroblewski](http://www.lukew.com/ff/entry.asp?1085).


### <a name="Taillsuf"></a>Taille suffisante
Les éléments interactifs comme les boutons et les zones de texte activables peuvent être difficiles à manipuler s'ils ont une taille insuffisante sur des écrans de périphériques de petite taille, ou en haute résolution.

La taille de ces zones n'est pas définie en pixel mais en millimètre afin de tenir compte des tailles physiques réelles des périphériques d'affichage et de la densité en pixels qu'ils utilisent.

Il appartient aux développeurs de s'assurer, quelle que soit la taille en pixels utilisée, que les composants interactifs ont une taille restituée de 9mm x 9mm au moins pour être utilisés sur les écrans en haute résolution notamment.

### <a name="Typesaisie"></a>Type de saisie
HTML5 propose des types de saisie spécifiques qui, lorsque le périphérique le supporte, permettent d'optimiser la saisie. Par exemple, le type <code>"tel"</code> provoquera l'apparition du clavier numérique.

Les types de saisie sont&nbsp;&nbsp;:

- <code>text</code>&nbsp;;
- <code>search</code>&nbsp;;
- <code>tel</code>&nbsp;;
- <code>url</code>&nbsp;;
- <code>email</code>&nbsp;;
- <code>password</code>&nbsp;;
- <code>date</code>&nbsp;;
- <code>time</code>&nbsp;;
- <code>number</code>&nbsp;;
- <code>range</code>&nbsp;;
- <code>color</code>&nbsp;;
- <code>checkbox</code>&nbsp;;
- <code>radio</code>&nbsp;;
- <code>file</code>.

### <a name="Zonesens"></a>Zone sensible
Zone interactive de l'écran associée à une interaction gestuelle. Les zones sensibles recouvrent les boutons, les liens, les contrôles de formulaire ou tout autre élément interactif ou rendu interactif via JavaScript notamment.

## Cas particuliers

### <a name="CP1"></a>Critère 14.6
Il existe une gestion de cas particuliers lorsque la rotation, le basculement ou le secouement est inhérent à la fonctionnalité proposée et ne trouverait pas d'équivalent dans un autre mode d'interaction.

Dans ce cas, le critère est non-applicable.

## Notes techniques

### <a name="NT1"></a>Note au sujet des nouveaux types de formulaire
Pour que l'accessibilité "fonctionne", les différents éléments HTML notamment doivent avoir été intégrés sur les différentes plateformes. Or, il peut exister des différences de support importantes entre la prise en charge des nouveaux types de formulaire sur les ordinateurs de bureau et les plateformes mobiles/tactiles.

Pour certains types, par exemple le type <code>"date"</code> ou <code>"heure"</code>, il n'est pas possible actuellement de les utiliser de manière homogène. Cela nécessite généralement le recours à l'utilisation de composants développés via JavaScript et WAI-ARIA.

Dans d'autres cas, par exemple le type <code lang="en">"number"</code>, la dégradation dans les navigateurs de bureau ne le supportant pas est acceptable, ce qui permet de les utiliser dans un contexte mobile/tactile.

Il appartient aux auteurs de contenus et à l'auditeur de déterminer, au cas par cas, l'applicabilité du critère.

Dans le cas où un type de formulaire ne pourrait pas être utilisé en contexte mobile/tactile, du fait de son manque de support sur un navigateur de bureau notamment, il est acceptable de considérer le critère comme non-applicable.

## Ressources et références

* <a href="http://www.w3.org/TR/mobile-accessibility-mapping/" lang="en">Mobile Accessibility&nbsp;: How WCAG 2.0 and Other W3C/WAI Guidelines Apply to Mobile</a>
* <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile" lang="en">BBC Standards and Guidelines for Mobile Accessibility</a>
* <a href="http://www.w3.org/TR/mobile-bp/" lang="en">Mobile Web Best Practices 1.0</a>
* <a href="http://www.w3.org/TR/mwbp-wcag/" lang="en">Relationship between Mobile Web Best Practices (MWBP) and Web Content Accessibility Guidelines (WCAG)</a>
* <a href="http://www.w3.org/WAI/mobile/experiences" lang="en">Barriers Common to Mobile Device Users and People with Disabilities</a>
* <a href="http://www.w3.org/TR/mobileOK-basic10-tests/" lang="en">W3C mobileOK Basic Tests 1.0</a>
* <a href="http://www.funka.com/en/our-assignments/research-projects/archive---research-projects/mobile-navigation-guidelines/">Funka Mobile Navigation Guidelines</a>
* <a href="https://checklists.opquast.com/web-mobile/">Opquast Web Mobile</a>
* <a href="https://developer.mozilla.org/en-US/docs/Web/Accessibility/Mobile_accessibility_checklist" lang="en">Mobile accessibility checklist</a>.

## Licence
Ce document est la propriété du Secrétariat général à la modernisation de l'action publique français (SGMAP). Il est placé sous la [licence ouverte 1.0 ou ultérieure](https://www.etalab.gouv.fr/licence-ouverte-open-licence), équivalente à une licence <i lang="en">Creative Commons BY</i>. Pour indiquer la paternité, ajouter un lien vers la version originale du document disponible sur le [compte <span lang="en">Github</span> de la DInSIC](https://github.com/DISIC).
