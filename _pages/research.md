---
layout: page
permalink: /research/
title: research
description: Research statement — track record and future plans in empirical performance studies.
nav: true
nav_order: 3
toc:
  sidebar: left
---

## Track record

My research lies in **empirical performance studies**, a field that treats recordings as primary evidence for how musical works have been interpreted and for how interpretation has changed over time. My doctoral thesis, submitted to the University of Aberdeen in 2025, is the first systematic empirical study of Beethoven's five sonatas for piano and cello across the full eight decades of their recorded history. It is a 346-page contribution to a body of work that includes José Bowen's and Nicholas Cook's foundational studies of tempo and expressive flexibility, Daniel Leech-Wilkinson's portamento research, Marten Noorduin's historiographical account of Beethoven's tempo indications, and the broader CHARM tradition.

Three substantive contributions have emerged from this research and now form the basis of five papers and of a planned monograph.

### A methodological contribution

I developed a formalised **manual bar-by-bar tempo-measurement protocol** for polyphonic chamber recordings, in response to the systematic failure of automated beat-detection tools on historical duo material. The protocol rests on a cumulative timestamp architecture that prevents error accumulation, permits internal self-validation, and captures the expressive timing phenomena (rubato, fermatas, ritardandi) that automated tools suppress. It was developed in cross-disciplinary collaboration with an engineer specialising in VLSI design, and its error model, data architecture and quality-control procedures are characterised in full. The complete dataset and analysis code are publicly available, and the protocol has been designed from the outset to be adopted and extended by other researchers.

### A substantive finding about stylistic change

Applying **k-means clustering** to the bar-level BPM data, I have shown that every movement of the five sonatas supports at least two and usually three discrete tempo traditions (slow, mid-range, fast) whose internal regression slopes are negligible across the entire 1930–2012 period. The dominant mid-range tradition has been internally stable across eight decades; what has changed at the aggregate level is a shift in the relative prevalence of coexisting traditions, not a uniform drift of all performers toward a new norm. This supports what I call an **ecological model of stylistic change**: coexisting traditions fluctuate in relative density, rather than a single tradition evolving. It reframes how corpus-level regression results in earlier performance studies should be interpreted.

### A finding about Beethoven's historical tempo indications

My comparative analysis of **Czerny's, Moscheles's and Kolisch's** markings against the recorded corpus documents systematic gaps ranging from 11–20% in fast movements to 37–39% in some slow movements. Kolisch's 1943 markings, derived without corpus evidence, align considerably more closely with recorded practice than either Czerny's or Moscheles's — a striking result that suggests his musical intuitions tracked something the broader tradition had not yet been able to measure. From this comparison I propose a set of revised tempo indications grounded in the statistical modal tempi of the corpus, presented as ranges rather than single prescriptive values, and offered as evidence-based reference points rather than claims about Beethoven's intentions.

## Future plans

My immediate priority is the publication of the doctoral work **in book form**. I plan to submit a monograph proposal to a major university press within the next year, incorporating the five papers as revised chapters and adding substantial new material on Beethoven's historical pianos, the cultural history of portamento, and the implications of the ecological model for performance studies as a discipline.

In parallel, I intend to **extend the methodology to the Beethoven violin sonatas and selected string quartets**. The violin sonatas are an obvious test case because their recorded tradition is richer than the cello sonatas' and because violin technique and portamento history diverge from cello practice in instructive ways. A full clustering analysis would test whether the three-tradition structure generalises across Beethoven's chamber output.

A third direction is **methodological**: developing my spline-CDF smoothing procedure into a standalone, documented open-source tool, published with a short methods paper, so that other researchers can adopt it for performance-corpus analysis without implementing it from scratch. A related project is a full open-source implementation of the five-tool visualisation suite as a Python package.

A fourth direction is a **hybrid manual-and-automated audio-analysis pipeline** for polyphonic chamber recordings, in which the manual protocol generates training and validation data for more targeted automated tools. This would give music-information-retrieval researchers a principled way to validate their models on historical material, and give musicologists a path to scalability. The pipeline would be designed to be adaptable beyond the Western canon.

Finally, I am committed to the **public dimension** of this research. My open-access dataset and code are already freely available, and I would like to continue developing resources that make empirical performance analysis more accessible to performers, teachers and students. The gap between the tempo indications students are taught to respect and the tempi expert performers have actually adopted across the recording era has immediate pedagogical implications.
