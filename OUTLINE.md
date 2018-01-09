
# Outline

## Titles
* Nothing Is Implied: Legal Loopholes in Popular Open Source Licenses
* Mechanisms of Protection: Shortfalls in Popular Open Source Licenses

## Objectives
* To only use primary sources; that is, only cite cases, laws, and licenses.

---

## Introduction
* Brief history of the open source community
* Brief discussion of the most popular open source licenses

## Background and Case Law
* Licensing software is not a matter of simple permission. There are four major legal mechanisms that must be addressed.

### Patent law
* Patents allow for non-trivial algorithms and software designs to be held in temporary monopoly by a single entity.
* Derives from Article I, Section 8, clause 8 of U.S. Constitution.
* 35 U.S. Code § 101: "Whoever invents or discovers any new and useful process, machine, manufacture, or composition of matter, or any new and useful improvement thereof, may obtain a patent therefor, subject to the conditions and requirements of this title."
* Machine-or-transformation test: something is patentable if it is a non-trivial machine process or transforms something's physical state.

#### Precedent
* Gottschalk v. Benson, 409 U.S. 63 (1972) — software can be patented, algorithms excepted
* Diamond v. Diehr, 450 U.S. 175 (1981) — clarified *Benson*: algorithms part of a larger physical process can be patented
* Arrhythmia Research Technology, Inc. v. Corazonix Corporation, 958 F. 2d 1053 (1992) — algorithms part of concrete larger processes with tangible results are patentable
* Alice v. CLS Bank 573 U.S., 134 S. Ct. 2347 (2014) — 'abstract ideas' in software cannot be patented (Google, Amazon, and EFF argued such) --> WaPo: "[W]hile the court struck down what was universally said to be a bad patent, it didn't do much to say what kinds of software should be patentable. In other words, the court decided the most basic conflict in the case, but more or less declined to offer guidance for other, future cases."
* DDR Holdings, LLC v. Hotels.com, L.P. (2014) — clarified that non-trivial software can be patented (see Alice v. CLS Bank)
* Enfish LLC v. Microsoft, Inc. (2016) — upheld DDR Holdings LLC v. Hotels.com, LC (2014) decision that non-trivial software can be patented.

#### Summary
* Software patents on non-trivial processes are upheld, meaning that copyright is not the only mechanism by which software can be protected.
* Open source software licenses must be mindful of patents, as they could potentially be used to make free software nonfree.

| MIT | GPLv2 | GPLv3 | Apache 2.0 |
| --- | ----- | ----- | ---------- |
| no patent clause ("implicit") | no patent clause ("implicit") | patent grant & retaliation | patent grant & retaliation |

### Copyright law
* Unlike software patents, which protect non-abstract ideas, copyright protects source code and compiled binaries—software at large—from unauthorized re-use by third parties.
* In copyright law, the rights to any material is held by the _copyright holder_. The copyright holder can release materials under different terms to different entities.
* Software patents generally **do not release copyright**—they simply license the software.
* By default, all rights are reserved.
* Under 17 U.S.C.A. § 102, copyright protects "original works of authorship fixed in any tangible medium of expression, now known or later developed, from which they can be perceived, reproduced, or otherwise communicated, either directly or with the aid of a machine or device." Computer software is considered literary work under this definition (by Apple v. Franklin).

#### Precedent
* Apple Computer, Inc. v. Franklin Computer Corp. (1983) — a computer's operating system is protected by copyright
* Step-Saver Data Systems, Inc. v. Wyse Technology (1991) — "shrinkwrap" licenses ("by downloading this software, you agree...") are legally enforceable
* Computer Associates International, Inc. v. Altai, Inc. (1992) — non-literal elements of software are not copyrighted (UX, for example) --> led to Abstraction-Filtration-Comparison test
* Oracle America, Inc. v. Google, Inc. (2016) — trivial code cannot be copyrighted.

#### Summary
* Copyright is yet another legal mechanism by which software is controlled and regulated
* Object code is different from source code, however both are subject to copyright
* Non-trivial software is copyrighted, therefore it is necessary for open source licenses to explicitly grant permission for use.

| MIT | GPLv2 | GPLv3 | Apache 2.0 |
| --- | ----- | ----- | ---------- |
| granted | granted | granted if preserved ("infectious") | granted |

### Warranty and Liability
* Under the Uniform Commercial Code (UCC), sales have an implicit warranty that the items sold or shared are fit for a particular purpose. (UCC 2-314: Implied Warranty; Merchantability; Usage of Trade and UCC 2-315: Implied Warranty; Fitness for Particular Purpose.)
* Sales include gifts in many jurisdictions, meaning that open source software distribution is affected.
* To prevent open source contributors from being held legally (and therefore financially) liable for potential issues caused by their software, licenses must explicitly disclaim any warranty. (MIT does this in all caps.)
* Under Tort law, in order to recover for negligence, a plaintiff must prove (1) duty, (2) breach of duty, (3) causation, and (4) damages.
* All major open source licenses disclaim liability and warranty.

#### Precedent
* Disclaimers are found to be enforceable unless overruled by another law.
* **No precedent regarding tort liability exists.**

| MIT | GPLv2 | GPLv3 | Apache 2.0 |
| --- | ----- | ----- | ---------- |
| disclaimed | disclaimed | disclaimed | disclaimed |

### Attribution and Trademark
* Software might be licensed to the public, but the name of that software might be trademarked. (Example: Iceweasel as opposed to Firefox.)
* This trademark might prevent the software from being redistributed freely.
* At the same time, it is important that derivative works do not publish under the same name as the original to prevent confusion.
* It is also necessary to prevent the names of contributors of upstream projects being used as supposed endorsements of downstream projects.
* "You can share my code, but you can't share my brand." --> important impacts on distribution: renaming required.
* _See also: [fossmarks.org](http://fossmarks.org)]_

#### Precedent
* No litigation regarding open-source trademark infringement in United States federal courts exists. (Or at least none that I could find.)

| MIT | GPLv2 | GPLv3 | Apache 2.0 |
| --- | ----- | ----- | ---------- |
| no trademark clause | no trademark clause | trademark disclaimer allowed | use of trademarks _and name of licensor_ not allowed except as required for standard use (unmodified distribution) |

## Conclusions
* Lots of holes exist in popular open source licenses.
* GPLv3 and Apache 2.0 are the most 'secure.'
