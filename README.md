# Network Information Hiding 101: Terminology, Methodology of Network Steganography / Network Covert Channels

### Prof. Dr. Steffen Wendzel, [website](https://www.wendzel.de)
Worms University of Applied Sciences, contact: wendzel (at) hs-worms (dot) de

## Introduction
This is a open online course for network covert channels. The course contains video material and slides that I use in my undergraduate and graduate courses at Worms University of Applied Sciences, Germany. (I recorded the videos anyway, so why shouldn't I make them public.) I also used the slides at other universities, summer schools etc. over the years.

*Note:* More material will be added. You can always find the latest version of my slides here, as I updated these slides over the years and will continue to do so. Feel free to use my slides in your own class.

I made sure that references are using links so that you and your students can get easier access to the publications.

Please note that most content of this class is based on the book W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016. If you are an IEEE member, you should be able to download the book for free.

## Outline

*This online class **starts on May 5th, 2020 but all content will remain online on Github for those who want to start later (or in a few years)**. I will upload videos once in a week.* Please note that some weeks contain multiple videos:


| Week      | 1 | 2 | 3 | 4 | 5 | 6 | 7 |...|...|... |
|-----------|---|---|---|---|---|---|---|---|---|----|
| Chapter 1 | X *N,M* |   |   |   |   |   |   |   |   |    |
| Chapter 2 |   | X *M* |   |   |   |   |   |   |   |    |
| Chapter 3 |   | X *M* |   |   |   |   |   |   |   |    |
| Chapter 4 |   |   | X *N,M* |   |   |   |   |   |   |    |
| Chapter 5 |   |   | X *N,M*|   |   |   |   |   |   |    |
| Chapter 6 |   |   |   | X *M* |   |   |   |   |   |    |
| Chapter 7 |   |   |   |   | X *N,M* |   |   |   |   |    |
| Chapter 8 |   |   |   |   |   | X |   |   |   |    |
| Chapter 9 |   |   |   |   |   | X |   |   |   |    |
| Chapter 10|   |   |   |   |   |   | X |   |   |    |
| Chapter 11|   |   |   |   |   |   | X |   |   |    |

- *N*: relevant for *Network Security* class (B.Sc. level)
- *M*: relevant for *Mobile Security* class (M.Sc. level)

### Week 1: Chapter 1 - Introduction to Steganography and Covert Channels (May 5th, 2020)
This chapter provides an overview of the whole class. Afterwards, fundamental terminology, taxonomy and history of information hiding will be covered. The chapter also highlights some use-cases (legitimate and criminal ones) and tells you a bit about the CUING initiative.

- **Video:** [YouTube](https://www.youtube.com/watch?v=7YXXrbTah_s)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch1.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks, **Chapters 1 and 2**](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016.

- **Optional Papers to Read:**
	- F. Petitcolas, R. Anderson, M. Kuhn: [Information Hiding – A Survey](https://ieeexplore.ieee.org/abstract/document/771065), Proc. IEEE, 87(7), 1999.
	- B. Pfitzmann: [Information Hiding Terminology](https://doi.org/10.1007/3-540-61996-8_52), Proc. 1st Information Hiding Workshop, Springer, 1996.
	- E. Zielinska, W. Mazurczyk, K. Szczypiorski: [Trends in Steganography](https://dl.acm.org/doi/10.1145/2566590.2566610), Comm. ACM, 2014.
	-  K. Cabaj, L. Caviglione, W. Mazurczyk, S. Wendzel, A. Woodward, S. Zander: [The New Threats of Information Hiding: the Road Ahead](https://ieeexplore.ieee.org/document/8378979/), IT Professional, IEEE, 2018.
	- L. Caviglione: [Steg in the Wild](https://github.com/lucacav/steg-in-the-wild) (A list of attacks and malware using steganography or information hiding), Github repository.

- **Exercise:**
	- Explain one historic method of steganography that was not explained during the lecture in a short talk in front of the other students.
	- Is there a terminological inconsistency for the terms covert channel, network covert channel, steganography and network steganography given the introduced taxonomy? If yes: explain. (Chapter 2 of W. Mazurczyk et al., 2016)
	- Can Information Hiding methods be applied to deduce cryptography keys from encryption/decryption tools? If yes: how?
___


### Week 2-a: Chapter 2 - Introduction to classic covert channels (May 12th, 2020)
First, simple methods for local (system-internal) covert channels are discussed. Second, covert channels between Docker containers and for Android are shown.

- **Video:** [YouTube](https://youtu.be/MBV-NFQLH34)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch2.pdf)

- **Reading Assignment:**
	- none for this chapter

- **Optional Papers to Read:**
	- W. Mazurczyk, L. Caviglione: [Steganography in Modern Smartphones and Mitigation Techniques](https://ieeexplore.ieee.org/abstract/document/6884798), IEEE Communications Surveys & Tutorials, Vol. 17(1), 2014.
	- J.-F. Lalande, S. Wendzel: [Hiding privacy leaks in Android applications using low-attention raising covert channels](https://ieeexplore.ieee.org/abstract/document/6657308/), Proc. 8th ARES, Regensburg, DE, IEEE, 2013.

- **Exercise:**
	- Low-attention raising covert channels (such as described in the paper by Lalande and Wendzel above) are usually linked to a small bitrate. Explain why such channels can be considered valuable especially in network environments.
	- Given the rising trend of censorship circumvention, why do you think is Information Hiding not applied by a large number of people? (And who does actually apply it?)

___

### Week 2-b: Chapter 3 - Fundamental countermeasures (not network-specific) (May 12th, 2020)
In this chapter, you will learn how covert channels can be detected, eliminated, and limited on the basis of exemplary countermeasures. These countermeasures can be applied at different states of a system's lifetime (design-phase to operation phase). In particular, I cover the Shared Resource Matrix (SRM) methodology, Covert Flow Trees (CFT), Fuzzy Time, and the Spurious Processes Approach.

- **Video:** [YouTube](https://youtu.be/6cjsPzLscd8)

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

### Week 3-a: Chapter 4 - Fundamental network information hiding techniques (May 19th, 2020)
This chapter introduces basic methods for realizing network covert channels and their different types, in particular active and passive covert channels, intentional and unintentional (side) channels, and direct and indirect covert channels.

- **Video:** [YouTube](https://www.youtube.com/watch?v=29s696QwHVM)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch4.pdf)

- **Reading Assignment:**
	- L. Caviglione, W. Mazurczyk: [Understanding Information Hiding in iOS](https://ieeexplore.ieee.org/abstract/document/7030266), IEEE Computer, Vol. 48(1), 2015.

- **Exercise:**
	- In the paper of the reading asignment, you will find a steganographic method called *iStegSiri* for iOS published by Caviglione and Mazurczyk. Explain how it works! Also, [here](https://spectrum.ieee.org/tech-talk/telecom/security/malware-could-steal-data-from-iphones-using-siri) is a news article about iStegSiri.

___

### Week 3-b: Chapter 5 - Getting the big picture: hiding patterns (May 19th, 2020)
In this chapter, so-called *hiding patterns* are introduced. Patterns are an universal tool that is popular in software engineering and other disciplines, even outside of informatics. Hiding patterns are an easy way to describe and understand how data can be hidden using network covert channels. Instead of studying hundreds of separate hiding techniques, one can simply grasp all their core ideas using hiding patterns.

- **Video:** [YouTube](https://www.youtube.com/watch?v=0ztPHur0LUY)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch5.pdf)

- **Reading Assignment:**
	- S. Wendzel, S. Zander, B. Fechner, C. Herdin: [Pattern-based survey and categorization of network covert channel techniques](https://doi.org/10.1145/2684195), ACM Computing Survey (CSUR), Vol. 47(3), ACM, 2015.
	- W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks, **Chapter 3**](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016.

- **Optional Papers to Read:**
	- W. Mazurczyk, S. Wendzel, K. Cabaj: [Towards Deriving Insights into Data Hiding Methods Using Pattern-based Approach](https://doi.org/10.1145/3230833.3233261), in Proc. ARES, ACM, 2018.

- **Exercise:**
	- Get an overview of the [CCEAP tool and its protocol](https://ih-patterns.blogspot.com/p/cceap.html). Work through the provided sample [exercises](https://github.com/cdpxe/CCEAP/tree/master/sample_exercises) and try to understand the provided solutions.

___

### Week 4: Chapter 6 - Staying under the radar: sophisticated hiding methods and distributed hiding patterns (May 26th, 2020)
This chapter covers distributed hiding methods, including pattern variation, pattern hopping, protocol switching (protocol channels, protocol hopping covert channels), dynamic overlay routing for covert channels, micro protocols (covert channel internal control protocols, including their optimization), reversible data hiding (RDH), and dead drops that exploit network caches.

- **Video:** [YouTube](https://www.youtube.com/watch?v=YicdOu10FmE)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch6.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, P. Szary, S. Wendzel and L. Caviglione: [Towards Reversible Storage Network Covert Channels](https://doi.org/10.1145/3339252.3341493), in Proc. Third International Workshop on Criminal Use of Information Hiding (CUING 2019), pp. 69:1-69:8, ACM, 2019.
	- W. Mazurczyk, S. Wendzel, S. Zander et al.: [Information Hiding in Communication Networks, **Chapter 4**](https://ieeexplore.ieee.org/book/7434879), Wiley-IEEE, 2016.

- **Optional Papers to Read:**
	- Yarochkin, F. et al.: [Towards adaptive covert communication system](https://ieeexplore.ieee.org/abstract/document/4725291/), in Proc. 14th IEEE Pacific Rim International Symposium on Dependable Computing. IEEE, 2008.
	- S. Wendzel, J. Keller: [Hidden and UnderControl](https://doi.org/10.1007/s12243-014-0423-x), Annals of Telecommunications (ANTE), Springer, 2014.
	- S. Wendzel, J. Keller: [Systematic Engineering of Control Protocols for Covert Channels](https://link.springer.com/chapter/10.1007/978-3-642-32805-3_11), in Proc. Communications & Multimedia Security (CMS), Springer, 2012.
	- C. Krätzer, J. Dittmann, A. Lang, T. Kühne: [WLAN steganography: a first practical review](https://doi.org/10.1145/1161366.1161371), in Proc. 8th Workshop on Multimedia and Security (MM&Sec), ACM, 2006.
	- S. Schmidt, W. Mazurczyk, R. Kulesza, J. Keller, C. Caviglione: [Exploiting IP telephony with silence suppression for hidden data transfers](https://www.sciencedirect.com/science/article/pii/S0167404818305777), Computers & Security, Vol. 79, 2018.
	- Szczypiorski, K., Margasiński, I., Mazurczyk, W., Cabajetal.: [TrustMAS: Trusted communication platform for multi-agent  systems](https://link.springer.com/chapter/10.1007/978-3-540-88873-4_7), in Proc. OTM On the Move to Meaningful Internet Systems, Springer, 2008.

- **Exercise:**
	- Which pattern-based distributed hiding methods do protocol channels and protocol hopping covert channels belong to?
	- Is the micro protocol grammar shown in the slides a language-subset of the cover protocol language?
	- Have a look at the above-mentioned paper on by Schmidt et al.: How do the authors hide data in IP telephony traffic?
	- Why was it beneficial to [improve the NEL phase](https://dl.gi.de/handle/20.500.12116/18270)? Why does the original NEL phase suffer from a *Two-army Problem* and what is a Two-army Problem?
	- In the paper referenced above by Krätzer et al. you can read about a network steganography method for IEEE 802.11 (WLAN) networks. How does it work? Can you link the hiding approach to a particular pattern?
	- How do you think that distributed hiding methods could be detected or limited? (Will be answered in the next chapter.)

___

### Week 5: Chapter 7 - Selected network-level countermeasures (June 2nd, 2020)
Abstract t.b.d.

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:**
	- todo: Cabuk et al. ...
	- todo: Fadlalla et al. ...
	- todo: Zillien et al. ...
	- todo: Mazurcyk, Keller et al.: dynamic warden ...

- **Exercise:** t.b.d.

___

### Week 6-a: Chapter 8 - Replicating experiments for scientific advancement (June 9th, 2020)
Abstract t.b.d.

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:**
	- todo: Keidel et al. ...

- **Exercise:** t.b.d.

___

### Week 6-b: Chapter 9 - *OMG! I found a new hiding method. How do I become famous?!1!* a.k.a. How to describe a new hiding method in a paper? (June 9th, 2020)
Abstract t.b.d.

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### Week 7-a: Chapter 10 - *My smart fridge does strange things …* a.k.a. Steganography in the Internet of Things (IoT) (June 16th, 2020)
Abstract t.b.d.

- **Video:** [YouTube video](https://www.youtube.com/watch?v=Q7eAcBzojvo) of Wendzel, G. Haas, W. Mazurczyk: *Information Hiding in Cyber-physical Systems*, presented during the 2nd Int. BioSTAR workshop in late May, 2017 (IEEE Security & Privacy Workshops, San José, CA)

- **Slides:** t.b.d.

- **Reading Assignment:**
	- Steffen Wendzel, Wojciech Mazurczyk, Georg Haas: [Steganography for Cyber-physical Systems](http://www.riverpublishers.com/journaldownload.php?file=RP_Journal_2245-1439_621.pdf), Journal of Cyber Security and Mobility (JCSM), Vol. 6(2), pp. 105-126, River Publishers, 2017.
	- Aleksandar Velinov, Aleksandra Mileva, Steffen Wendzel, Wojciech Mazurczyk: [Covert Channels in the MQTT-Based Internet of Things](https://ieeexplore.ieee.org/document/8890870/), IEEE ACCESS, 2019.
	- A Mileva, A Velinov, D Stojanov: [New covert channels in Internet of Things](http://eprints.ugd.edu.mk/20423/1/securware_2018_2_10_30122.pdf), in Proc. Securware 2018.

- **Exercise:** t.b.d.

___

### Week 7-b: Chapter 11 - Summary and Overall conclusion (June 16th, 2020)
This chapter summarizes what we have learned in the ten previous chapters.

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### *maybe*: Week 8. Extension (e.g. lectures by invited experts)

If someone likes to contribute own lectures, then I am happy to link them here (e.g. your YouTube videos and slides). E.g. on VoIP stego, reversible stego, history of stego, ...
