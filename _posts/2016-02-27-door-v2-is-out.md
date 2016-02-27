---
layout: post
title: DoOR 2.0 released and published
published: true
author: Dahaniel
comments: true
date: 2016-02-25 09:02:40
tags: DoOR, Drosophila, ensemble code, database, publcations
categories: research
permalink: /2014/02/door_v2
---
Great news for the DoOR project, the paper on our comprehensive update of the _Database of Odorant Responses_ was [published in _Scientific Reports_](http://www.nature.com/articles/srep21841) a few days ago [[^1]]. With the paper being published I also finally set the versions of [DoOR.functions](https://github.com/Dahaniel/DoOR.functions) and [DoOR.data](https://github.com/Dahaniel/DoOR.data) 2.0 and created releases on [GitHub](https://github.com/Dahaniel/DoOR.functions/releases) and [Zenodo](http://dx.doi.org/10.5281/zenodo.46555). The updated web page for quick queries is available at [http://neuro.uni.kn](http://neuro.uni.kn).

The database now holds responses for 7381 different odorant-receptor combinations. In total we added 15 new data sets from 11 studies adding 467 new odorants summing up to a total of 2894 new responses to DoOR. The Raw data used for calculating the consensus database consists of 11337 individual data points. Running the merging process (i.e. trying all 7,714,976 possible combinations of pairwise study merges; see paper for details) with 100 jobs in parallel on a cluster took more than a week.

Checkout the new documentation (R vignettes) to find out about the new [functions](http://neuro.uni-konstanz.de/DoOR/content/doc/DooR.functions_main.html), [tools](http://neuro.uni-konstanz.de/DoOR/content/doc/DoOR_tools.html) and [visualizations](http://neuro.uni-konstanz.de/DoOR/content/doc/DoOR_visualizations.html) DoOR offers. For example, I wrote a little _sensillum identification tool_ which will hopefully be helpful for people performing single sensillum recordings (`identifySensillum()`). With `dplot_ALmap()` you can now quickly produce antennal lobe activity maps for your odorant of interest, visualized with Veith Grabe's beautiful _in vivo_ AL map.
![output of dplot_ALmap](/assets/DoOR2.0_AL.png)



The [project web page](http://neuro.uni.kn/DoOR) got a complete facelift, tables can now be sorted by clicking the headers and we link to several additional external sources [ChEBI](https://www.ebi.ac.uk/chebi/), [ChemSpider](http://chemspider.com) and the [Virtual Fly Brain](http://www.virtualflybrain.org/).

So if your work is somehow related to olfaction, if you are a physiologist or need data for modeling, checkout DoOR and tell me what you think!

### References

[^1]: Münch, D., Galizia, C.G., 2016. DoOR 2.0 - *Comprehensive Mapping of Drosophila melanogaster Odorant Responses.* Scientific Reports 6, 21841. doi:10.1038/srep21841
