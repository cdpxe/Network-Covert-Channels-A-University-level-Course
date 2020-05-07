# Network Information Hiding 101: Terminology, Methodology of Network Steganography / Network Covert Channels

### Prof. Dr. Steffen Wendzel, [website](https://www.wendzel.de)
Worms University of Applied Sciences, contact: wendzel (at) hs-worms (dot) de

## Introduction
This is a open online course for network covert channels. The course contains video material and slides that I use in my undergraduate and graduate courses at Worms University of Applied Sciences, Germany. (I recorded the videos anyway, so why shouldn't I make them public.) I also used the slides at other universities, summer schools etc. over the years.

*Note:* More material will be added. You can always find the latest version of my slides here, as I updated these slides over the years and will continue to do so. Feel free to use my slides in your own class.

I made sure that references are using links so that you and your students can get easier access to the publications.

## Outline

*This online class **starts on May 5th, 2020**. I will upload videos once in a week.* Please note that some weeks contain multiple videos:


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
| Chapter 10|   |   |   |   |   |   | X *M* |   |   |    |
| Chapter 11|   |   |   |   |   |   | X *M* |   |   |    |

- *N*: relevant for *Network Security* class (B.Sc. level)
- *M*: relevant for *Mobile Security* class (M.Sc. level)

### Week 1: Chapter 1 - Introduction to Steganography and Covert Channels (May 5th, 2020)

- **Video:** [YouTube](https://www.youtube.com/watch?v=7YXXrbTah_s)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch1.pdf)

- **Reading Assignment:**
	- W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks, Chapters 1 and 2](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016.

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

- **Video:** [YouTube](https://youtu.be/6cjsPzLscd8)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch3.pdf)

- **Reading Assignment:**
	- R. Kemmerer, P. Porras: Covert Flow Trees: A Visual Approach to Analyzing Covert Storage Channels, Trans. Software Engineering, IEEE, 1991.

- **Optional Papers to Read:**
	- *in German:* I discuss SRM, extended SRM (Gypsy SRM), CFT, the Pump, and several other fundamental anti-covert channel concepts in my book S. Wendzel: *Tunnel und verdeckte Kanäle im Netz*, Springer, 2012 ([Chapter 6](https://link.springer.com/chapter/10.1007/978-3-8348-2143-0_6)).

- **Exercise:**
	- Which method would you apply to eliminate/spot covert channels in the following situations:
		- The company you are working for wishes to get a certificate (e.g. a high level of EAL) for their product; the certificate requires a code-level audit that lists all possible covert storage channels.
		- You plan to design a new product (not implemented in code). You need to perform a covert channel analysis using the product’s specification.
		- Your company plans to sell a product to a military customer. The customer requires a covert timing channel audit, which you performed. However, the customer will only accept covert channels with a channel capacity below 1 bit/s.
	- How could you create a policy-breaking covert channel during your exam in order to secretly exchange answers to exam questions?
		- Link this scenario to the Prisoner’s Problem.


___

### Week 3-a: Chapter 4 - Fundamental network information hiding techniques (May 19th, 2020)

- **Video:** [YouTube](https://www.youtube.com/watch?v=29s696QwHVM)

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch4.pdf)

- **Reading Assignment:**
	- L. Caviglione, W. Mazurczyk: [Understanding Information Hiding in iOS](https://ieeexplore.ieee.org/abstract/document/7030266), IEEE Computer, Vol. 48(1), 2015.

- **Exercise:**
	- In the paper of the reading asignment, you will find a steganographic method called *iStegSiri* for iOS published by Caviglione and Mazurczyk. Explain how it works! Also, [here](https://spectrum.ieee.org/tech-talk/telecom/security/malware-could-steal-data-from-iphones-using-siri) is a news article about iStegSiri.

___

### Week 3-b: Chapter 5 - Getting the big picture: hiding patterns (May 19th, 2020)

- **Video:** t.b.d.

- **Slides:** [PDF](https://github.com/cdpxe/Network-Covert-Channels-A-University-level-Course/blob/master/slides/NIH_Ch5.pdf)

- **Reading Assignment:**
	- S. Wendzel, S. Zander, B. Fechner, C. Herdin: [Pattern-based survey and categorization of network covert channel techniques](https://doi.org/10.1145/2684195), ACM Computing Survey (CSUR), Vol. 47(3), ACM, 2015.
	- W. Mazurczyk, S. Wendzel, S. Zander, A. Houmansadr, K. Szczypiorski: [Information Hiding in Communication Networks, Chapter 3](https://ieeexplore.ieee.org/book/7434879), WILEY-IEEE, 2016.

- **Optional Papers to Read:**
	- W. Mazurczyk, S. Wendzel, K. Cabaj: [Towards Deriving Insights into Data Hiding Methods Using Pattern-based Approach](https://doi.org/10.1145/3230833.3233261), in Proc. ARES, ACM, 2018.

- **Exercise:**
	- Get an overview of the [CCEAP tool and its protocol](https://ih-patterns.blogspot.com/p/cceap.html). Work through the [exercises](https://github.com/cdpxe/CCEAP/tree/master/sample_exercises) and make sure you understand the provided solutions.

___

### Week 4: Chapter 6 - Staying under the radar: sophisticated hiding methods and distributed hiding patterns (May 26th, 2020)

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### Week 5: Chapter 7 - Selected network-level countermeasures (June 2nd, 2020)

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### Week 6-a: Chapter 8 - Replicating experiments for scientific advancement (June 9th, 2020)

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### Week 6-b: Chapter 9 - *OMG! I found a new hiding method. How do I become famous?!1!* a.k.a. How to describe a new hiding method in a paper? (June 9th, 2020)

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### Week 7-a: Chapter 10 - *My smart fridge does strange things …* a.k.a. Steganography in the Internet of Things (IoT) (June 16th, 2020)

- **Video:** [YouTube video](https://www.youtube.com/watch?v=Q7eAcBzojvo) of Wendzel, G. Haas, W. Mazurczyk: *Information Hiding in Cyber-physical Systems*, presented during the 2nd Int. BioSTAR workshop in late May, 2017 (IEEE Security & Privacy Workshops, San José, CA)

- **Slides:** t.b.d.

- **Reading Assignment:** Steffen Wendzel, Wojciech Mazurczyk, Georg Haas: [Steganography for Cyber-physical Systems](http://www.riverpublishers.com/journaldownload.php?file=RP_Journal_2245-1439_621.pdf), Journal of Cyber Security and Mobility (JCSM), Vol. 6(2), pp. 105-126, River Publishers, 2017.

- **Exercise:** t.b.d.

___

### Week 7-b: Chapter 11 - Summary and Overall conclusion (June 16th, 2020)

- **Video:** t.b.d.

- **Slides:** t.b.d.

- **Reading Assignment:** t.b.d.

- **Exercise:** t.b.d.

___

### *maybe*: Week 8. Extension (e.g. lectures by invited experts)

If someone likes to contribute own lectures, then I am happy to link them here (e.g. your YouTube videos and slides). E.g. on VoIP stego, reversible stego, history of stego, ...

___

## TODO

- convert all publication's links to DOI
