# Network Steganography and Network Information Hiding

Version: 2.1.3

## Author
Prof. Dr. Steffen Wendzel, [website](https://www.wendzel.de)\
([Institute of Information Resource Management](https://www.uni-ulm.de/in/omi/), University of Ulm, Germany)

## How to Cite this Class?

Steffen Wendzel: *Network Steganography and Network Information Hiding* (online class), available online: [https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/), 2025.

## Introduction
This is an open online course on network information hiding and network steganography. The course contains video material and slides of a class that I teach at different universities. I updated the content over the years and will continue to do so.

Please note that quite some content of this class is based on the book W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016. If you are an IEEE member, you should be able to download the book for free.

[*YouTube Playlist for this Class*](https://www.youtube.com/watch?v=7YXXrbTah_s&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s)

[*List of my own Network Steganography Tools*](https://github.com/cdpxe/NetworkCovertChannels)


### Chapter 1 - Introduction to steganography and covert channels
This chapter provides an overview of the whole class. Afterwards, fundamental terminology, taxonomy and history of information hiding will be covered. The chapter also highlights some use-cases (legitimate and criminal ones) and tells you a bit about the CUING initiative.

- **Video:** [YouTube](https://www.youtube.com/watch?v=eDjlQbH_DTI&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=1)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch1.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks, **Chapters 1 and 2**](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016.

- **Optional Papers to Read:**
	- F. Petitcolas, R. Anderson, M. Kuhn: [Information Hiding – A Survey](https://ieeexplore.ieee.org/abstract/document/771065), Proc. IEEE, 87(7), 1999.
	- B. Pfitzmann: [Information Hiding Terminology](https://doi.org/10.1007/3-540-61996-8_52), Proc. 1st Information Hiding Workshop, Springer, 1996.
	- L. Caviglione: [Steg in the Wild](https://github.com/lucacav/steg-in-the-wild) (a list of attacks and malware using steganography or information hiding), Github repository.
	- F. Strachanski et al.: [A Comprehensive Pattern-based Overview of Stegomalware](https://doi.org/10.1145/3664476.3670886). In: Proc. 19th International Conference on Availability, Reliability and Security (ARES 2024). ACM, DOI: [https://doi.org/10.1145/3664476.3670886](https://doi.org/10.1145/3664476.3670886), 2024.

- **Exercise:**
	- Explain one historic method of steganography that was not explained during the lecture in a short talk in front of the other students.
	- Was there any terminological inconsistency regarding the terms *network covert channel* and *network steganography* in the introduced taxonomy? (Chapter 2 of W. Mazurczyk et al., 2016)
	- Different domains of steganography exist, including network steganography, digital media steganography, text steganography and cyber-physical systems steganography. Name typical cover objects for all four of them.
	- Would it beneficial to combine different types of wardens?

___


### Chapter 2 - Introduction to classic covert channels
First, simple methods for local (system-internal) covert channels are discussed. Second, covert channels between Docker containers and for Android are shown.

- **Video:** [YouTube](https://www.youtube.com/watch?v=iyEqschrN6g&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=2)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch2.pdf)

- **Reading Assignment:**
	- none for this chapter

- **Optional Papers to Read:**
	- W. Mazurczyk, L. Caviglione: [Steganography in Modern Smartphones and Mitigation Techniques](https://ieeexplore.ieee.org/abstract/document/6884798), IEEE Communications Surveys & Tutorials, Vol. 17(1), 2014.
	- J.-F. Lalande, S. Wendzel: [Hiding privacy leaks in Android applications using low-attention raising covert channels](https://ieeexplore.ieee.org/abstract/document/6657308/), Proc. 8th ARES, Regensburg, DE, IEEE, 2013.
	- C. Krätzer, J. Dittmann: [Steganography by synthesis: Can commonplace image manipulations like face morphing create plausible steganographic channels?](https://dl.acm.org/doi/10.1145/3230833.3233263), in Proc. 13th International Conference on Availability, Reliability and Security (ARES 2018), ACM, 2018.

- **Exercise:**
	- Low-attention raising covert channels (such as described in the paper by Lalande and Wendzel above) are usually linked to a small bitrate. Explain why such channels can be considered valuable especially in network environments.
	- Given the rising trend of censorship circumvention, why do you think is Information Hiding not applied by a large number of people? (And who does actually apply it?)
	- The above-mentioned paper by Krätzer et al. proposes a "modern (post 2010) steganographic communication setup". Why did the authors introduce this model? How does it differ from the classical *prisoner's problem* that was covered in Chapter 1?

___

### Chapter 3 - Fundamental countermeasures (not network-specific)
In this chapter, you will learn how covert channels can be detected, eliminated, and limited on the basis of exemplary countermeasures. These countermeasures can be applied at different states of a system's lifetime (design-phase to operation phase). In particular, I cover the Shared Resource Matrix (SRM) methodology, Covert Flow Trees (CFT), Fuzzy Time, and the Spurious Processes Approach.

- **Video:** [YouTube](https://www.youtube.com/watch?v=F5rMlC-tlRw&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=3)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch3.pdf)

- **Reading Assignment:**
	- R. Kemmerer, P. Porras: Covert Flow Trees: A Visual Approach to Analyzing Covert Storage Channels, Trans. Software Engineering, IEEE, 1991.

- **Optional Papers to Read:**
	- *in German:* I discuss SRM, extended SRM (Gypsy SRM), CFT, the Pump, and several other fundamental anti-covert channel concepts in my book S. Wendzel: *Tunnel und verdeckte Kanäle im Netz*, Springer, 2012 (**[Chapter 6](https://link.springer.com/chapter/10.1007/978-3-8348-2143-0_6)**).

- **Exercise:**
	- Which method would you apply to eliminate/spot covert channels in the following situations:
		- The company you are working for wishes to get a certificate (e.g. a high level of EAL) for their product; the certificate requires a code-level audit that lists all possible covert storage channels.
		- You plan to design a new product (not implemented in code). You need to perform a covert channel analysis using the product’s specification.
		- Your company plans to sell a product to a military customer. The customer requires a covert timing channel audit, which you performed. However, the customer will only accept covert channels with a channel capacity below 1 bit/s.
	- How could you create a policy-breaking covert channel during your exam in order to secretly exchange answers to exam questions?
		- Link this scenario to the Prisoner’s Problem.

___

### Chapter 4 - Fundamental network information hiding techniques
This chapter introduces basic methods for realizing network covert channels and their different types (active and passive covert channels, intentional and unintentional (side) channels, and direct and indirect covert channels).

- **Video:** [YouTube](https://www.youtube.com/watch?v=NQxwOo-ugh8&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=4)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch4.pdf) (PDF version newer than video!)

- **Reading Assignment:**
	- L. Caviglione, W. Mazurczyk: [Understanding Information Hiding in iOS](https://ieeexplore.ieee.org/abstract/document/7030266), IEEE Computer, Vol. 48(1), 2015.
	- T. Schmidbauer, S. Wendzel: [SoK: A Survey Of Indirect Network-level Covert Channels](https://dl.acm.org/doi/10.1145/3488932.3517418), in: ASIA CCS '22: Proceedings of the 2022 ACM on Asia Conference on Computer and Communications Security, ACM, 2022.
	- S. Wendzel, T. Schmidbauer, S. Zillien, J. Keller: [DYST (Did You See That?): An Amplified Covert Channel That Points To Previously Seen Data](https://doi.org/10.1109/TDSC.2024.3410679), IEEE Transactions on Dependable and Secure Computing (TDSC), Vol. 22(1), 2025.

- **Network Covert Channel Tools:**
	- [Source code of my network covert channel tools on GitHub](https://github.com/cdpxe/NetworkCovertChannels/) (phcct, pct, vstt, ...)

- **Exercise:**
	- In the paper of the reading assignment, you will find a steganographic method called *iStegSiri* for iOS published by Caviglione and Mazurczyk. Explain how it works! Also, [here](https://spectrum.ieee.org/tech-talk/telecom/security/malware-could-steal-data-from-iphones-using-siri) is a news article about iStegSiri.
	- Can Information Hiding methods be applied to deduce cryptographic keys from encryption/decryption tools? If yes: how?
___

### Chapter 5 - Getting the big picture: hiding patterns
In this chapter, so-called *hiding patterns* are introduced. Patterns are a universal tool that is popular in software engineering and other disciplines, even outside of informatics. Hiding patterns are an easy way to describe and understand how data can be hidden using network covert channels. Instead of studying hundreds of separate hiding techniques, one can simply grasp all their core ideas using hiding patterns.
The second part of this chapter introduces a revised version of the patterns taxonomy that is not specific to the network context. Instead, it can be applied to *all* domains of steganography. This revised model was introduced in 2025 and contains certain additional features, such as the distinction between *embedding* and *representation* patterns.

- **Video 1:** [YouTube](https://www.youtube.com/watch?v=PABu1HVXHvE&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=5) (OLD version)
- **Video 2:** [YouTube](https://www.youtube.com/watch?v=7MiMI5eUjMw) (NEW version)

- **Slides (network-specific taxonomy):** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch5.pdf)
- **Slides (generic taxonomy):** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch5_new_taxonomy_2025.pdf)

- **Reading Assignment:**
	- S. Wendzel, S. Zander, B. Fechner, C. Herdin: [Pattern-based survey and categorization of network covert channel techniques](https://doi.org/10.1145/2684195), ACM Computing Survey (CSUR), Vol. 47(3), ACM, 2015. ([pre-print on researchgate](https://www.researchgate.net/publication/263048788_Pattern-Based_Survey_and_Categorization_of_Network_Covert_Channel_Techniques))
	- S. Wendzel, L. Caviglione, W. Mazurczyk, A. Mileva, J. Dittmann, C. Krätzer, K. Lamshöft, C. Vielhauer, L. Hartmann, J. Keller, T. Neubert, S. Zillien: [A Generic Taxonomy for Steganography Methods](https://doi.org/10.1145/3729165), ACM Computing Survey (CSUR), 2025.
		- This paper is the 2025-revision of the patterns taxonomy.
		- Electronic supplement to that paper: [supplement PDF](https://dl.acm.org/doi/suppl/10.1145/3729165/suppl_file/csur-2022-0464-File002.pdf)

- **Exercise:**
	- Get an overview of the [CCEAP tool and its protocol](https://ih-patterns.blogspot.com/p/cceap.html). Work through the provided sample [exercises](https://github.com/cdpxe/CCEAP/tree/master/sample_exercises) and try to understand the provided solutions.
	- Why is it useful to differentiate between embedding and representation patterns?
	- Explain the partial backwards-compatibility to the network-specific patterns taxonomy.

___

### Chapter 6 - Staying under the radar: sophisticated hiding methods and distributed hiding patterns
This chapter covers distributed hiding methods, including pattern variation, pattern hopping, protocol switching (protocol channels, protocol hopping covert channels), dynamic overlay routing for covert channels, micro protocols (covert channel internal control protocols, including their optimization), reversible data hiding (RDH), and dead drops that exploit network caches.

- **Video:** [YouTube](https://www.youtube.com/watch?v=Ac-pJIGlzmg&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=6)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch6.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, P. Szary, S. Wendzel and L. Caviglione: [Towards Reversible Storage Network Covert Channels](https://doi.org/10.1145/3339252.3341493), in Proc. Third International Workshop on Criminal Use of Information Hiding (CUING 2019), pp. 69:1-69:8, ACM, 2019.
	- W. Mazurczyk, S. Wendzel, S. Zander et al.: [Information Hiding in Communication Networks, **Chapter 4**](https://ieeexplore.ieee.org/book/7434879), Wiley-IEEE, 2016.

- **Optional Papers to Read:**
	- Yarochkin, F. et al.: [Towards adaptive covert communication system](https://ieeexplore.ieee.org/abstract/document/4725291/), in Proc. 14th IEEE Pacific Rim International Symposium on Dependable Computing. IEEE, 2008.
	- S. Wendzel, J. Keller: [Hidden and Under Control](https://doi.org/10.1007/s12243-014-0423-x), Annals of Telecommunications (ANTE), Springer, 2014.
	- S. Wendzel, J. Keller: [Systematic Engineering of Control Protocols for Covert Channels](https://link.springer.com/chapter/10.1007/978-3-642-32805-3_11), in Proc. Communications & Multimedia Security (CMS), Springer, 2012.
	- C. Krätzer, J. Dittmann, A. Lang, T. Kühne: [WLAN steganography: a first practical review](https://doi.org/10.1145/1161366.1161371), in Proc. 8th Workshop on Multimedia and Security (MM&Sec), ACM, 2006.
	- S. Schmidt, W. Mazurczyk, R. Kulesza, J. Keller, C. Caviglione: [Exploiting IP telephony with silence suppression for hidden data transfers](https://www.sciencedirect.com/science/article/pii/S0167404818305777), Computers & Security, Vol. 79, 2018.
	- K. Szczypiorski, I. Margasiński, W. Mazurczyk, K. Cabaj, P. Radziszewski: [TrustMAS: Trusted communication platform for multi-agent  systems](https://link.springer.com/chapter/10.1007/978-3-540-88873-4_7), in Proc. OTM On the Move to Meaningful Internet Systems, Springer, 2008.

- **Exercise:**
	- Which pattern-based distributed hiding methods do protocol channels and protocol hopping covert channels belong to?
	- Is the micro protocol grammar shown in the slides a language-subset of the cover protocol language?
	- Have a look at the above-mentioned paper on by Schmidt et al.: How do the authors hide data in IP telephony traffic?
	- Why was it beneficial to [improve the NEL phase](https://dl.gi.de/handle/20.500.12116/18270)? Why does the original NEL phase suffer from a *Two-army Problem* and what is a Two-army Problem?
	- In the paper referenced above by Krätzer et al. you can read about a network steganography method for IEEE 802.11 (WLAN) networks. How does it work? Can you link the hiding approach to a particular pattern?
	- How do you think that distributed hiding methods could be detected or limited? (Will be answered in the next chapter.)
	- How did the paper [Covert Storage Caches using the NTP Protocol](https://dl.acm.org/doi/10.1145/3407023.3409207) advance over previous work that uses ARP (see reading assignment above)? Why is this useful for an attacker? What are the limitations of the NTP-based approach?

___

### Chapter 7 - Selected network-level countermeasures
Chapter 7 finally introduces methods to combat network covert channels. The chapter is separated into two parts. **Part A** covers selected basic methods, namely traffic normalization (preventing/limiting), three methods by Berk et al. and Cabuk et al. (detection of inter-packet times pattern), and finally, the so-called *countermeasure variation*. **Part B** introduces countermeasures that help limiting and detecting sophisticated network covert channels, namely the protocol switching covert channels and the NEL phase. These methods are the *protocol (switching covert) channel-aware active warden* (PCAW) and the *dynamic warden*.

- **Video:** [part A-1, YouTube](https://www.youtube.com/watch?v=DW8eT5NtoxE&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=7), [part A-2, YouTube](https://www.youtube.com/watch?v=57uVKD1X6-w&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=8) (extended content), [part B, YouTube](https://www.youtube.com/watch?v=v3AeSPAmF8Y&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=9)

- **Slides:** [part A, PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch7a.pdf), [part B, PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch7b.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, S. Wendzel, S. Zander et al.: [Information Hiding in Communication Networks, **Chapter 8**](https://ieeexplore.ieee.org/book/7434879), Wiley-IEEE, 2016.

- **Optional Papers to Read:**
	- Fundamental heuristics for network timing channel detection: S. Cabuk, C. E. Brodley, C. Shields: [IP covert channel detection](https://dl.acm.org/doi/abs/10.1145/1513601.1513604), Trans. Information and System Security (TISSEC) Vol. 12(4), ACM, 2009.
	- Details of the dynamic warden: W. Mazurczyk, S. Wendzel, M. Chourib, J. Keller: [Countering Adaptive Network Covert Communication with Dynamic Wardens](https://doi.org/10.1016/j.future.2018.12.047), Future Generation Computer Systems (FGCS), Vol. 94, pp. 712-725, Elsevier, 2019.
	- How popular covert channel countermeasures can be circumvented: S. Zillien, S. Wendzel: [Weaknesses of Popular and Recent Covert Channel Detection Methods and a Remedy](https://doi.org/10.1109/TDSC.2023.3241451), IEEE Trans. Dep. Secur. Comp. (TDSC), Vol. 20(6), 2023.

___

### Chapter 8 - Replicating experiments for scientific advancement
First, I briefly discuss why we need replication studies and which obstacles prevent the conduction of these studies. Second, I show one study that we conducted ourselves.

- **Video:** [YouTube](https://www.youtube.com/watch?v=hs_nPTwQXXA&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=10)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch8.pdf)

- **Optional Papers to Read:**
	- S. Wendzel, L. Caviglione, W. Mazurczyk, J.-F. Lalande: [Network Information Hiding and Science 2.0: Can it be a Match?](https://www.researchgate.net/publication/316215336_Network_Information_Hiding_and_Science_20_Can_it_be_a_Match), International Journal of Electronics and Telecommunications 63(2), 2017.

- **Exercise:**
	- Answer the following questions:
		- Why is it essential to replicate experiments?
		- What can scientists do to support experimental replications of their *own* work?
		- What is commonly referred to under the term *Open Science*?

___

### Chapter 9 - Describing Hiding Methods (+ Some Notes on Experimental Setups)
When a new hiding technique is found, how should it be described in a way that other authors can easily access it? How to ease replication studies? How to ease the process of finding out what still needs to be done? These questions can be answered with the *unified description method* for information hiding techniques explained in this chapter. Moreover do I introduce the *creativity* approach that helps to decide about the novelty of a research contribution. Finally, I cover a traditionall paper by V. Paxson on Measurement Studies as these are important in covert channel reseach (and Internet censorship (circumvention) research). *This chapter is work in progress and will (hopefully) feature more content on experimental setups in the future.*

- **Video:** [YouTube](https://www.youtube.com/watch?v=viieBAdAQh0&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=11) (old version)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch9.pdf) (new version of Jun-2025, taken from my class on Internet censorship)

- **Reading Assignment:**
	- S. Wendzel, C. Krätzer, J. Dittmann, L. Caviglione, A. Mileva, T. Schmidbauer, C. Vielhauer, S. Zander: *[Describing Steganography Hiding Methods by Combining Pre-Existing Methodology](https://arxiv.org/abs/2506.01700)*. In: Proc. 20th International Conference on Availability, Reliability and Security (ARES 2025 Workshops (CUING Workshop)).
   	- **Revised version** of the unified description method that has been adjusted to the 2025-taxonomy: [download (PDF, see Sect. A.6)](https://dl.acm.org/doi/suppl/10.1145/3729165/suppl_file/csur-2022-0464-File002.pdf) (electronic supplement of [this](https://dl.acm.org/doi/10.1145/3729165) paper)
   	- V. Paxson: *[Strategies for Sound Internet Measurement](https://dl.acm.org/doi/10.1145/1028788.1028824)*, Proc. IMC, 2004.


- **Exercise:**
	- Why is it important to consider Paxson's strategies when conducting network-based measurements? How do his observations apply to network covert channel research? How do they apply to Internet censorship (circumvention) research?
 	- Read the above-mentioned paper on the unified description method and answer the following questions:
		- What is the difference between the two attributes *required properties of the carrier* and *covert channel properties*?
		- Why is the attribute on *control protocols* not mandatory in the unified description method?
		- How does the *creativity metric* work jointly with the unified description method?

___

### Chapter 10 - *My smart fridge does strange things …* a.k.a. steganography in the Internet of Things (IoT)
In the Internet of Things (and Cyber-physical Systems, CPS), data can either be hidden within network communications (e.g. in IoT protocols) *or* in can be hidden the CPS *components* (e.g. unused registers or states of actuators). I will discuss these methods as well as scenarios in this conference talk below. However, please note that the PDF files contain an extended scenario. I plan to update the PDF slides in the coming years as there is still quite a lot to say about this chapter.

- **Video:** [part A, YouTube](https://www.youtube.com/watch?v=P9XYV4mcPV0&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=12), [part B, YouTube](https://www.youtube.com/watch?v=Q7eAcBzojvo&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=13). Part B is the video of the talk S. Wendzel, G. Haas, W. Mazurczyk: *Information Hiding in Cyber-physical Systems*, presented during the 2nd Int. BioSTAR workshop in late May, 2017 (IEEE Security & Privacy Workshops, San José, CA)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch10.pdf)

- **Reading Assignment:**
	- S. Wendzel, W. Mazurczyk, G. Haas: [Steganography for Cyber-physical Systems](http://www.riverpublishers.com/journaldownload.php?file=RP_Journal_2245-1439_621.pdf), Journal of Cyber Security and Mobility (JCSM), Vol. 6(2), pp. 105-126, River Publishers, 2017.
	- A. Velinov, A. Mileva, S. Wendzel, W. Mazurczyk: [Covert Channels in the MQTT-Based Internet of Things](https://ieeexplore.ieee.org/document/8890870/), IEEE ACCESS, 2019.
	- A Mileva, A Velinov, D Stojanov: [New covert channels in Internet of Things](http://eprints.ugd.edu.mk/20423/1/securware_2018_2_10_30122.pdf), in Proc. Securware 2018.

- **Exercise:**
	- What is the difference between an intentional covert channel and an intentional side channel in a CPS? Can you name a few examples? Both terms of CPS Steganography are introduced in [this paper](https://www.researchgate.net/publication/229092563_Covert_and_Side_Channels_in_Buildings_and_the_Prototype_of_a_Building-aware_Active_Warden/link/00b495349285c92bbd000000/download). What was the solution proposed by this paper to combat both types of channels?
	- In [this paper](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6468400&tag=1), I describe how an MLS-based filtering can prevent covert and side channels in CPS network communications (exemplified using smart buildings). How does this work? What are limitations?

___

### Chapter 11 - Summary and overall conclusion
This chapter summarizes what we have learned in the ten previous chapters. I also highlight open research problems that might support you in finding topics for a Master or even a PhD thesis.

- **Video:** [YouTube](https://www.youtube.com/watch?v=pXo3mdmR_yM&list=PLlCWln7xuottidcUEsfqhXeV9fhIbkJ4s&index=14)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch11.pdf)

- **Reading Assignment:** none

- **Exercise:**
Congratulations, you made it through the whole class! **Now it is time for the final (big!) exercise!** Try to find a new network protocol for which there is absolutely no work available that analyzes covert channels in this protocol (use [Google Scholar](https://scholar.google.com) or any other paper search engine to find such works). Next, analyze the protocol regarding all known hiding patterns and describe all covert channels that you found using the unified description method. If you like, submit your paper to a conference (or: let me know and I can potentially link the paper at least here).

___

### Changelog

- v. 2.1.3, 2025-Jun-12
    - replace Ch 9 PDF with new version from my class on Internet censorship

- v. 2.1.2, 2025-Jun-11
    - point to new tutorial paper on the description of hiding methods

- v. 2.1.1, 2025-Apr-29
    - removed outdated exercises
    - revised UDM section

- v. 2.1.0, 2025-Apr-17
    - added content for the 2025 generic steganography taxonomy

- v. 2.0.12, 2025-Apr-08
    - replaced pre-print of generic taxonomy paper with the Comp. Surv. DOI

- v. 2.0.11-b, 2025-Jan-20
    - added vol.+no. for TDSC paper

- v. 2.0.11, 2024-Oct-15
    - editorial changes in the README.md, replacing HS Worms w/ Uni Ulm

- v. 2.0.10, 2024-Sep-05
    - added citation info and adjusted title in README.md to title in the slides

- v. 2.0.9, 2024-Aug-21
    - added reference to Strachanski et al. in chapter 1
    - updated reference to DYST paper in chapter 4 (replaced pre-print with official TDSC paper)
    - remove nefias (out of date, not updated anymore)
    - update publications list for Ch. 8.

- v. 2.0.7, 2024-Jun-24
    - tiny link update for DYST paper (TDSC)

- v. 2.0.6, 2024-May-08
    - tiny link updates

- v. 2.0.5 (no new version), 2023-Aug-14
    - modified schedule for HSW M.Sc. class

- v. 2.0.5, 2023-Jan-04 (only slide updates; videos remain as is):
   - Updated Ch. 4: added "history covert channels" and "fully-passive covert channels".

- v. 2.0.4, 2022-Sep-16 (only slide updates; videos remain as is):
   - Updated Ch. 1: added reference to new paper by Luca Caviglione (@lucacav) and Wojciech Mazurczyk on stego-malware.

EOF
