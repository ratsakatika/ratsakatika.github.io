---
layout: page
title: AI, Remote Sensing & Old-Growth Forests
description: My PhD research will apply artificial intelligence to fused remote sensing data to map and value old-growth forests in Romania’s Carpathian Mountains.
img: assets/img/drone.jpg
redirect:
importance: 1
category: artificial intelligence
related_publications: true
---

**My PhD will leverage remote sensing data and state-of-the-art (SOTA) processing pipelines to identify old-growth forests in Romania's Carpathian Mountains, and evaluate the forests' value in terms of biodiversity and carbon.** The research will collaborate with [Fundația Conservation Carpathia (FCC)](https://www.carpathia.org/), who will provide scientific and contextual knowledge, and an existing dataset of 300 mobile laser plot scans, high-resolution drone imagery, and a comprehensive GIS database (including the locations of catalogued and potential old-growth forests). This will be complemented with further data collected in the field. The original PhD proposal is below. I will update this page will outputs from my research as it progresses.

{% include figure.liquid loading="eager" path="assets/img/rucar.jpg" title="Map of mountain village nested in a valley" class="img-fluid rounded z-depth-1" %}
_Figure 1: The village of Rucar nested in Romania's Carpathian Mountains_ [^44].

## PhD Proposal - 22 July 2024

**Thomas Ratsakatika<sup>1</sup>, Srinivasan Keshav<sup>2</sup>, Mihai Zotta<sup>3</sup>, [Emily Lines<sup>1</sup>](https://www.linesresearchgroup.com/)**  
<sup>1</sup> Department of Geography, University of Cambridge, <sup>2</sup> Department of Computer Science and Technology, University of Cambridge, <sup>3</sup> Fundația Conservation Carpathia

### Motivation and Context

Old-growth (also known as primary) forests are complex ecosystems that have developed over long periods, resulting in unique ecological, economic, and cultural benefits. They account for approximately one-third of the world's total forested area [^1]. Specific definitions of old-growth forests vary across geographies and contexts; however, they are often characterised by diverse tree ages, complex tree structures, multilayered canopies, coarse woody debris, and no clearly visible indications of anthropogenic disturbance to ecological processes [^2], [^3], [^4]. Old-growth forests' structural complexity and long-term stability provide unique and irreplaceable habitats that support rich biodiversity, which includes many endangered species [^5], [^2]. They also provide critical ecosystem services, including climate regulation [^6], water cycle management [^7], carbon storage [^8], carbon sequestration [^9], soil management [^10], pathogen control [^11], and medicine discovery [^2]. Despite these benefits, old-growth forests are being destroyed at an alarming rate [^2]. Approximately 47 million hectares of old-growth forest were lost between 2000 and 2020 [^3] - an area larger than Sweden. Historically, deforestation has been particularly high in Europe. Half of Europe's forests were cleared by the Middle Ages [^12] and today, less than 3% of Europe's old-growth forests remain intact [^13].

Romania's Carpathian Mountains are home to Europe's largest remaining tracts of old-growth forests outside of Scandinavia and Russia [^14]. The unique ecosystem is rich in biodiversity and supports some of the continent's largest populations of brown bears, wolves, and lynxes [^15], [^16], [^17]. However, post-Soviet restitution laws that intended to restore property rights to individuals and communities inadvertently led to increased legal and illegal logging. 250,000 hectares of forest were lost between 1990 and 2012 (6% of the total afforested area) [^18]. Today, an estimated 525,000 hectares of Romania's old-growth forests remain nationally, much of which is unprotected [^14]. Where protections do exist, limited public consultation and education, and misalignments between Romanian and EU legislation (e.g. Natura 2000) undermine effective management [^19], [^20], [^21]. Economic interests and governance challenges in the logging sector are also major obstacles to law enforcement [^22]. Positive developments include Law 97/2023 for Protecting Remarkable Trees, which targets "Large Old Trees" (LOTs) [^23]. LOTs are defined as either being older than 160 years, having a minimum taxon-specific trunk circumference, or being "subject to local legends and stories." However, a peculiarity of this law is it only applies to trees outside of forests.

Several organisations operate in Romania to conserve and restore forest ecosystems, the largest of which is Fundația Conservation Carpathia (FCC). Established in 2009, FCC aims to create Europe's largest forest wilderness National Park in the Făgăraș Mountain Range of the Southern Carpathians (Fig. 2) [^24]. To better plan its forest management and conservation work, FCC requires a more detailed understanding of the spatial distribution of old-growth trees and old-growth patches.

### Related Work

Recent advances in remote sensing methods, including terrestrial laser scanning (TLS), mobile LiDAR, unmanned aerial vehicle (UAV) scanning, and earth observations (EO), have revolutionised our understanding of forest ecosystems [^25], [^26]. Machine learning has underpinned recent advances in the methods used to process these large datasets, including for tree segmentation [^27], species classification [^28] and biomass calculations [^29]. There is a growing literature on the use of these tools to detect old-growth forests [^30]. Tree structure analysis using aerial laser scanning (ALS) has been used to identify old-growth forests in Australia, Canada, France, Norway, and Spain [^31], [^32], [^33], [^34], [^35], [^36], and spaceborne LiDAR (GEDI) has been used to describe their structural characteristics in the Ukrainian Carpathians [^37]. Many opportunities remain to apply these tools to new data and develop new tools to analyse existing data, providing more detailed and accurate information to support conservation.

### Research Questions and Methods

This research will aim to answer three questions (RQs):

1. **Can remote sensing data accurately locate old-growth individual trees and old-growth patches at scale in the Făgăraș Mountains?** FCC's 300 mobile LiDAR plot scans will be combined with tree canopy dimensions derived from high-resolution UAV and EO data to create a labelled LOT dataset. Machine learning-based tree segmentation and classification pipelines will then be trained to identify and quantify old-growth trees at a landscape scale automatically. The trade-off between accuracy, scalability, and cost of different remote sensing data sources will be assessed to determine the optimal workflow for ongoing monitoring.
2. **Is the accuracy and scalability of remote sensing data sufficient to inform an actionable over-logging detection system?** The workflow developed in RQ1 will be integrated into a logging alert system. The objective will be to improve on existing systems (e.g. Lens, Global Forest Watch [^38], [^39]) by incorporating analysis of old-growth trees. The update frequency for the system will be at least one month to help ensure insights are actionable and impactful.
3. **Can the value of old-growth forests in the Făgăraș Mountains be evaluated in terms of biodiversity, carbon storage and/or carbon sequestration?** The objective is to provide a scientific basis for FCC's conservation advocacy with communities. TLS, UAV and EO data can be used to estimate old-growth forests' carbon value accurately and efficiently. Biodiversity can be assessed by using camera trap data on keystone species (e.g. brown bears [^40]), building on my MRes thesis, which used AI to monitor wildlife in the Carpathian Mountains [^41].

Chapter 1 of the thesis will cover the introduction and literature review. Chapters 2-4 will address the three research questions, including methods, results and discussion. Chapter 5 will conclude.

### Work Plan and Timeline

- **Months 1-3 (Oct-Dec 2024).** Review and document the literature on Romania's old-growth forest ecosystems, Romania's legislative and political economy context, and forest data collection and processing methods. Develop a deep understanding of FCC's data as a starting point for further analysis. Develop a working knowledge of the SOTA machine learning tools, prioritising those developed by the Lines Research Group [^42], [^28], [^43]. Potential fact-finding field visit.
- **Months 4-6 (Jan-Mar 2025).** Apply the SOTA tools to FCC's datasets and evaluate their strengths and weaknesses in answering RQ1. Develop methods for answering RQ3 that are feasible within the PhD timeline. Plan a field visit to the Făgăraș Mountains to collect additional data required to answer RQ1. Determine which biodiversity sensors must be deployed during the field visit to answer RQ3 (enabling 1-2 years of data collection).
- **Month 7-9 (Apr-Jun 2025).** Undertake a field visit to the Făgăraș Mountains to collect data for RQ1 & 3. Analyse initial results while in the field and collect additional data as necessary. Develop a detailed Year 2 work plan to address RQ2 & 3. Write up the first-year report.
- **Month 10-12 (Jul-Sep 2025).** Record Year 1 progress in a draft of Chapters 1 & 2 of the thesis.
- **Year 2 (Oct 2025 - Sep 2026).** Develop and finalise RQ1, and build a system for RQ2 and monitor performance. Analyse the initial results for RQ3 and deploy further sensors if necessary.
- **Year 3 (Oct 2026 - Sep 2027).** Finalise results analysis for RQ2 and RQ3. Write up the thesis.

{% include figure.liquid loading="eager" path="assets/img/map.png" title="Map of Romania highlighting the Făgăraș Mountain Range" class="img-fluid rounded z-depth-1" %}
_Figure 2: Map of Romania highlighting the Făgăraș Mountain Range_ [^44].

### References

[^1]: FAO. _The State of the World’s Forests 2022_. FAO; 2022. Available from: http://www.fao.org/documents/card/en/c/cb9360en.
[^2]: Wirth C. Old-Growth Forests: Function, Fate and Value – a Synthesis. In: Wirth C, Gleixner G, Heimann M, editors. _Old-Growth Forests: Function, Fate and Value_. Berlin, Heidelberg: Springer; 2009. p. 465-91. Available from: https://doi.org/10.1007/978-3-540-92706-8_21.
[^3]: FAO, UNEP. _The State of the World’s Forests 2020. In brief._ FAO and UNEP; 2020. Available from: https://openknowledge.fao.org/handle/20.500.14283/ca8985en.
[^4]: Maloof J. _Nature’s Temples: The Complex World of Old-Growth Forests_. Timber Press; 2016. Google-Books-ID: 5ZxzDQAAQBAJ.
[^5]: Franklin JF, Spies TA. Composition, function, and structure of old-growth Douglas-fir forests; 2017. Available from: https://andrewsforest.oregonstate.edu/publications/1242.
[^6]: Gilhen-Baker M, Roviello V, Beresford-Kroeger D, Roviello GN. Old growth forests and large old trees as critical organisms connecting ecosystems and human health. A review. _Environmental Chemistry Letters_. 2022 Apr;20(2):1529-38. Available from: https://doi.org/10.1007/s10311-021-01372-y.
[^7]: Vilhar U. Water Regulation Ecosystem Services Following Gap Formation in Fir-Beech Forests in the Dinaric Karst. _Forests_. 2021 Feb;12(2):224. Available from: https://www.mdpi.com/1999-4907/12/2/224.
[^8]: McGarvey JC, Thompson JR, Epstein HE, Shugart Jr HH. Carbon storage in old-growth forests of the Mid-Atlantic: toward better understanding the eastern forest carbon sink. _Ecology_. 2015;96(2):311-7. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1890/14-1154.1.
[^9]: Luyssaert S, Schulze ED, Börner A, Knohl A, Hessenmöller D, Law BE, et al. Old-growth forests as global carbon sinks. _Nature_. 2008 Sep;455(7210):213-5. Available from: https://www.nature.com/articles/nature07276.
[^10]: Chiti T, Benilli N, Mastrolonardo G, Certini G. The potential for an old-growth forest to store carbon in the topsoil: A case study at Sasso Fratino, Italy. _Journal of Forestry Research_. 2023 Dec;35(1):10. Available from: https://doi.org/10.1007/s11676-023-01660-z.
[^11]: Fodor E, Hărută O. The roles of plant pathogens in old-growth forests. _Bucovina Forestieră_. 2022 Jul;22:41-59.
[^12]: FAO. _State of the World’s Forests 2012_. 2012. Available from: https://www.fao.org/4/i3010e/i3010e00.htm.
[^13]: Greenpeace. _Roadmap to Recovery: The world’s last intact forest landscapes_; 2006. Available from: https://www.greenpeace.org/usa/research/roadmap-to-recovery-the-world/.
[^14]: Schickhofer M, Schwarz U. _Inventory of potential primary and old-growth forest areas in Romania (PRIMOFARO): Identifying the largest intact forests in the temperate zone of the European Union_; 2019.
[^15]: Iosif R, Pop MI, Chiriac S, Sandu RM, Berde L, Szabó S, et al. Den structure and selection of denning habitat by brown bears in the Romanian Carpathians. _Ursus_. 2020 Apr;2020(31e5):1-13. Available from: https://bioone.org/journals/ursus/volume-2020/issue-31e5/URSUS-D-18-00010.1/Den-structure-and-selection-of-denning-habitat-by-brown-bears/10.2192/URSUS-D-18-00010.1.full.
[^16]: Iosif R, Popescu VD, Ungureanu L, Șerban C, Dyck MA, Promberger-Fürpass B. Eurasian lynx density and habitat use in one of Europe’s strongholds, the Romanian Carpathians. _Journal of Mammalogy_. 2022 Apr;103(2):415-24. Available from: https://doi.org/10.1093/jmammal/gyab157.
[^17]: Dyck MA, Iosif R, Promberger–Fürpass B, Popescu VD. Dracula’s ménagerie: A multispecies occupancy analysis of lynx, wildcat, and wolf in the Romanian Carpathians. _Ecology and Evolution_. 2022;12(5):e8921. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1002/ece3.8921.
[^18]: Kucsicsa G, Dumitrică C. Spatial modelling of deforestation in Romanian Carpathian Mountains using GIS and Logistic Regression. _Journal of Mountain Science_. 2019 May;16(5):1005-22. Available from: https://doi.org/10.1007/s11629-018-5053-8.
[^19]: Manolache S, Ciocanea CM. NATURA 2000 IN ROMANIA - A DECADE OF GOVERNANCE CHALLENGES. 2017.
[^20]: Stringer LC, Paavola J. Participation in environmental conservation and protected area management in Romania: A review of three case studies. _Environmental Conservation_. 2013 Jun;40(2):138-46. Available from: https://www.cambridge.org/core/journals/environmental-conservation/article/abs/participation-in-environmental-conservation-and-protected-area-management-in-romania-a-review-of-three-case-studies/EB5F136AA7E07BA948C93AD66B136F82.
[^21]: WWF. Communities in one of the biggest Natura 2000 sites in Romania know nothing of the EU’s network. Available from: https://wwf.panda.org/wwf_news/?201968/Communities-in-one-of-the-biggest-Natura-2000-sites-in-Romania-know-nothing-of-the-EUs-network-of-protected-areas.
[^22]: Ellis G. ‘Timber Mafia’ threatens the future of Romania’s ancient forests. Available from: https://www.aljazeera.com/features/2020/11/26/romania-disappearing-forests.
[^23]: Hartel T, Arghius, V, Stoican F, Réti KO, Bouriaud L. New Law for Old Trees in Romania: lessons and opportunities. Available from: https://conbio.onlinelibrary.wiley.com/doi/10.1111/csp2.13032.
[^24]: FCC. _Fundația Conservation Carpathia | About Us_; 2024. Available from: https://www.carpathia.org/about/.
[^25]: Lines ER, Allen M, Cabo C, Calders K, Debus A, Grieve SWD, et al. AI applications in forest monitoring need remote sensing benchmark datasets. In: _2022 IEEE International Conference on Big Data (Big Data)_; 2022. p. 4528-33. Available from: https://ieeexplore.ieee.org/document/10020772.
[^26]: Nită MD. Testing Forestry Digital Twinning Workflow Based on Mobile LiDAR Scanner and AI Platform. _Forests_. 2021 Nov;12(11):1576. Available from: https://www.mdpi.com/1999-4907/12/11/1576.
[^27]: Puliti S, Pearse G, Surový P, Wallace L, Hollaus M, Wielgosz M, et al. FOR-instance: a UAV laser scanning benchmark dataset for semantic and instance segmentation of individual trees. arXiv; 2023. Available from: http://arxiv.org/abs/2309.01279.
[^28]: Allen MJ, Grieve SWD, Owen HJF, Lines ER. Tree species classification from complex laser scanning data in Mediterranean forests using deep learning. _Methods in Ecology and Evolution_. 2023;14(7):1657-67. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.13981.
[^29]: Calders K, Verbeeck H, Burt A, Origo N, Nightingale J, Malhi Y, et al. Laser scanning reveals potential underestimation of biomass carbon in temperate forest. _Ecological Solutions and Evidence_. 2022;3(4):e12197. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1002/2688-8319.12197.
[^30]: Hirschmugl M, Sobe C, Di Filippo A, Berger V, Kirchmeir H, Vandekerkhove K. Review on the Possibilities of Mapping Old-Growth Temperate Forests by Remote Sensing in Europe. _Environmental Modeling & Assessment_. 2023 Oct;28(5):761-85. Available from: https://doi.org/10.1007/s10666-023-09897-y.
[^31]: Trouvé R, Jiang R, Baker PJ, Kasel S, Nitschke CR. Identifying Old-Growth Forests in Complex Landscapes: A New LiDAR-Based Estimation Framework and Conservation Implications. _Remote Sensing_. 2024 Jan;16(1):147. Available from: https://www.mdpi.com/2072-4292/16/1/147.
[^32]: Sverdrup-Thygeson A, Ørka HO, Gobakken T, Næsset E. Can airborne laser scanning assist in mapping and monitoring natural forests? _Forest Ecology and Management_. 2016 Jun;369:116-25. Available from: https://www.sciencedirect.com/science/article/pii/S0378112716301128.
[^33]: Martin M, Valeria O. “Old” is not precise enough: Airborne laser scanning reveals age-related structural diversity within old-growth forests. _Remote Sensing of Environment_. 2022 Sep;278:113098. Available from: https://www.sciencedirect.com/science/article/pii/S0034425722002127.
[^34]: Fuhr M, Lalechère E, Monnet JM, Bergès L. Detecting overmature forests with airborne laser scanning (ALS). _Remote Sensing in Ecology and Conservation_. 2022 Oct;8(5):731-43. Available from: https://zslpublications.onlinelibrary.wiley.com/doi/10.1002/rse2.274.
[^35]: de Assis Barros L, Elkin C. An index for tracking old-growth value in disturbance-prone forest landscapes. _Ecological Indicators_. 2021 Feb;121:107175. Available from: https://www.sciencedirect.com/science/article/pii/S1470160X20311146.
[^36]: Hevia A, Calzado A, Alejano R, Vázquez-Piqué J. Identification of Old-Growth Mediterranean Forests Using Airborne Laser Scanning and Geostatistical Analysis. _Remote Sensing_. 2022 Jan;14(16):4040. Available from: https://www.mdpi.com/2072-4292/14/16/4040.
[^37]: Spracklen B, Spracklen DV. Determination of Structural Characteristics of Old-Growth Forest in Ukraine Using Spaceborne LiDAR. _Remote Sensing_. 2021 Jan;13(7):1233. Available from: https://www.mdpi.com/2072-4292/13/7/1233.
[^38]: Tech U. Lens - Upstream Tech; 2024. Available from: https://www.upstream.tech/lens.
[^39]: Vizzuality. About GFW | Global Forest Watch; 2024. Available from: https://www.globalforestwatch.org/about/.
[^40]: Palazón S. The Importance of Reintroducing Large Carnivores: The Brown Bear in the Pyrenees. In: Catalan J, Ninot JM, Aniz MM, editors. _High Mountain Conservation in a Changing World_. Cham: Springer International Publishing; 2017. p. 231-49. Available from: https://doi.org/10.1007/978-3-319-55982-7_10.
[^41]: Ratsakatika T. Real-time wildlife monitoring: Machine learning analysis of camera trap photos for an automated wildlife alert system in the Romanian Carpathian Mountains. University of Cambridge; 2024.
[^42]: Lines ER, Fischer FJ, Owen HJF, Jucker T. The shape of trees: Reimagining forest ecology in three dimensions with remote sensing. _Journal of Ecology_. 2022;110(8):1730-45. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1111/1365-2745.13944.
[^43]: Owen HJF, Flynn WRM, Lines ER. Competitive drivers of interspecific deviations of crown morphology from theoretical predictions measured with Terrestrial Laser Scanning. _Journal of Ecology_. 2021;109(7):2612-28. Available from: https://onlinelibrary.wiley.com/doi/abs/10.1111/1365-2745.13670.
[^44]: Wikimedia. Făgăraș Mountains in Romania; 2006. Available from: https://commons.wikimedia.org/wiki/File:Fagaras-mountains-Ro.jpg.
