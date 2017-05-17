# RGAA&nbsp;3 application guide in mobile/tactile context for web content

## Introduction

### Warning
This resource must be used in addition to [RGAA&nbsp;3 (in French)](http://references.modernisation.gouv.fr/rgaa/), in particular its [technical reference (in French)](http://references.modernisation.gouv.fr/rgaa/criteres.html), without which accessibility can not be measured. [These documents are available in English](https://github.com/DISIC/rgaa_referentiel_en).

### About this resource

The mobile/tactile platforms (telephones or tablets) may require a certain number of adaptations specific to the problems encountered by the users, in a disability situation in particular.

This document presents, in the form of a list of criteria, the adaptations applicable to the web contents in the context of their consultation via a mobile/tactile device.

These recommendations are an addition to the applicable RGAA&nbsp;3 criteria that they supplement or correct, if applicable.

They take into account the careful study of the state of the art. Nevertheless, the mobile/tactile platforms evolving very rapidly, these recommendations are not normative in nature.

It is up to each organization to evaluate if it is appropriate to apply them, depending on the context of consultation specific to each web site or application concerned.

In the case of mandatory requirements or the existence of an accessibility policy that takes into account the mobile/tactile platforms, the targeted platforms should be added to the reference database used during the tests and be included, for information purposes, to the conformance claim.

## Applicable Contents

Mobile/tactile platforms can offer three generic types of content to the user:

- content using exclusively web technologies like HTML and JavaScript;
- contents using exclusively non-web technologies, ie specific development languages ​​like objective-C or Java for example;
- Hybrid content that can mix content provided via web technologies and content provided via non-web technologies. This is the case, for example, for "webviews", ie embedded components in a non-web application for displaying and interacting with web content.

**The [list of criteria](./mobile-touch-guidelines-criteria.md) presented here relates exclusively with contents that can be viewed through a web browser, therefore it excludes native applications**.

Methodological guides adapted to non-web applications will be made available in [companion resources provided with the RGAA&nbsp;3 (in French)](http://references.modernisation.gouv.fr/resources).

## WCAG, state of the art and mobile/tactile devices

WCAG does not propose criteria or techniques specific to  consultation on mobile/tactile platforms. This is why the RGAA&nbsp;3, which is a WCAG application method, does not specifically address this issue.

In February 2015, a working group published the first draft of a note ([Mobile Accessibility: How WCAG 2.0 and Other W3C/WAI Guidelines Apply to Mobile](http://www.w3.org/TR/mobile-accessibility-mapping/) to clarify the application of WCAG, or other recommendations from the WAI, to the context of mobile/tactile platforms.

In addition, WCAG also offers a selection of techniques applicable in mobile/tactile context ([WCAG 2.0 Techniques that Apply to Mobile](http://www.w3.org/WAI/GL/mobile-a11y-tf/MobileTechniques/)).

However, mobile/tactile platforms, regardless of their level of accessibility support, are still too heterogeneous and subject to major changes or regressions.

Their management, and even more so the objective of regulatory conformance, appears to be an unreasonable requirement, because it is still too difficult to elaborate a permanent and effective control system.

On the other hand, this issue has strongly driven key players in the industry, or in the area of ​​digital accessibility, to  propose a number of resources, tutorials or lists of recommendations, applicable in a mobile/tactile context.

The note produced by W3C/WAI and the elements from the state of the art have served as a basis for the development of the [list of criteria applicable to mobile/tactile platforms](./mobile-touch-guidelines-criteria.md) presented in this document.

It would be unreasonable to make it a regulatory requirement, however it is strongly recommended to consider applying these recommendations to web applications or versions of websites dedicated to consultation on mobile/tactile platforms.

## Mobile/tactile platforms

The landscape of the mobile/tactile platforms is made up of two different kinds of devices: smartphones and tablets, plus hybrid wide-screen phones that offer features usually found on tablets.

From a web accessibility point of view, even if variations can exist, it is the same technical context whether on a phone or on a tablet. The contents are consulted in the same way through the same operating systems. The difference is at the level of interaction devices or peripherals, especially for inputs.

For example, a tablet will be commonly used with a physical keyboard; a wide-screen hybrid phone will often be used with a stylus; while on a telephone, the method of interaction relies almost exclusively on a touch interface.

Although these different modes of interaction may vary considerably, the recommendations make no distinction between these different types of devices; particularly in the case of hybrid devices such as tablets, where the use of a physical keyboard does not alter, fundamentally, the needs for adaptations related to the use of a tactile surface, for example.

### Accessibility on a desktop, versus accessibility on a mobile/tactile platform

There is no difference, from a technological point of view, between the accessibility support on a desktop computer and a mobile/tactile platform.

These two contexts use the same elements, which are managed in the same way, for at least the web content.

In both cases, accessibility depends on an operating system, one or more accessibility APIs, a browser, with or without assistive technology.

This explains why it appeared unnecessary to produce a technical reference, considered as a WCAG application method, dedicated to mobile/tactile platforms.

This means, in practice, that **all the  RGAA&nbsp;3 criteria are applicable to web content accessed via a mobile/tactile platform**.

**Only certain issues related to the use of *small screens* and *tactile interactions* are applicable specifically to mobile/tactile platforms**.

These issues, limited in number because of their specificity, are the subject of this document.

## Mobile/Touch Baseline

Currently, it is not possible to define a default reference baseline, like the one proposed by RGAA&nbsp;3 for consultation via a desktop computer.

This is because, as explained above, the installed base is still too heterogeneous and too changing. Particularly with operating systems updates that may cause important regressions, as well as major evolutions.

Moreover, in the same range of peripherals based on the same operating system, there still may be significant differences between a telephone and a tablet, or between two identical telephones from different makers, because of specific features, or optimized or customized interfaces.

However, according to the [2014 Gartner study](http://www.gartner.com/newsroom/id/2996817), two operating systems dominate the market, which can be a starting point of reference. These two operating systems are iOS, from Apple, and Android, from Google.

Apple's iOS is highly optimized for the device (phone or tablet) and includes an advanced screen reader (VoiceOver), as well as adaptation features such as contrast adjustment, haptic feedback, and magnification features.

Google's Android is published under free license and is therefore widely used by different manufacturers, who optimize or customize the interfaces. Android also provides a screen reader (Talkback) whose quality does not yet match VoiceOver at the time of writing (July 2015), as well as adaptation features similar to the ones in Apple's products.

Note that Google also proposes an operating system (Chrome OS).

Other vendors are also present on the market, such as Microsoft (Windows Phone and Windows 10), Mozilla Foundation (Firefox OS), RIM (Blackberry OS), Samsung (Bada)&hellip;

But these platforms still represent a minority market share in 2015.

According to the [2014 Gartner study](http://www.gartner.com/newsroom/id/2996817), Android dominates the installed base with about 80%. Apple's iOS accounts for about 15% of the installations. The other operating systems therefore represent barely 5%.

These two operating systems are a <i>de facto</i> baseline, but it should be nuanced, for blind users in particular.

The iOS/Safari/VoiceOver package is very popular among  blind users due to Apple's strong commitment to accessibility.

The WEBAIM survey: <a href="http://webaim.org/projects/screenreadersurvey5/">Screen Reader User Survey #5 Results (2014)</a> shows that more than half of screen reader users (63%) use the Apple platform. Caution is required, however, since these figures can evolve rapidly from year to year.

## Licence
This document is the property of the <span lang="fr">Secrétariat général à la modernisation de l'action publique</span> (SGMAP). It is placed under [Open Licence 1.0 or later (PDF, 541 kb)](http://ddata.over-blog.com/xxxyyy/4/37/99/26/licence/Licence-Ouverte-Open-Licence-ENG.pdf), equivalent to a Creative Commons BY licence. To indicate authorship, add a link to the original version of the document available on the [DInSIC's Github account](https://github.com/DISIC).