# Nothing Is Implied: Legal Loopholes in Popular Open Source Licenses
Miles McCain

_Draft paper; please do not cite without author's permission._

_For case subsections, all factual information is drawn directly from the case proceedings. No secondary sources are referenced._

## Abstract
In the United States, many legal mechanisms are in place that control and affect the distribution of computer software, including patents, copyright, liability, and trademark. The open source community uses a variety of licenses to allow the public to use its software freely. This survey of open source law finds that many of these licenses only explicitly address a small portion of these legal mechanisms, leaving the software's licensing ambiguous and subject to potential restriction. GPLv3 and the Apache 2.0 license are found to be the most secure and unambiguous licenses, while the MIT license and GPLv2 are found to leave important legal mechanisms governing open source software unaddressed.

## Introduction

TODO

## Patent Law

### Overview of Patent Law

Patents allow for ideas—user interfaces, API design patterns, and algorithms—to be owned and protected independent of their technical implementation. First defined in the United States Constitution (Art. I § 8.8), patents are an integral part of intellectual property law. They provide inventors with a temporary monopoly—typically twenty years—to their idea, during which no one else may use the idea without explicit permission from the patent holder. If a patent is infringed, the patent holder may sue for patent infringement and request that the infringer cease their use of the patented idea.

Patent law was first designed in a world without software. The framers of the Constitution could not possibly have imagined today's digital world, and this disconnect is visible when assessing software patent case law. In the early 1970's, when the first software patent court cases arose, it was unclear whether software was even eligible for patent. Since then, various cases have concretely extended patent law to the digital world.

Today, it is affirmed that patent law is applicable to software (Enfish LLC v. Microsoft, Inc. and DDR Holdings, LLC v. Hotels.com, L.P.). Because patent infringement can lead to both a fine and a legal order to cease use of the patented material, open source licenses must explicitly address patents to ensure that licensed software remains available for free use. In order to understand how software licenses can address patents, however, it is necessary to first understand the legal precedents regarding software patents themselves.

### Software Patent Case Law

#### Gottschalk v. Benson (1972)

In 1972, inventor Gary Benson sued for patent infringement for unauthorized use of an algorithm he had patented: the process by which numbers in decimal notation could be transformed into binary notation. Benson claimed that all uses of his algorithm—be they automated by a computer or performed by hand—were subject to his patent. Calling the patented algorithm nothing more than a "law of nature," the court ruled against Benson and declared the patent invalid. Benson appealed, and eventually the case appeared before the Supreme Court. (Gottschalk v. Benson, 409 U.S. 63.)

There was little precedent at the time as to whether an algorithm could be patented. In 1939 it was ruled that mathematical expressions could not be patented (Mackay Co. v. Radio Corp., 306 U.S. 86), however Benson argued that his patent was not an _equation_ but rather a _process_—a particular way of solving an equation, so to speak. The distinction was lost on the Supreme Court justices, however, and they upheld the lower court's decision. Algorithms, they ruled, could not be patented. (Gottschalk v. Benson, 409 U.S. 63.)

The significance of this decision could not have been anticipated in 1972. Computers had yet to revolutionize the world, and many of the intricacies of modern programming had not been invented. As computers began to occupy increasingly important roles in the world of business, however, companies began to worry whether their software—which was, after all, just a collection of algorithms—was patentable.

> The precedent set by Benson was unclear. Was _any_ computer program ineligible for patent? Was any process that even _used_ a computer ineligible?

> See also: Parker v. Flook (1978)

#### Diamond v. Diehr (1981)
A patent to the "[process] for molding raw, uncured synthetic rubber into cured precision products" using a machine was filed by James Diehr in 1975. Part of the patent was the use of a mathematical equation—the Arrhenius equation—solved by a computer. Unlike Benson, Diehr was not patenting the computer or program itself—instead, he claimed only that collective system was his patent. Initial reviewers of the patent were sufficiently convinced of Diehr's eligibility, and the filing raised few eyebrows—until a later patent examiner argued that the use of a mathematical equation run by a computer made the _entire process_ ineligible for patent under the Benson ruling.

> _Is a machine that uses a computer to transform physical materials patentable?_

The case made its way to the Surpreme Court. If the justices decided in favor of the examiner, any patent that made use of a mathematical equation—even if only as part of a subprocess—would be ineligible for protection. If the justices filed in favor of Diehr, computer manufacturers would rejoyce, now secure in their ability to patent their products containing computer.

In a 5 to 4 decision, the court deciced that the process _was_ patentable. The court was careful not to overrule Benson, and explained that so long as the patent was not itself a 'law of nature' and some physical change occurs, a process or machine is patentable.

