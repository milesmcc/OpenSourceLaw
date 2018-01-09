# Nothing Is Implied: Legal Loopholes in Popular Open Source Licenses
Miles McCain

_Draft paper; please do not cite without author's permission._

## Abstract
In the United States, many legal mechanisms are in place that control and affect the distribution of computer software, including patents, copyright, liability, and trademark. The open source community uses a variety of licenses to explicitly allow the public to use its software freely. This survey of open source law finds that many of these licenses only explicitly address a small portion of these legal mechanisms, leaving the software's licensing ambiguous and subject to potential restriction. GPLv3 and the Apache 2.0 license are found to be the most secure and unambiguous licenses, while the MIT license and GPLv2 are found to leave important legal mechanisms governing open source software unaddressed.

## Introduction

TODO

## Patent Law

### Overview of Patent Law

Patents allow for ideas—user interfaces, design patterns, and algorithms—to be owned and protected independent of their technical implementation. First defined in the United States Constitution (Art. I § 8.8), patents are an integral part of intellectual property law. They provide inventors with a temporary monopoly—typically twenty years—to their idea, during which no other entity may use the idea without explicit permission from the patent holder. If a patent is infringed, the patent holder may sue for patent infringement and request that the infringer cease their use of the patented idea.

Given that patent law is applicable to software (Enfish LLC v. Microsoft, Inc. and DDR Holdings, LLC v. Hotels.com, L.P.) and that patent infringement can lead to both a fine and a legal order to cease use of the patented material, open source licenses must explicitly address patents to ensure that open source software remains available for free use. In order to understand how software licenses can address patents, however, it is necessary to first understand the legal precedents regarding software patents themselves.

### Software Patent Case Law

In 1972, inventor Gary Benson sued for patent infringement for unauthorized use of an algorithm he had patented: the process by which numbers in decimal notation could be transformed into binary notation. Benson claimed that all uses of his algorithm—be they automated by a computer or performed by hand—were subject to his patent. Calling the patented algorithm nothing more than a "law of nature," the court ruled against Benson and declared the patent invalid. Benson appealed, and eventually the case appeared before the Supreme Court. (Gottschalk v. Benson, 409 U.S. 63.)

There was little precedent at the time as to whether an algorithm could be patented. In 1939 it was ruled that mathematical expressions could not be patented (Mackay Co. v. Radio Corp., 306 U.S. 86), however Benson argued that his patent was not an _equation_ but rather a _process_—a particular way of solving an equation, so to speak. The distinction was lost on the Supreme Court justices, however, and they upheld the lower court's decision. Algorithms, they ruled, could not be patented. (Gottschalk v. Benson, 409 U.S. 63.)

The significance of this decision could not have been anticipated in 1972. Computers had yet to revolutionize the world, and many of the intricacies of modern programming had yet to even be invented. As computers began to occupy increasingly important roles in the world of business, however, companies began to worry whether their software—which was, after all, just a collection of algorithms—was patentable.

## Copyright Law

TODO

## Warranty and Liability Law

TODO

## Attribution and Trademark Law

TODO

## Conclusion

TODO

---

## References

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
