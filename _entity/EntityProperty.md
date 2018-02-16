---
layout: entry
title: "Entity Property"
shortdef: "entity properties"
order: 6
---

{% comment %}TODO: entity type introduction {% endcomment %}

<!-- details -->

### Attribute; Reaction states

"Substrate(s)", "product(s)", "intermediate(s)", and "transition
state(s)", which are reaction states, will be annotated in this
category. In addition, their `EntityAttribute` will be identified as
`ReactionState`.  Those words, which describe the characteristics of
these reaction states, such as "covalent", "tetrahedral", and
"negatively-charged", will be included in the annotation (see example
1).

{% include image.html name="state.png"
   caption="Example 1"
%}

Moreover, if the functional groups or “enzyme” are indicated adjacent
to these words, these functional groups or “enzyme” must be included
into the reaction states. Such functional groups or “enzyme” must be
connected by “whole_part” relations with the words indicating
“Reaction States”, described below in the section of “Relations” (see
examples 2-4).

{% include image.html name="state-whole-part-1.png"
   caption="Example 2"
%}
{% include image.html name="state-whole-part-2.png"
   caption="Example 3"
%}
{% include image.html name="state-whole-part-3.png"
   caption="Example 4"
%}

On the other hand, if the independent “compounds” are indicated
adjacent to these words, such compounds are not included in the
annotation. In that case, the compounds must be connected by
“correspond_to” relations with the words indicating “Reaction States”,
described below in the section of “Relations” (see example 5).

{% include image.html name="state-corresponds-to.png"
   caption="Example 5"
%}

Furthermore, “complexes” of enzyme structures with their
corresponding ligand will be annotated in this category, with their
“EntityAttribute” identified as “ReactionState”. If the enzyme and its
ligand molecules are indicated along with “complex”, the “enzyme”
and “ligand molecules” will be included along with “complex” in the
annotation, and the relationships will be annotated with “whole_part”
from “complex” to “enzyme” or “ligand”, described below in the section of “Relations” (see examples 6-7).

{% include image.html name="complex-whole-part-1.png"
   caption="Example 6"
%}
{% include image.html name="complex-whole-part-2.png"
   caption="Example 7"
%}

### Attribute; Reactive parts

The phrases such as “leaving group”, “acceptor group”, “scissile bond”
and “cleavage bond”, which generally describe reactive parts of
compounds or enzyme functional groups, will be annotated in this
category. Occasionally, the words “group”, “moiety” or “bond” can be
abbreviated in these phrases.

### Other entity properties

“Active site” and “binding site” will be annotated in this
category. In addition, some “motif(s)”, “region” and “sequence”, which
indicates some specific part of enzymes, will be annotated in this
category.

- binding motif(s)
- signature motif(s)
  - conserved ***(113)RTXGISTT*** motif
  - conserved ***(14)HXGH*** motif
  - analogous ***HXGH*** motifs
  - ***histidine*** motif
- binding region(s)
- region(s)
  - (multiple) regulatory regions
  - ***primed*** region
  - ***single-stranded*** regions
  - ***Mn2*** region

“Mutation” or those words that describe mutations, such as
“replacement”, and “change”, will be included in this category.
The ***emphasized*** words can be replaced with other phrases.

Some parameters, such as the following, will also be annotated as
“entity property”.

- k(cat)
- k(cat) values
- kcat
- k(cat)/K(m)
- k(cat)/K(m) value
- kcat/KM
- kcat/Km
- log(k(cat))
- log(k(cat)/K(m))
- pKa
- pK(a)
- Ki
- Ki values
