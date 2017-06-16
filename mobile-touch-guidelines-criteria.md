# List of criteria RGAA&nbsp;3, specific to mobile/tactile platforms

## Introduction

### Warning
This resource must be used in addition to [RGAA 3 (in French)](http://references.modernisation.gouv.fr/rgaa/), in particular its [technical reference (in French)](http://references.modernisation.gouv.fr/rgaa/criteres.html), without which accessibility can not be measured. [These documents are available in English](https://github.com/DISIC/rgaa_referentiel_en).

### Instructions

This list uses the same formalism as the RGAA&nbsp;3. It was elaborated according to the same rules of writing and proposes the same validation system based on the 5 statuses of the RGAA&nbsp;3:

1. Conforming;
2. Non-conforming;
3. Not applicable;
4. Not tested;
5. Derogated.

The list of criteria specific to mobile/tactile platforms is designed as an extension of the RGAA&nbsp;3, independent of the rest of the technical reference, and not mandatory.

Criteria for this category are numbered starting with 14, in order to maintain consistency with the RGAA&nbsp;3.

## List of criteria

### Category 14 - Mobile/Tactile

Principles: Perceivable, Operable, Understandable, Robust.

#### Recommendation
Make sure that <a href="#Zonesens">touch targets</a> are large enough, that zooming is possible, simplify <a href="#intergest">gesture-based interactions</a> or provide an alternative, make sure that the content remains legible independently of the orientation of the screen, group <a href="#Elemadj">adjacent interactive elements</a> with the same function and optimize input via relevant <a href="#Typesaisie">input types</a>.

#### 14.1 Does each <a href="#Zonesens">touch target</a> have a <a href="Taillsuf">sufficient size</a>?

* Test 14.1.1: Does each <a href="#Zonesens">touch target</a> meet these requirements?
    * The width of the <a href="#Zonesens">touch target</a> is at least 9 mm;
    * The height of the <a href="#Zonesens">touch target</a> is at least 9 mm;
    * The <a href="#Zonesens">touch target</a> has a <a href="#Margesuf">sufficient external margin</a>.

##### Mappings
- W3C Mobile Accessibility: [3.2 Touch Target Size and Spacing](http://www.w3.org/TR/mobile-accessibility-mapping/#touch-target-size-and-spacing).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it's a **level A criterion**. </p>

#### 14.2 [AA] Browser zoom functionality should not be suppressed or limited, has this rule been followed?

* Test 14.2.1: Do the values ​​used by the metadata <code>viewport</code> meet these conditions?
    * The value of the <code>maximum-scale</code> attribute is greater than or equal to 2.0 or 200%;
    * The value of the <code>user-scale</code> attribute is equal to <code>yes</code>, if present.

* Test 14.2.2: Do the values ​​used by the CSS <code>@viewport</code> rule meet these conditions?
    * The value of the <code>max-zoom</code> property is greater than or equal to 2.0 or 200%;
    * The value of the <code>user-zoom</code> property is equal to <code>zoom</code>, if present.

##### Mappings
- W3C Mobile Accessibility: [2.2 Zoom/Magnification](http://www.w3.org/TR/mobile-accessibility-mapping/#zoom-magnification);
- [WCAG 2.0 Success Criterion: 1.4.4](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-scale.html).

#### 14.3 For each <a href="#Intergest">gesture-based interaction</a> triggering an action, is the action triggered appropriately?

* Test 14.3.1: Does each gesture-based interaction triggering an action meet these conditions?
    * The action is triggered only at the end of the gesture-based interaction;
    * The action is not triggered if the triggering element loses focus.

Read the proposed technique <a href="http://w3c.github.io/Mobile-A11y-TF-Note/Techniques/M003.html">Activating elements via the <code>mouseup</code> or <code>touchend</code> event</a>.

##### Mappings
- W3C Mobile Accessibility: [3.3 Touchscreen Gestures](http://www.w3.org/TR/mobile-accessibility-mapping/#touchscreen-gestures).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it's a **level A criterion**.</p>

#### 14.4 Does each <a href="#Intergestcomplex">complex gesture-based interaction</a> have an alternative?

* Test 14.4.1: Does each complex gesture-based interaction meet one of these conditions?
    * The gesture-based interaction has a non-gesture based alternative;
    * A setting allows the user to use simplified <a href="#Intergest">gesture-based interactions</a>.

##### Mappings
- W3C Mobile Accessibility: [3.3 Touchscreen Gestures](http://www.w3.org/TR/mobile-accessibility-mapping/#touchscreen-gestures).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

#### 14.5 [AAA] <a href="#intergest">Gesture-based interactions</a> should be described using online help, has this rule been followed?

* Test 14.5.1: Do <a href="#intergest">gesture-based interactions</a> meet one of these conditions?
    * Each gesture-based interaction is described prior to triggering;
    * Each gesture-based interaction is described via online help.

##### Mappings

- W3C Mobile Accessibility: [4.6 Provide instructions for custom touchscreen and device manipulation gestures](http://www.w3.org/TR/mobile-accessibility-mapping/#provide-instructions-for-custom-touchscreen-and-device-manipulation-gestures);
- [WCAG 2.0 Success Criteria: 3.3.5](https://www.w3.org/TR/WCAG20/#minimize-error-context-help).

#### 14.6 Do <a href="#Intergest">gesture-based interactions</a> involving a change in screen orientation (tilting, rotation, shaking...) have an alternative (<a href = "#CP1">except in particular cases</a>)?

* Test 14.6.1: Do <a href="#intergest">gesture-based interactions</a> involving a change in screen orientation (tilting, rotation, shaking...) meet these conditions?
    * A touch-based alternative interaction is available;
    * A keyboard operable alternative provides access to the same contents and features.

##### Mappings
- W3C Mobile Accessibility:
    * [4.1 Changing Screen Orientation (Portrait/Landscape)](http://www.w3.org/TR/mobile-accessibility-mapping/#changing-screen-orientation-portrait-landscape);
    * [3.4 Device Manipulation Gestures](http://www.w3.org/TR/mobile-accessibility-mapping/#device-manipulation-gestures).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

#### 14.7 Access to content should not depend on a screen orientation (portrait or landscape), has this rule been followed?

* Test 14.7.1: Does access to content meet one of these conditions?
    * A setting allowing the user to choose the orientation of the display of content, portrait or landscape, is available;
    * The content is available in both orientations, portrait and landscape.

##### Mappings
- W3C Mobile Accessibility: [4.1 Changing Screen Orientation (Portrait/Landscape)](http://www.w3.org/TR/mobile-accessibility-mapping/#changing-screen-orientation-portrait-landscape).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

#### 14.8 For each input field, is the expected input format, if possible, associated with a relevant <a href="#Typesaisie">input type</a>?

* Test 14.8.1: For each input field, is the expected input format associated with a relevant input type?

</p> See the <a href="#NT1">technical note about new form input types</a>.</p>

##### Mappings
- W3C Mobile Accessibility: [5.1 Set the virtual keyboard to the type of data entry required](http://www.w3.org/TR/mobile-accessibility-mapping/#set-the-virtual-keyboard-to-the-type-of-data-entry-required).

###### Level mapping
</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

#### 14.9 [A] The <a href="#Elemadj">adjacent interactive elements</a>, triggering the same action, must be grouped into a single element, has this rule been followed?

* Test 14.9.1: The <a href="#Elemadj">adjacent interactive elements</a>, triggering the same action, must be grouped into one element, has this rule been followed?

See technique <a href="http://www.w3.org/WAI/GL/WCAG20-TECHS/H2.html">H2: Combining adjacent image and text links for the same resource</a>.

</p> Note: this recommendation refers to a WCAG technique, currently not supported in the RGAA&nbsp;3 technical reference. This requirement should be introduced in RGAA&nbsp;3 in a future update. This criterion 14.9 would then be deleted to avoid duplication.</p>

##### Mappings
- W3C Mobile Accessibility: [4.4 Grouping operable elements that perform the same action](http://www.w3.org/TR/mobile-accessibility-mapping/#grouping-operable-elements-that-perform-the-same-action);
- [WCAG 2.0 Success Criterion: 2.4.4](https://www.w3.org/TR/WCAG20/#navigation-mechanisms-refs);
- [WCAG 2.0 Success Criterion: 2.4.9](https://www.w3.org/TR/WCAG20/#navigation-mechanisms-link).

## Additional Recommendations

These recommendations should also, as far as possible, be taken into account in order to optimize the user experience of users with disabilities, in particular.

It should be noted, however, that some of them may pose problems or be complex to follow for content common to both platforms (desktop and mobile/tactile platforms).

In this context, we have numbered differently these criteria and have prefixed them with the key word "RecoMT-".

### RecoMT-14.1 Does each image conveying information used as an element's background property have a visible alternative?

* Test RecoMT-14.1.1: Does each image conveying information used as an element's background property via CSS, meet one of these conditions?
    * The image is accompanied by a visible text;
    * A mechanism can replace the image with visible text.

#### Reference
- BBC Mobile Accessibility Guidelines: [Background images](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/images/background-images).

</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

### RecoMT-14.2 Is each visible alternative associated with a background image relevant?

* Test RecoMT-14.2.1: Is each visible alternative associated with a background image relevant?

#### Reference
- BBC Mobile Accessibility Guidelines: [Background images](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/images/background-images).

</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level A criterion**.</p>

### RecoMT-14.3 Is each image optimized for the screen size and resolution?

* Test RecoMT-14.3.1: Does each image meet one of these conditions?
    * The image is optimized for the screen size and resolution;
    * A mechanism allows to replace the image with an image optimized for the screen size and resolution.

#### Reference
- W3C Mobile Web Best Practices 1.0: [5.3.5 Graphics](http://www.w3.org/TR/mobile-bp/#d0e1219).

</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level AA criterion**.</p>

### RecoMT-14.4 Is the content order of the page optimized for viewing on a mobile/touch device screen?

* Test RecoMT-14.4.1: Are the most important contents of the page presented first, without requiring to scroll?

#### Reference
- W3C Mobile Accessibility [4.3 Positioning important page elements before the page scroll](http://www.w3.org/TR/mobile-accessibility-mapping/#positioning-important-page-elements-before-the-page-scroll).

</p>The [W3C/WAI note](http://www.w3.org/TR/mobile-accessibility-mapping/), on which this document is based, does not associate a level with this criterion. For information, based on "<a href="https://www.w3.org/TR/UNDERSTANDING-WCAG20/conformance.html">Understanding Conformance</a>", we consider it’s a **level AA criterion**.</p>

## Glossary

### <a name="Elemadj"></a>Adjacent Interactive Elements
All interactive elements such as links, buttons, etc. that are adjacent and that perform the same action or display the same resource.

### <a name="Intergestcomplex"></a>Complex gesture-based interaction
Complex gesture-based interactions involve several successive or synchronized movements. For example, a swipe followed by several taps.
These interactions may present insurmountable difficulties for some users.

Note: The term "synchronized" includes simultaneous gestures and gestures chained without pause.

### <a name="intergest"></a>Gesture-based interaction
Any interaction carried out by gestures triggering an action, in particular via a tactile surface. For example, interactions like a tap  (quick touch, equivalent to a mouse click), a touch (longer than a tap), a swipe or pinching are gesture-based interactions.

### <a name="Typesaisie"></a>Input Type
HTML5 proposes specific input types that, when supported by the device, can be used to optimize input. For example, the <code>tel</code> type will trigger the display of a virtual numeric keyboard.

The input types are:

- <code>text</code>;
- <code>search</code>;
- <code>tel</code>;
- <code>url</code>;
- <code>email</code>;
- <code>password</code>;
- <code>date</code>;
- <code>time</code>;
- <code>number</code>;
- <code>range</code>;
- <code>color</code>;
- <code>checkbox</code>;
- <code>radio</code>;
- <code>file</code>.

### <a name="Margesuf"></a>Sufficient external margin

When controls, such as buttons or actionable texts, are adjacent, it may be difficult for a user to activate them individually if their spacing is not sufficient, especially when this size is close to the minimum required (9mm by 9mm).

The implementation of a margin makes it possible to reduce the errors of activation of adjacent elements. There is no fixed value for this margin because it may depend on the resolution and physical size of the screen.

It must be sufficient, however, regardless of the resolution and the physical size of the screen, to activate without error each interactive component.

As an indication, here are some recommendations for margins references:

* The [BBC mobile accessibility guidelines](http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile/design/spacing) recommend a margin of at least 1 pixel.

* [Google](https://www.google.com/design/spec/usability/accessibility.html) recommends a margin of 8dp

* More references can be found on [Luke Wroblewski's blog](http://www.lukew.com/ff/entry.asp?1085).


### <a name="Taillsuf"></a>Sufficient size
Interactive elements such as buttons and actionable text boxes can be difficult to manipulate if they are insufficient in size on small, or high-resolution device screens.

The size of these areas is not defined in pixels but in millimeters in order to take into account the actual physical sizes of the display devices and the pixel density they offer.

It is up to developers to ensure, regardless of the pixel size used, that the interactive components have a rendered size of at least 9mm by 9mm for use on high resolution screens, in particular.

### <a name="Zonesens"></a>Touch target
Interactive area of ​​the screen associated with gesture-based interaction. Touch targets include buttons, links, form controls, or other interactive elements, or elements made interactive via JavaScript.

## Particular cases

### <a name="CP1"></a>Criterion 14.6
There is a particular case when rotation, tilting or shaking is inherent to the proposed functionality and could not have an equivalent in another mode of interaction.

In this case, the criterion is not applicable.

## Technical Notes

### <a name="NT1"></a>Note about new form types
For accessibility to "work", the various HTML elements must have been integrated on the various platforms. However, there may be significant inconsistencies, regarding the support of new form types, on desktops and mobile/touch platforms.

Some types, such as <code>date</code> or <code>time</code>,  can not currently be used in a consistent way. This generally requires the use of components developed using JavaScript and WAI-ARIA.

In other cases, such as with <code>number</code>,  in desktop browsers that do not support it, the degradation is acceptable, allowing them to be used in a mobile/tactile context.

It is up to the content authors and the auditor to determine, on a case-by-case basis, the applicability of the criterion.

In the case where a form type could not be used in a mobile/tactile context, due to its lack of support on a particular desktop browser, it is acceptable to consider the criterion as non-applicable. 

## Resources and References

* <a href="http://www.w3.org/TR/mobile-accessibility-mapping/">Mobile Accessibility: How WCAG 2.0 and Other W3C/WAI Guidelines Apply to Mobile</a>
* <a href="http://www.bbc.co.uk/guidelines/futuremedia/accessibility/mobile">BBC Standards and Guidelines for Mobile Accessibility</a>
* <a href="http://www.w3.org/TR/mobile-bp/">Mobile Web Best Practices 1.0</a>
* <a href="http://www.w3.org/TR/mwbp-wcag/">Relationship between Mobile Web Best Practices (MWBP) and Web Content Accessibility Guidelines (WCAG)</a>
* <a href="http://www.w3.org/WAI/mobile/experiences">Barriers Common to Mobile Device Users and People with Disabilities</a>
* <a href="http://www.w3.org/TR/mobileOK-basic10-tests/">W3C mobileOK Basic Tests 1.0</a>
* <a href="http://www.funka.com/en/our-assignments/research-projects/archive---research-projects/mobile-navigation-guidelines/">Funka Mobile Navigation Guidelines</a>
* <a href="https://checklists.opquast.com/web-mobile/">Opquast Web Mobile (in French)</a>
* <a href="https://developer.mozilla.org/en-US/docs/Web/Accessibility/Mobile_accessibility_checklist">Mobile accessibility checklist</a>.

## Licence
This document is the property of the <span lang="fr">Secrétariat général à la modernisation de l'action publique</span> (SGMAP). It is placed under [Open Licence 1.0 or later (PDF, 541 kb)](http://ddata.over-blog.com/xxxyyy/4/37/99/26/licence/Licence-Ouverte-Open-Licence-ENG.pdf), equivalent to a Creative Commons BY licence. To indicate authorship, add a link to the original version of the document available on the [DINSIC's GitHub account](https://github.com/DISIC).