This decision did not entirely secure the future of software patents—today's computers, after all, do not always create physical changes—but it was a vital case that affirmed the patentability of _some_ software.

#### Arrhythmia Research Technology, Inc. v. Corazonix Corporation (1992)
Following Diehr in 1981, processes that used a computer as a part of some larger process were patentable. As computers became increasingly capable and prevalent over the following decade, however, not all uses of computers resulted in some physical process. Corazonix Corporation, for example, created a computer device that processed electrocardiographic signals to analyze heart function. At the time of filing, there existed no strong precedent as to whether a use-case of a computer was patentable. Arrhythmia Research Technology, a Corazonix competitor, believed that it wasn't.

Importantly, Corazonix did not patent one particular implementation of a electrocardiographic signal processing computer. (Actual software implementations—the source code and object code itself—is firmly protected under copyright.) Instead, Corazonix patented the machine itself—as interpreted, a particular _use case_ of a computer.

Arrhythmia Research Technology, Inc. v. Corazonix Corporation was the first major case in which the software patent in question did not result in some physical change. If the court ruled in favor of Corazonix, the patentability of software would be affirmed. If the court ruled in favor of Arrhythmia Research Technology, computer use cases would be ineligible for patent.

The court ruled in favor of Corazonix and affirmed the eligibility of software for patent.

#### Alice v. CLS Bank 573 U.S., 134 S. Ct. 2347 (2014)
Arrhythmia was the law of the land for nearly twenty two years before the patentability of software was clarified. Following Diamond v. Diehr and Arrhythmia v. Corazonix, the decision of Benson—that trivial algorithms or computer algorithms that are laws of nature—was largely forgotten. _[citation needed]_ Vague and abstract software patents were filed and approved—perhaps most notably, a patent by CLS Bank to an electronic escrow service.

The high-profile case eventually made it to the Supreme Court. Google, Amazon, and the Electronic Frontier Foundation argued in favor of Alice, saying that abstract software ideas without any specific implementation details could not be patented.

The Supreme Court decided that CLS Bank's patent was not valid, but did not provide a clear benchmark by which trivial 'abstract' software patents could be distinguished from non-trivial ones. The ruling declared that patent eligible software must not be "routine," "conventional" or "generic," but did little to define these terms as they related to software. The Washington Post [wrote](https://www.washingtonpost.com/news/the-switch/wp/2014/06/20/the-supreme-courts-decision-on-software-patents-still-doesnt-settle-the-bigger-question/?utm_term=.33bb309294f0) at the time:

> [W]hile the court struck down what was universally said to be a bad patent, it didn't do much to say what kinds of software should be patentable. In other words, the court decided the most basic conflict in the case, but more or less declined to offer guidance for other, future cases.

_(See also: Bilski v. Kappos, 2010.)_

#### DDR Holdings, LLC v. Hotels.com, L.P. (2014)
Later in 2014, the Supreme Court would clarify its position regarding software patents. In DDR Holdings, LLC v. Hotels.com, the Supreme Court TODO

#### Enfish LLC v. Microsoft, Inc. (2016)

TODO

### Current Legal Landscape

### Consequences for Open Source

### License Comparison

## Copyright Law

TODO

## Warranty and Liability Law

TODO

## Attribution and Trademark Law

TODO

## Conclusion

TODO

---

## References, Statutes, and Cases Considered

* United States Constitution Article 1 § 8.8.
* 35 U.S. Code § 101
* Mackay Co. v. Radio Corp., 306 U.S. 86
* Gottschalk v. Benson, 409 U.S. 63 (1972)
* Diamond v. Diehr, 450 U.S. 175 (1981)
* Arrhythmia Research Technology, Inc. v. Corazonix Corporation, 958 F. 2d 1053 (1992)
* Alice v. CLS Bank 573 U.S., 134 S. Ct. 2347 (2014)
* DDR Holdings, LLC v. Hotels.com, L.P. (2014)
* Enfish LLC v. Microsoft, Inc. (2016)
* 17 U.S.C.A. § 102
* Apple Computer, Inc. v. Franklin Computer Corp. (1983)
* Step-Saver Data Systems, Inc. v. Wyse Technology (1991)
* Computer Associates International, Inc. v. Altai, Inc. (1992)
* Oracle America, Inc. v. Google, Inc. (2016)
* UCC 2-314
* UCC 2-315
* MIT license
* GPLv2 license
* GPLv3 license
* Apache 2.0 license

---

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
