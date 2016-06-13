This document contains comments made by the FORCE11 community on the draft Software Citation Principles, either directly on the [posted draft document](https://www.force11.org/software-citation-principles), via [GitHub issues](https://github.com/force11/force11-scwg/issues), or sent via email.
Here we will address these comments or discuss planned changes in response to them.

## Comments made via Hypothesis on the principles:

 * On unique identification: I know this suggestion of a single unique identifier comes from the DOI perspective where it works pretty well, but I'm wondering if something different in the way of identification should be used for software. For creative works generally there is the FRBR model - https://en.wikipedia.org/wiki/Functional_Requirements_for_Bibliographic_Records - which defines several levels for a creative entity - "work", "expression", "manifestation", and "item". I think something along these lines are particularly relevant for software - it is useful to be able to locate all uses of a particular piece of software no matter what version (the "work" level - software identified by a particular name and purpose over a period of time), but it is also important to specify the particular version used in any given work ("expression" - the source code at the time of use) and in some cases also the platform ("manifestation" - the compiled bytes including libraries, for example a docker image). "Item" probably isn't relevant for software. That is, I think a software citation perhaps could use THREE distinct unique identifiers, one for the work itself, one for the specific version (source code), and possibly an additional one for the actual downloadable binary image that can be run. Rather than leave it implicit I think recognizing the different levels of citable record would be helpful here. #F11SC

 Reply: I interpret the requirement for 'global uniqueness' as referring to the identifier itself. Two different people can have the same name (not globally unique) but cannot share a single ORCID (globally unique). Global uniqueness of the identifier does not preclude multiple identifiers pointing to the same person. I think the suggestion of differentiating between different software expressions/manifestations/items is a reasonable one, but I don't think it relaxes the requirement for identifiers to be globally unique.

 **Our response:**




 * On accessibility: Should this document address this in further detail? For example, "permit and facilitate access" could be explored further. Should this be done through open access licensing? repositories? who's responsible for providing this access?

 I am also wondering if this is a separate issue since "citing" traditionally pointed to publications but did not necessarily address access. DOI, for example is stated, but doesn't guarantee "access", so does this simply restating point 3, or should it provide something new?

 **Our response:**




 * On specificity: I am wondering if this should be folded into number 3 "Unique Identification". Both seem to deal with the issue of identification and access.

 **Our response:**




 * On academic credit: A lot of software that were developed by non-academic engineers also contribute to academic research indirectly. Their names and contributions should also be credited. So removing "Academic" makes more sense?

 Reply: This is a good point, though I think academic and non-academic credit are different, so perhaps we can add to this regarding non-academic credit, rather than removing "academic".

 Reply: I agree with Daniel on this. Keep Academic and add non-academic.

 **Our response:**  We've made the bullet more general, just about credit, discussing academic credit and adding a sentence about non-academic credit as well.



 * On citations in text: Although the focus here is on citations in the references, as a publisher, our experience is that most common practice of “citation” of data and software for authors is typically in the main body of the text. In order to encourage software to be treated and valued as a first-class research object, it is important that citations to it be positioned in the references as citations to articles and books are. However, it would be a missed opportunity if we did not leverage current practices of authors. This will also likely arise during implementation, as it has for the Data Citation Implementation Publisher Early Adopters Pilot. This could be addressed in future work on implementation.

 **Our response:**




 * On unique identification: Clearer instructions will be needed for authors on which version to cite. For BioMed Central journals, we ask authors to cite two versions of the software, an archived version (eg on Zenodo) as well as the current version (eg on GitHub). This is to ensure accessibility. However, if repositories and archives were to include a persistent link to the current version of the software, publishers could then instruct authors to cite only software with a UID, which wouldn’t point to a current version, but would point to the version(s) used and would be a more accurate version of scientific record. Related to this point is the idea of group object identifiers. A need for group identifiers has been identified in the area of data (eg in the case of meta-analyses), and one could also identify a use case for these in the case of software, collecting metadata around all versions of a given software package. See blog here (https://blog.datacite.org/to-better-understand-research-communication-we-need-a-groid-group-object-identifier/).

 **Our response:**




 * On future work: For implementation we would recommend both consulting with adopters as well as developing metadata standards simultaneously rather than developing metadata standards and then pursuing early adopters implementation. The work early adopters are doing now for data citation will be able to be leveraged for software citation and the changes needed to do so could happen now. There is no need to wait on approval of new tagging for a specific metadata standard. Many publishers will have their own preferred metadata standards and so implementation could begin now with publishers, as long as we know what we want to capture. Future implementation groups might also consider levels of contribution. This is particularly relevant for software. Who is considered an author? For example, to what extent should authors of pull requests receive attribution? This might be considered in an FAQs group, or possibly an early adopters group.

 **Our response:**




 * Additional thoughts (not sure what section this applies to): The principles do not address virtual machines. As these are becoming more common and relevant when addressing the reproducibility of research, it is important this “form” of software is acknowledged. The question remains in which cases should authors cite the current version, which the static archived version, and in which the virtual machine? In this way software is very much a unique evolving research object and might not fit perfectly into the same citation practices and structure as other research objects. In addition, software citation could possibly occur within the virtual machine. This could be added as a use case.

 **Our response:**





## GitHub issues:

 * On persistence of identifier vs. persistence of software (#143): The persistence principle outlined in (4) is a key element in making software citeable. Where software has become part of the record of science not only the identifier and metadata of the software should be persistent, it should also be the goal to keep a persistent copy of the source code, where applicable. This links with the accessibility principle (5).

 There are still many open questions about how to resolve package dependencies in the long term, therefore I would not make the persistent access to code a hard requirement but may add something more specific towards preserving the record of science.

 **Our response:**




 * Granularity of the citation (#140): one of the key issues with any citation, whether document, individual, or software is the specificity of what is being cited. in the case of publications, there is almost zero specificity most of the time.

 it's very easy to cite an entire package even though one function was used. part of this problem is being solved in the Python world through this project (https://github.com/duecredit/duecredit).

 any citation should have the ability to specify more than just the obvious, but even the obvious would be a good starting point.

 the citation/url should therefore allow for greater specificity within a code base. in general though, a provenance record of the workflow would be significantly more useful than a citation from a research perspective.

 **Our response:**




 * "Software citations should permit ... access to the software itself" (#138): Under the "Access" header, the data declaration states that:

 > "Data citations should facilitate access to the data themselves"

 Under the same header, the software declaration states:

 > "Software citations should permit and facilitate access to the software itself "

 The addition of "permit" suggests that software citations should also grant the user with permission to access the software. Is this intentional?

 It doesn't seem like a good idea to make access a requirement for discovery, so "permit" might not be helpful in this sentence.

 **Our response:**




 * Access to software: free vs commercial (#137): The section talks about software that is “free” as well as “commercial” software. I am not sure whether this is about free as in freedom (or just gratis or freely available), since it is compared with commercial software, which is unrelated in general, see http://www.gnu.org/philosophy/words-to-avoid.html#Commercial

 I suppose that “free” should be replaced by “gratis” and “commercial” be replaced by “non-free” in that section.

 **Our response:**




## From Mike Hucka:

 1. On the topic of persistent identifiers: we've faced similar problems in the area of biology.  An example situation is that annotations within a computational model point to data references, but the physical locations of those data items may change; the models can't reasonably be updated all the time, so we needed a scheme for uniform persistent identifiers that get resolved to the right thing.  Some close colleagues of mine developed http://identifiers.org for this purpose.  It was then natural to use this machinery when we developed a scheme for identifying the specifications for data formats in COMBINE: http://co.mbine.org/standards/specification-infrastructure . What struck me while reading Section 5.7 in your paper is that the same approach could be used to identify software, both specific versions as well as the software in general.

 What I imagine is creating identifiers along the following lines, as a start:

 http://identifiers.org/software/name
 http://identifiers.org/software/name.X
 http://identifiers.org/software/name.X.Y
 http://identifiers.org/software/name.X.Y.Z

 For instance (this does not exist -- just to illustrate the line of thinking):

 http://identifiers.org/software/libsbml
 http://identifiers.org/software/libsbml.5
 http://identifiers.org/software/libsbml.5.13
 http://identifiers.org/software/libsbml.5.13.0

 Since identifiers.org id's are both unique identifiers (in the URI sense) and resolvable (in the URL sense), they could be both the identifier of the software as well as a way for people to click on links and be sent to locations where the software is found (or alternatively, described somehow).

 The above examples are obviously incomplete in terms of a scheme -- this is just an initial idea, and I only mean to bring it up as something that could potentially be done.  I'd be interested in pursuing this further if you are interested.

 **Our response:**




 2. On p.6, the paper mentions the NIH Software Discovery Index meeting report, but the online copy of the report is a poor copy of what used to be online.  I happened to have saved a copy of the report as PDFs of the web pages shortly before the end of the NIH comment period.  In case it's of any use to anyone, I put a copy here:

 https://gist.github.com/mhucka/44921ea1e9a01697dbd0591d872b7b22

 **Our response:**  Thanks - this is helpful.  We've added this link to the bibliography as well.

