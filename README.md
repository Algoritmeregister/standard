---
title: Readme
description: Readme file on the code base
---
<a href="#nederlandse-vertaling">Nederlandse vertaling</a>

# Algorithm Register Metadata Standard

## Objectives

In this code base we define the metadata standard: what do we register about the algorithms being used in government, why and how.

[Attributes](https://standaard.algoritmeregister.org/standard)

[Glossary](https://standaard.algoritmeregister.org/glossary)

[User Stories](https://standaard.algoritmeregister.org/user-stories) (in Dutch)

[Standard for Public Code compliance](#publiccode)

## Policies

The Algorithm Register Metadata Standard aims to help implement two policies for algorithm registers.

### Laying down harmonised rules on artificial intelligence (Artificial Intelligence Act) and amending certain union legislative acts

The proposal, [2021/0106(COD)](https://eur-lex.europa.eu/legal-content/EN/TXT/?qid=1623335154975&uri=CELEX%3A52021PC0206), from the European Union states:

> [The Commission] will establish a system for registering stand-alone high-risk AI applications in a public EU-wide database. This registration will also enable competent authorities, users and other interested people to verify if the high-risk AI system complies with the requirements laid down in the proposal and to exercise enhanced oversight over those AI systems posing high risks to fundamental rights. To feed this database, AI providers will be obliged to provide meaningful information about their systems and the conformity assessment carried out on those systems.

It should be noted that this act is still being processed.

### Motie van het lid Klaver c.s. over opzetten van een algoritmeregister

The motion, [35510-16](https://www.tweedekamer.nl/kamerstukken/brieven_regering/detail?id=2021Z00984&did=2021D02426), in the Dutch House of Representatives calls on the government to:

> set up an algorithm register describing which algorithms the government uses, for what purpose and of which datasets they rely on, so that everyone can monitor whether the algorithms are discriminatory, and follow current rule of law.

It should be noted that while the motion has passed in the House, it has not been signed into law yet.

## Inventarisations

All consortium organisations are working on a list of algorithms that they will be disclosing in the registry: https://www.algoritmeregister.nl/

<h2>Nederlandse vertaling</h2>

# Algoritmeregister Metadata-standaard

In het project Publieke Controle op Algoritmes werkt [een consortium van Nederlandse overheden](https://publiekecontrole.com/about/) momenteel aan beleidsinstrumenten om de controle op systemen te vergroten. Een onderdeel daarvan is dat we werken aan een overzicht van algoritmes, een Algoritmeregister. Door in deze registratie aspecten van algoritmes op een begrijpelijke manier vast te leggen kunnen wij transparantie bieden en verantwoording af leggen. In het register kun je technische elementen terugvinden, zoals de dataverwerking of broncode, maar bijvoorbeeld ook afspraken tussen overheden en leveranciers of bijvoorbeeld een beschrijving van de werking van het algoritme.

## Doel

In deze code base leggen we de metadata standaard vast: wat leggen we vast over de algoritmes die gebruikt worden binnen de overheid, waarom, en hoe.

[Woordenlijst](https://standaard.algoritmeregister.org/glossary)

[Attributen](https://standaard.algoritmeregister.org/standard)

[User Stories](https://standaard.algoritmeregister.org/user-stories)

## Inventarisaties

Alle organisaties binnen het consortium werken momenteel aan een inventarisatie van de algoritmes die ze willen ontsluiten middels het algoritmeregister: https://www.algoritmeregister.nl/

## Bijdragen

Bijdragen kunnen worden geleverd tijdens werkgroepbijeenkomsten en online via de [Code for NL slack omgeving](https://praatmee.codefor.nl) op kanaal #algoritmeregister.

## Status

Deze code base is in de prototype (pre-alfa) fase, dat wil zeggen dat alles nog ter discussie staat.

<a name="publiccode"></a>

# Standard for Public Code compliance

We are planning on following https://standard.publiccode.net/ more and more over time:

### Nomenclature

. Not yet evaluated

v Complies

x Does not comply

\* Does not apply

? Not sure how to apply

### Code in the open
- [x] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v | All source code for any policy and software in use (unless used for fraud detection) MUST be published and publicly accessible. |
v | Contributors MUST NOT upload sensitive information regarding users, their organization or third parties to the repository. |
v | Any source code not currently in use (such as new versions, proposals or older versions) SHOULD be published. |
v | The source code MAY provide the general public with insight into which source code or policy underpins any specific interaction they have with an organization. |

### Bundle policy and source code
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v | A codebase MUST include the policy that the source code is based on. |
v | A codebase MUST include all source code that the policy is based on. |
v |All policy and source code that the codebase is based on MUST be documented, reusable and portable. |
\* |Policy SHOULD be provided in machine readable and unambiguous formats. | Policy is not signed into its final form yet
x |Continuous integration tests SHOULD validate that the source code and the policy are executed coherently. |

### Create reusable and portable code
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v |The codebase MUST be developed to be reusable in different contexts. |
v |The codebase MUST be independent from any secret, undisclosed, proprietary or non-open licensed code or services for execution and understanding. |
x |The codebase SHOULD be in use by multiple parties. | Not in use by anyone yet?
v |The roadmap SHOULD be influenced by the needs of multiple parties. | Multiple parties involved, but no published roadmap yet.
\* |Configuration SHOULD be used to make code adapt to context specific needs. |
x |The codebase SHOULD include a machine readable metadata description, for example in a [publiccode.yml](https://github.com/publiccodeyml/publiccode.yml) file. |
v |Code and its documentation SHOULD NOT contain situation-specific information. |

### Welcome contributors
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v |The codebase MUST allow anyone to submit suggestions for changes to the codebase. |
x |The codebase MUST include contribution guidelines explaining what kinds of contributions are welcome and how contributors can get involved, for example in a CONTRIBUTING file. |
v |The codebase SHOULD advertise the committed engagement of involved organizations in the development and maintenance. | Listed in README
x |The codebase SHOULD document the governance of the codebase, contributions and its community, for example in a GOVERNANCE file. |
x |The codebase SHOULD have a publicly available roadmap. |
x |The codebase MAY include a code of conduct for contributors. |

### Make contributing easy
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v |The codebase MUST have a public issue tracker that accepts suggestions from anyone. | [issues](https://github.com/Algoritmeregister/standard/issues)
x |The codebase MUST include instructions for how to privately report security issues for responsible disclosure. |
x |The documentation MUST link to both the public issue tracker and submitted codebase changes, for example in a README file. |
? |The codebase MUST have communication channels for users and developers, for example email lists. | No mailing list yet, but a Slack channel is linked in the README
x |The documentation SHOULD include instructions for how to report potentially security sensitive issues on a closed channel. |

### Maintain version control
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v |The community MUST have a way to maintain version control for the code. | Git+GitHub
v |All files in a codebase MUST be version controlled. |
x |All decisions MUST be documented in commit messages. | The codebase is very young still with few contributors
x |Every commit message MUST link to discussions and issues wherever possible. | So few contributors so not many discussions to link to.
v |The codebase SHOULD be maintained in a distributed version control system. | Git
v |Contributors SHOULD group relevant changes in commits. |
x |Maintainers SHOULD mark released versions of the codebase, for example using revision tags or textual labels. | git tags are not yet in use, nor are releases published, versions can be seen in [file names](https://github.com/Algoritmeregister/standard/tree/main/schemas) and some commits reference versions, e.g: 3749673 , c62896e , eba10c0 , 4a6aa66
v |Contributors SHOULD prefer file formats where the changes within the files can be easily viewed and understood in the version control system. | Mostly markdown, json and yaml files. There is one pdf with a presentation of the codebase  that would be a great start for documentation.
v |Contributors MAY sign their commits and provide an email address, so that future contributors are able to contact past contributors with questions about their work. |

### Require review of contributions
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |All contributions that are accepted or committed to release versions of the codebase MUST be reviewed by another contributor. | Single contributor so far.
. |Reviews MUST include source, policy, tests and documentation. |
. |Reviewers MUST provide feedback on all decisions to not accept a contribution. |
. |Contributions SHOULD conform to the standards, architecture and decisions set out in the codebase in order to pass review. |
. |Reviews SHOULD include running both the code and the tests of the codebase. |
. |Contributions SHOULD be reviewed by someone in a different context than the contributor. |
. |Version control systems SHOULD NOT accept non-reviewed contributions in release versions. |
. |Reviews SHOULD happen within two business days. |
. |Reviews MAY be performed by multiple reviewers. |

### Document codebase objectives
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |The codebase MUST contain documentation of its objectives – like a mission and goal statement – that is understandable by designers and developers so that they can use or contribute to the codebase. | Very brief description
v |Codebase documentation SHOULD clearly describe the connections between policy objectives and codebase objectives. |
x |The codebase MAY contain documentation of its objectives for the general public. |

### Document the code
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
? |All of the functionality of the codebase – policy as well as source – MUST be described in language clearly understandable for those that understand the purpose of the code. | It would be better if this documentation was not only in the pdf; need to look to see what is not covered in the documentation
? |The documentation of the codebase MUST contain: a description of how to install and run the source code, examples demonstrating the key functionality.  | Discussion about what it would mean for someone else to use/test still needed
? |The documentation of the codebase SHOULD contain: a high level description that is clearly understandable for a wide audience of stakeholders, like the general public and journalists, a section describing how to install and run a standalone version of the source code, including, if necessary, a test dataset, examples for all functionality. | (some of this might be in the pdf?)
x |There SHOULD be continuous integration tests for the quality of the documentation. |
x |The documentation of the codebase MAY contain examples that make users want to immediately start using the codebase. |
x |The code MAY be tested by using examples in the documentation. |

### Use plain English
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |All codebase documentation MUST be in English. |
v |All code MUST be in English, except where policy is machine interpreted as code. |
v |All bundled policy not available in English MUST have an accompanying summary in English. |
? |Any translation MUST be up to date with the English version and vice versa. | Looks like they are up to date in the standard but not in the documentation
v |There SHOULD be no acronyms, abbreviations, puns or legal/non-English/domain specific terms in the codebase without an explanation preceding it or a link to an explanation. |
v |The name of the codebase SHOULD be descriptive and free from acronyms, abbreviations, puns or organizational branding. | Algoritmeregister "standard" vs "algorithmregistery-standard" could be discussed
x |Documentation SHOULD aim for a lower secondary education reading level, as recommended by the [Web Content Accessibility Guidelines 2](https://www.w3.org/WAI/WCAG21/quickref/?showtechniques=315#readable). |
. |Any code, documentation or tests MAY have a translation. |

### Use open standards
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
v |For features of a codebase that facilitate the exchange of data the codebase MUST use an open standard that meets the Open Source Initiative Open Standard Requirements. | Looks like it only requires a csv file to be generated
\* |If no existing open standard is available, effort SHOULD be put into developing one. |
v |Standards that are machine testable SHOULD be preferred over those that are not. |
\* |Functionality using features from a non-open standard (one that doesn’t meet the Open Source  Initiative Open Standard Requirements) MAY be provided if necessary, but only in addition to compliant features. |
\* |All non-compliant standards used MUST be recorded clearly in the documentation. |
x |The codebase SHOULD contain a list of all the standards used with links to where they are available. |

### Use continuous integration
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |All functionality in the source code MUST have automated tests. |
x |Contributions MUST pass all automated tests before they are admitted into the codebase. |
v |Contributions MUST be small. | However, there is not policy or guidance to contributors documented
x |The codebase MUST have active contributors. | currently there is only a single active contributor
? |Source code test and documentation coverage SHOULD be monitored. |
x |Policy and documentation MAY have testing for consistency with the source and vice versa. |
x |Policy and documentation MAY have testing for style and broken links. |

### Publish with an open license
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |All code and documentation MUST be licensed such that it may be freely reusable, changeable and redistributable. | There is no license file in the repository
x |Software source code MUST be licensed under an [OSI-approved open source license](https://opensource.org/licenses/category). |
x |All code MUST be published with a license file. |
. |Contributors MUST NOT be required to transfer copyright of their contributions to the codebase. |
x |All source code files in the codebase SHOULD include a copyright notice and a license header that are machine readable. |
. |Codebases MAY have multiple licenses for different types of code and documentation. |

### Use a coherent style
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
x |Contributions MUST adhere to either a coding or writing style guide, either the codebase community’s own or an existing one that is advertised in or part of the codebase. |
x |Contributions SHOULD pass automated tests on style. |
? |The codebase SHOULD include inline comments and documentation for non-trivial sections. |
x |The style guide MAY include sections on understandable English. |

### Document codebase maturity
- [ ] compliant with this criterion.

Status | Requirement | links and notes
-----|-----|-----
? | A codebase MUST be versioned. | Is 0.2 the schema and codebase version? is there any difference between the two?
\* | A codebase that is ready to use MUST only depend on other codebases that are also ready to use. |
v | A codebase that is not yet ready to use MUST have one of these labels: prototype - to test the look and feel, and to internally prove the concept of the technical possibilities, alpha - to do guided tests with a limited set of users, beta - to open up testing to a larger section of the general public, for example to test if the codebase works at scale, pre-release version - code that is ready to be released but hasn’t received formal approval yet. | It is marked, but only in Dutch in the README
x | A codebase SHOULD contain a log of changes from version to version, for example in the CHANGELOG. |
