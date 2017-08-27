---
author: Neel Smith
title: Parsing Greek morphology
date: ICGLE, August 29, 2017
header-includes:
    - \setsansfont{Gentium}
---

# ... in multiple dialects and alphabets

---



# Digital scholarship and Classics


-   25 years ago: a leading discipline
-   today: largely absent from new areas of textual analysis?


---


# Example: latent pattern recognition

-    topic modelling
-    semantic relations with embedded word vectors

---

# Some reasons, good and bad

-   corpus size vs. tolerance for imprecise editions
-   **morphological complexity**


---

# Motivation

Homer Multitext project: manuscripts with

-   multiple dialects
-   unattested vocabulary
-   distinct orthographies

![The Venetus A manuscript](imgs/VA012RN-0013.jpg)

---

# Limitations of current standards


-   ISO 639* family: Greek dialects not recognized
-   Unicode:
    -   language and script conflated
    -   epichoric scripts not recognized
    -   confusion of multivalent and contradictory glyphs

---


# In 2017, it is (still!) not possible to encode Greek


---



![A Vienna secession?](imgs/secession.png)


---



# A corpus-linguistic perspective

Every corpus is characterized by:

-    a unique lexicon
-    a unique set of inflectional rules


---

# "Greek" is defined by *analytical categories*


- "noun" (GCN)
- "adjective" (GCND)
- "conjugated verb" (PNTMV)
- "infinitive" (TV)
- "participle" (GCTMV)
- "verbal adjective" (GCN)
- "adverb" (Degree)
- "indeclinable" (part of speech)


---

"Analysis by synthesis" algorithm



---

FSA not expressive enough for Greek morphology

crossing of lexical and inflectional properties of Greek accent cannot be reduced to context-free state transitions

---

# A simple worked example

---


Andocides *On the Mysteries* 1.96

> Νόμος. ἔδοξε τῇ βουλῇ καὶ τῷ δήμῳ.

---

IG 1.3, 156

![Decree honoring Leonides of Halicarnassus](imgs/decree-masked.png)


---

# Vocabulary ("stems")

![Nouns, in Attic](imgs/attic-noun-stems.png)

![Nouns, in literary Greek](imgs/lit-noun-stems.png)

---

# Inflectional rules

![Nouns, in Attic](imgs/attic-noun-infl.png)

![Nouns, in literary Greek](imgs/lit-noun-infl.png)

---

# Analysis

![literary Greek](imgs/analysis-lit.png)

---


# Analysis

![Attic Greek](imgs/analysis-attic.png)




---


# Generated


![literary Greek](imgs/generator.png)

---

# Pipeline

Output of Attic analysis fed as input to literary generator:


![From Attic to literary Greek](imgs/pipeline.png)


---

# Possibilities




---

# Current state

---

# Thank you!

For more information:

-   "Morphological Analysis of Historical Languages," *BICS* 59-2 (2016) 89-102.
-   <https://github.com/neelsmith/kanones.git>
