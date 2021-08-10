---
---
<a href="#nl">Nederlandse vertaling</a>

# Algorithm Register Metadata Standard

## Objectives

In this code base we define the metadata standard: what do we register about the algorithms being used in government, why and how.

[Glossary](/glossary)

[Attributes](/)

[User Stories](/user-stories) (in Dutch)

[Standard for Public Code complience](#publiccode)

## Inventarisations

All consortium organisations are working on a list of algorithms that they will be disclosing in the registry. Currently these are the lists of algorithms per organisation:


- Rotterdam
- Amsterdam
- Utrecht
- Den Haag
- Haarlemmermeer
- Zuid-Holland
- Noord-Brabant
- Limburg
- Kadaster
- Politie
- [Rijkswaterstaat](https://www.rijkswaterstaat.nl/en/about-us)
- the Association of Netherlands Municipalities (Vereniging van Nederlandse Gemeenten, VNG)
- UWV (Employee Insurance Agency)
- Ministry of Interior Affairs and Kingdom Relations

<h2>Nederlandse vertaling</h2>

# Algoritmeregister Metadata-standaard

In het project Publieke Controle op Algoritmes werkt [een consortium van Nederlandse overheden](https://publiekecontrole.com/about/) momenteel aan beleidsinstrumenten om de controle op systemen te vergroten. Een onderdeel daarvan is dat we werken aan een overzicht van algoritmes, een Algoritmeregister. Door in deze registratie aspecten van algoritmes op een begrijpelijke manier vast te leggen kunnen wij transparantie bieden en verantwoording af leggen. In het register kun je technische elementen terugvinden, zoals de dataverwerking of broncode, maar bijvoorbeeld ook afspraken tussen overheden en leveranciers of bijvoorbeeld een beschrijving van de werking van het algoritme.

## Doel

In deze code base leggen we de metadata standaard vast: wat leggen we vast over de algoritmes die gebruikt worden binnen de overheid, waarom, en hoe.

[Woordenlijst](/glossary)

[Attributen](/)

[User Stories](/user-stories)

## Inventarisaties

Alle organisaties binnen het consortium werken momenteel aan een inventarisatie van de algoritmes die ze willen ontsluiten middels het algoritmeregister. Hieronder een overzicht van voorlopige inventarisaties per organisatie (links volgen):

- Rotterdam
- Amsterdam
- Utrecht
- Den Haag
- Haarlemmermeer
- Zuid-Holland
- Noord-Brabant
- Limburg
- Kadaster
- Politie
- Rijkswaterstaat
- VNG
- UWV
- Ministerie van BZK

## Bijdragen

Bijdragen kunnen worden geleverd tijdens werkgroepbijeenkomsten en online via de [Code for NL slack omgeving](https://praatmee.codefor.nl) op kanaal #algoritmeregister.

## Status

Deze code base is in de prototype (pre-alfa) fase, dat wil zeggen dat alles nog ter discussie staat.

<a name="publiccode"></a>

# Standard for Public Code complience

We are planning on following https://standard.publiccode.net/ more and more over time:

### Nomenclature

. Not yet evaluated

v Complies

x Does not comply

\* Does not apply

? Not sure how to apply

### Code in the open
Status | Requirement | links and notes
-----|-----|-----
. | All source code for any policy and software in use (unless used for fraud detection) MUST be published and publicly accessible. |
. | Contributors MUST NOT upload sensitive information regarding users, their organization or third parties to the repository. |
. | Any source code not currently in use (such as new versions, proposals or older versions) SHOULD be published. |
. | The source code MAY provide the general public with insight into which source code or policy underpins any specific interaction they have with your organization. |

### Bundle policy and source code
Status | Requirement | links and notes
-----|-----|-----
. | A codebase MUST include the policy that the source code is based on. |
. | A codebase MUST include all source code that the policy is based on. |
. |All policy and source code that the codebase is based on MUST be documented, reusable and portable. |
. |Policy SHOULD be provided in machine readable and unambiguous formats. |
. |Continuous integration tests SHOULD validate that the source code and the policy are executed coherently. |

### Create reusable and portable code
Status | Requirement | links and notes
-----|-----|-----
. |The codebase MUST be developed to be reusable in different contexts. |
. |The codebase MUST be independent from any secret, undisclosed, proprietary or non-open licensed code or services for execution and understanding. |
. |The codebase SHOULD be in use by multiple parties. |
. |The roadmap SHOULD be influenced by the needs of multiple parties. |
. |Configuration SHOULD be used to make code adapt to context specific needs. |
. |Codebases SHOULD include a publiccode.yml metadata description so that they’re easily discoverable. |
. |Code and its documentation SHOULD NOT contain situation-specific information. |

### Welcome contributors
Status | Requirement | links and notes
-----|-----|-----
. |The codebase MUST allow anyone to submit suggestions for changes to the codebase. |
. |The codebase MUST include contribution guidelines explaining how contributors can get involved, for example in a CONTRIBUTING file. |
. |The codebase SHOULD advertise the committed engagement of involved organizations in the development and maintenance. |
. |The codebase SHOULD document the governance of the codebase, contributions and its community, for example in a GOVERNANCE file. |
. |The codebase SHOULD have a publicly available roadmap. |
. |The codebase MAY include a code of conduct for contributors. |

### Make contributing easy
Status | Requirement | links and notes
-----|-----|-----
. |The codebase MUST have a public issue tracker that accepts suggestions from anyone. |
. |The codebase MUST include instructions for how to privately report security issues for responsible disclosure. |
. |The documentation MUST link to both the public issue tracker and submitted codebase changes, for example in a README file. |
. |The codebase MUST have communication channels for users and developers, for example email lists. |
. |The documentation SHOULD include instructions for how to report potentially security sensitive issues on a closed channel. |

### Maintain version control
Status | Requirement | links and notes
-----|-----|-----
. |You MUST have a way to maintain version control for the code. |
. |All files in a codebase MUST be version controlled. |
. |All decisions MUST be documented in commit messages. |
. |Every commit message MUST link to discussions and issues wherever possible. |
. |You SHOULD use a distributed version control system. |
. |You SHOULD group relevant changes in commits. |
. |You SHOULD mark different versions of the codebase, for example using revision tags or textual labels. |
. |You SHOULD prefer file formats where the changes within the files can be easily viewed and understood in the version control system. |

### Require review of contributions
Status | Requirement | links and notes
-----|-----|-----
. |All contributions that are accepted or committed to release versions of the codebase MUST be reviewed by another contributor. |
. |Reviews MUST include source, policy, tests and documentation. |
. |Reviewers MUST provide feedback on all decisions to not accept a contribution. |
. |Contributions SHOULD conform to the standards, architecture and decisions set out in the codebase in order to pass review. |
. |Reviews SHOULD include running both the code and the tests of the codebase. |
. |Contributions SHOULD be reviewed by someone in a different context than the contributor. |
. |Version control systems SHOULD not accept non-reviewed contributions in release versions. |
. |Reviews SHOULD happen within two business days. |
. |Reviews MAY be performed by multiple reviewers. |

### Document your objectives
Status | Requirement | links and notes
-----|-----|-----
. |The codebase MUST contain documentation of its objectives – like a mission and goal statement – that is understandable by designers and developers so that they can use or contribute to the codebase. |
. |The codebase SHOULD contain documentation of its objectives understandable by policy makers and management. |
. |The codebase MAY contain documentation of its objectives for the general public. |

### Document the code
Status | Requirement | links and notes
-----|-----|-----
. |All of the functionality of the codebase – policy as well as source – MUST be described in language clearly understandable for those that understand the purpose of the code. |
. |The documentation of the codebase MUST contain:<ul><li>a description of how to install and run the source code,</li><li>examples demonstrating the key functionality.</li></ul> |
. |The documentation of the codebase SHOULD contain:<ul><li>a high level description that is clearly understandable for a wide audience of stakeholders, like the general public and journalists,</li><li>a section describing how to install and run a standalone version of the source code, including, if necessary, a test dataset,</li><li>examples for all functionality.</li></ul> |
. |There SHOULD be continuous integration tests for the quality of your documentation. |
. |The documentation of the codebase MAY contain examples that make users want to immediately start using the codebase. |
. |You MAY use the examples in your documentation to test the code. |

### Use plain English
Status | Requirement | links and notes
-----|-----|-----
. |All code and documentation MUST be in English. |
. |Any translation MUST be up to date with the English version and vice versa. |
. |There SHOULD be no acronyms, abbreviations, puns or legal/domain specific terms in the codebase without an explanation preceding it or a link to an explanation. |
. |The name of the codebase SHOULD be descriptive and free from acronyms, abbreviations, puns or branding. |
. |Documentation SHOULD aim for a lower secondary education reading level, as recommended by the Web Content Accessibility Guidelines 2. |
. |Any code, documentation and tests MAY have a translation. |

### Use open standards
Status | Requirement | links and notes
-----|-----|-----
. |For features of a codebase that facilitate the exchange of data the codebase MUST use an open standard that meets the Open Source Initiative Open Standard Requirements. |
. |If no existing open standard is available, effort SHOULD be put into developing one. |
. |Standards that are machine testable SHOULD be preferred over those that are not. |
. |Functionality using features from a standard that is not an open standard MAY be provided if necessary, but only in addition to compliant features. |
. |All non-compliant standards used MUST be recorded clearly in the documentation. |
. |The codebase SHOULD contain a list of all the standards used with links to where they are available. |

### Use continuous integration
Status | Requirement | links and notes
-----|-----|-----
. |All functionality in the source code MUST have automated tests. |
. |Contributions MUST pass all automated tests before they are admitted into the codebase. |
. |Contributions MUST be small. |
. |The codebase MUST have active contributors. |
. |Source code test and documentation coverage SHOULD be monitored. |
. |Policy and documentation MAY have testing for consistency with the source and vice versa. |
. |Policy and documentation MAY have testing for style and broken links. |

### Publish with an open license
Status | Requirement | links and notes
-----|-----|-----
. |All code and documentation MUST be licensed such that it may be freely reusable, changeable and redistributable. |
. |Software source code MUST be licensed under an OSI-approved open source license. |
. |All code MUST be published with a license file. |
. |Contributors MUST NOT be required to transfer copyright of their contributions to the codebase. |
. |All source code files in the codebase SHOULD include a copyright notice and a license header that are machine readable. |
. |Codebases MAY have multiple licenses for different types of code and documentation. |

### Use a coherent style
Status | Requirement | links and notes
-----|-----|-----
. |Contributions MUST adhere to either a coding or writing style guide, either your own or an existing one that is advertised in or part of the codebase. |
. |Contributions SHOULD pass automated tests on style. |
. |Your codebase SHOULD include inline comments and documentation for non-trivial sections. |
. |You MAY include sections in your style guide on understandable English. |

### Document codebase maturity
Status | Requirement | links and notes
-----|-----|-----
v | A codebase MUST be versioned. |
. | A codebase that is ready to use MUST only depend on other codebases that are also ready to use. |
v | A codebase that is not yet ready to use MUST have one of these labels:<ul><li>prototype - to test the look and feel, and to internally prove the concept of the technical possibilities,</li><li>alpha - to do guided tests with a limited set of users,</li><li>beta - to open up testing to a larger section of the general public, for example to test if the codebase works at scale,</li><li>pre-release version - code that is ready to be released but hasn’t received formal approval yet.</li></ul> |
. | A codebase SHOULD contain a log of changes from version to version, for example in the CHANGELOG. |
