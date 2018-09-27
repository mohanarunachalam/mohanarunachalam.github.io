---
title: Building the Open Source Drug Discovery Ecosystem
published: true
layout: post
---

We are currently undergoing a transition where software is becoming increasingly important for drug discovery. While parts of the drug discovery pipeline [1] have used sophisticated computational methods for decades, other domains such as clinical trials use scarcely any software beyond Word or Excel. This situation is unfortunate, because there already exists a strong, albeit fragmented, ecosystem of open source datasets. Unifying this ecosystem and making it accessible from open source software packages like DeepChem will accelerate the process of discovering new medicines. In this essay, we explore what good open source tooling for disease selection and clinical trial management might look like, and comment on good directions for open algorithmic development.

The first stage of the drug discovery pipeline involves disease selection (which disease are you trying to treat?). Most modern drug discovery programs start with scientists carefully reading through the scientific literature to build internal mental models of chosen disease areas. There don't currently exist good open source tools for algorithmically and systematically picking diseases and indications to target. The construction of open source APIs for disease selection that tie into available public databases could accelerate the drug discovery process by allowing scientists to systematically explore hypotheses around treatment strategies.

As I've discussed elsewhere [1], target driven drug discovery revolves critically around the identification of a particular macromolecule or macromolecular system whose (mis)behavior is believed to be a causal factor for a disease. A number of good open source resources exist for finding novel targets [2]. The therapeutic target database [3] lists known protein targets linked with diseases and available drugs. This data source is valuable when doing exploratory analysis on a new disease area when it’s desirable to quickly pull up known facts and treatments. Good open source tooling would enable rapid querying of this resource from within a python library such as DeepChem with a simple method invocation. 

Increasingly, it’s becoming possible to get started with drug discovery without identifying explicit protein targets. One such approach exploits data drawn from functional genomics experiments. The Gene Expression Omnibus [4], a database of known gene expression datasets which can be used to discover putative drugs without initially identifying an explicit target up front. Gene expression data provides a window into the internal state of cells. By using expression data from diseased cells, and comparing with data from cells dosed with putative drugs, it can be feasible to find drugs with “cancel out” diseased expression states [5]. Open source tooling which provided algorithmic access to this data and allowed for easy construction of these “cancellation” models would be a powerful tool in the hands of any drug discovery team.

Another non-target driven approach uses microscopy data to understand the visual effect of putative drugs on cells state. The Broad Biomage Benchmark Collection [6] provides some first datasets to get started in the space. Good open source tooling would likely provide some convolutional neural networks, hopefully pretrained, which would be capable of rapidly classifying or clustering basic phenotypes. Some tools could accelerate the adoption of microscopy driven drug discovery by allowing experimentalists to focus on other challenges.

Yet another non-target driven approach focuses on utilizing information from large scale genomic studies. The basic idea is to associate disease (or lack thereof) with mutations in patients. Such linkages can be extracted from large scale genomic databases which have patients’ genomes alongside their physical conditions. This strategy has been most famously exploited to inhibit PCSK9 by Amgen and Regeneron [7]. In this case, exception patients without very low LDL cholesterol were discovered who had non-functional PCSK9 proteins coded into their genomes. Scientists reasoned that inhibiting PCSK9 in healthy patients could induce some portion of the same benefit, and this hunch has been subsequently proven out with experimental work. Good open source tooling in this space could connect python toolchains with databases such as SNPedia [8], the cancer genomics atlas [9], or the personal genome project [10] to allow for systematic investigation of such linkages. By cross-correlating this information with other target discovery mechanisms listed above, it might be possible to find very compelling and so far undiscovered treatment strategies.

So far, we’ve discussed strategies for picking a disease and target to treat. Once we have a chosen disease and target, we are in friendlier open source territory. Libraries like DeepChem provide sophisticated tools for helping develop (small molecule) compounds which could potentially treat a desired disease. Such tools provide reasonable support up until the end of the preclinical drug discovery process [1]. However, afterwards we enter the clinical drug discovery ream, where a software desert awaits us.

Good software tools for clinical trials don't yet exist; treatment efficacy for many diseases are still measured with subjective tests. For example, the walk test [11] measures the effectiveness of multiple sclerosis treatments by having patients walk 25 feet and having doctors score patient gait. Given that patients are probably only seen at most at monthly intervals, there’s no chance that doctors will carefully be able to analyze changes in gait. Good open source software tooling should enable video recording of such trials and use video deep learning techniques to automatically cluster patient gaits and allow for interactive comparisons. In general, all data for clinical trials should be video logged and analyzed. Doctors rely critically on their eyes to gauge patient health, and we need to create open source tooling that enables our clinical algorithms to “see” as well.

Furthermore, there should be good access to records of past clinical trials. clinicaltrials.gov [12] has standardized reporting of information about clinical trials in the US. Providing open algorithmic access to this data would allow researchers to mine past trials for potentially missed clues or treatments that were perhaps misjudged by past trials. Most of this data is in free text form, and the development of good deep natural language tooling will be required to make sense of this information source.

As a general note, it's a curious fact that none of the algorithms or models of disease mentioned so far in this essay include basic details of physiology, such as the fact that humans have hearts, fist sized organs that circulate blood by beating. The lack of such "common sense" in existing computational models (open or proprietary) is a sign that much algorithmic development remains to be done for drug discovery. Greater integration of systems biology and machine learning might help here. There have already been a number of interesting research initiatives in this space, such as computational whole cell modeling [13] or the OpenWorm [3] initiative that aims to model C. Elegans in exquisite detail. It sounds like it would be perfect time to start an OpenHuman initiative!

I hope that readers walk away convinced that open source tooling for drug discovery could have transformative effects. By pooling know-how and making it easy to access (already open) datasets, we might enable the rapid treatment of diseases which remain ignored today.

[1] http://rbharath.github.io/a-short-overview-of-drug-discovery/

[2] https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4785018/

[3] http://bidd.nus.edu.sg/group/cjttd/ 

[4] https://www.ncbi.nlm.nih.gov/geo/

[5] http://stm.sciencemag.org/content/3/96/96ra77

[6] https://data.broadinstitute.org/bbbc/image_sets.html  

[7] http://blogs.sciencemag.org/pipeline/archives/2017/03/20/what-pcsk9-is-telling-us-about-drug-discovery 

[8] https://www.snpedia.com/ 

[9] https://cancergenome.nih.gov/

[10] https://en.wikipedia.org/wiki/Personal_Genome_Project 

[11] http://www.nationalmssociety.org/For-Professionals/Researchers/Resources-for-Researchers/Clinical-Study-Measures/Timed-25-Foot-Walk-(T25-FW) 

[12]  clinicaltrials.gov 

[13] http://www.cell.com/abstract/S0092-8674(12)00776-3

[14] http://www.openworm.org/ 
