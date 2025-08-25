---
title: Colour works best when it's tested for everyone
date: 2025-08-24
description: A deep dive into the accessibility colour assessment for the GOV.UK refresh
tags:
  - design
  - accessibility
---

As part of work in GDS I pride myself on making sure that we take accessibility and usability seriously. This is something that my colleagues are exceptionally brilliant and ensures happens too, and the work done to refresh [GOV.UK](http://gov.uk) has been no exception to this.

Although [logos are exempt from the colour contrast](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html) under the [Web Content Accessibility Guidelines](https://www.w3.org/TR/WCAG22/) 2.2 (WGAC 2.2), we wanted to explore the potential impact that the new cyan colour could have on users.

The cyan accent colour has been an accessibility concern since its initial design conception. WCAG 2.2 guidelines state that regular text must pass to a 4.5:1 ratio, whereas large text, UI components and graphics must pass to a 3:1 ratio.

When designing the designers within the project soon realised that the cyan colour could not be used against a white background due to its 1.28:1 ratio, failing WCAG 2.2 colour contrast guidance. As a concession, we agreed that this colour could only be used against the brand blue background.

As this is a significant change from the previous brand, I wanted to go one step further and understand how our users may see the main accent and core brand colour, if they have vision impairment issues such as colour vision deficiency.

## What is colour vision deficiency?

Colour vision deficiency (CVD), also known as colour blindness, is a condition that makes it harder for some people to distinguish certain colours. It can be caused by other conditions, aging or medications. CVD is more prevalent in men and affects around 1 in 10 men compared to 1 in 100 women.

People with CVD can have a vision that ranges from almost normal colour perception to almost total absence of perception of red, green or blue light. It is also possible to have more than one type of CVD.

Protanomaly is a reduced sensitivity to red light, affecting 1.3%[<a href="https://www.whocanuse.com">1</a>] of the population, or approximately 887,900[<a href="https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/bulletins/annualmidyearpopulationestimates/mid2023">2</a>] people have this condition in the UK. To put this into terms that can be imagined, this is more than the population of Leeds[<a href="https://www.ciphr.com/infographics/biggest-cities-in-the-uk-by-population">3</a>].

Deuteranomaly is a reduced sensitivity to green light, affecting 5.3% of the population or approximately 3.6million people have this condition in the UK. To put this into terms that can be imagined, this is more than the population of Wales[<a href="https://www.gov.wales/mid-year-estimates-population-2023-html">4</a>].

People with deuteranomaly and protanomaly are often incorrectly diagnosed collectively as ‘red-green’ colour blind because both types generally have difficulty distinguishing between reds, greens, browns and oranges. They also commonly confuse different types of blue and purple hues and many other colour combinations.

Tritanomaly is a reduced sensitivity to blue light, affecting 0.02% of the population or approximately 13600 people have this condition in the UK. This is the rarest type of CVD. People with tritanomaly have difficulty identifying differences between blue and yellow, violet and red and blue and green. To these people the world appears as generally red, pink, black, white, grey and turquoise.  

## Applying knowledge to our work

The Department for Education has developed a tool[<a href="https://accessibility.education.gov.uk/app/how-many-people/11300000">5</a>] that can estimate the number of people who might have a disability or impairment when using a service. We estimate that GOV.UK has approximately 11.3 million weekly visitors.

Using this tool we could estimate that 8,701,000 people would have some form of visual impairment, including blindness, low or poor vision and other conditions like cataracts. For those who have a colour vision deficiency or colour blindness, we estimated that 904,000 men and 90,400 women would be affected.

We were able to break that down further, into the three main types of CVD, with:

-   protanomaly affecting approximately 146,900 users    
-   deuteranomaly affecting approximately 598,900 and
-   tritanomaly affecting approximately 2,260 users.

## What we did next

To understand what someone with CVD sees I needed to use a simulator. It is important to state that simulations are never perfectly accurate. There are variables that we are unable to control that differ in every situation, as well as human perception.  

I used using the Brettel 1997[<a href="https://pubmed.ncbi.nlm.nih.gov/9316278/">6</a>] method for testing all three types of simulated CVD and the Viénot 1999[<a href="https://vision.psychol.cam.ac.uk/jdmollon/papers/colourmaps.pdf">7</a>] and Machado 2009[<a href="https://www.researchgate.net/publication/38015459_A_Physiologically-Based_Model_for_Simulation_of_Color_Vision_Deficiency_vol_15_pg_1291_2009">8</a>] methods for protanopia and deuteranopia. I also tested the image at a severity of 0.5 and 1 respectively. In this instance severity is the extent to which a person has a CVD condition.

## Table of test results

### Protanopia/Protanomaly 

Severity of condition: 0.5 

Background hex: #2E6FB7 / Dot: #B6F8DF

Colour contrast ratio:  4.29:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Fail AA and AAA |
| Large text: | Pass AA, Fail AAA |
| Objects and UI: | Pass AA |

Severity of condition: 1 

Background hex: #3A6EB7 / Dot: #F7F1DF

Colour contrast ratio:  4.54:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Pass AA, Fail AAA |
| Large text: | Pass AA and AAA |
| Objects and UI: | Pass AA |

### Deuteranopia/Deuteranomaly 

Severity of condition: 0.5 

Background hex: #2A6EB8 / Dot: #9FEEE1

Colour contrast ratio:  3.92:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Fail AA and AAA |
| Large text: | Pass AA, Fail AAA |
| Objects and UI: | Pass AA |

Severity of condition: 1 

Background hex: #346CB8 / Dot: #D8DBE2

Colour contrast ratio:  3.8:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Fail AA and AAA |
| Large text: | Pass AA, Fail AAA |
| Objects and UI: | Pass AA |

### Tritanopia/Tritanomaly 

Severity of condition: 0.5 

Background hex: #0074A7 / Dot: #3DF9FE

Colour contrast ratio:  3.98:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Fail AA and AAA |
| Large text: | Pass AA, Fail AAA |
| Objects and UI: | Pass AA |

Severity of condition: 1

Background hex: #007994 / Dot: #57F4FE

Colour contrast ratio:  3.88:1 

| WCAG text and images | Pass or Fail |
| ----------- | ---------- |
| Normal text: | Fail AA and AAA |
| Large text: | Pass AA, Fail AAA |
| Objects and UI: | Pass AA |


This information has been incredibly useful in helping the appropriate teams write the guidance around dot and wordmark usage. Without the insights we gained from the enhanced colour palette testing and we may have inappropriately stated that this is usable.