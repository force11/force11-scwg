# Editor's Comments

## MAJOR REVISIONS

First of all, I would like to thank the reviewers, who have done a fantastic job and provided very insightful comments for improving the paper. I hope that the authors will take them into serious consideration in the revision.

From my personal perspective, this is a very good contribution, which addresses one of the most important topics in the "citation" domain, i.e. software citation. I totally agree with the reviewers about the readability of the paper, and I think this paper will deserve publication in PeerJ CS.

However, there are some aspects that should be clarified in the revision. In particular:

 - I would like to see a new section that describes the presentation of these principles at FORCE 2016, and includes also a summary of the most important outcomes derived from the discussion the authors have done during the conference. Did such outcomes change some of the principles and/or other claims in this paper?

 - The link between the principles and the requirements should be introduced explicitly, since it is not entirely clear how ones are connected to the others.

 - A clear research question should be announced explicitly from the very beginning, and accompanied by a text that explains how the authors would like to address it.

 - I suggest to include one or more appendixes with all the details about the use cases presented. This would make the paper more self-contained.

 - The reviewers did not agree on some aspects described in the paper, e.g. "if the software authors ask that a paper should be cited, that should typically be respected". I would like to see an appropriate discussion on these points, so as to clearly address these disagreements.

All these aspects should be clearly addressed, revising the paper accordingly, so as to deserve a publication in PeerJ CS - that's why I've assigned "major revision" as final decision of the paper.

In addition, I would also like to see a full addressing of all the other relevant comments made by the reviewers, accompanied by an appropriate response letter.


# Reviewer 1 (Tobias Kuhn)

##Basic reporting

This paper argues for the adoption of software citations, basically for the same reasons that data citations have been advocated: Because software packages have become so important in science, they should be appropriately credited and referenced, which can be achieved if we extend the concept of citations in scientific articles.

The paper tackles an important problem and provides a very valuable foundation for further discussions and future implementations. In particular, the six software citation principles presented in the beginning are very valuable.

While I think this is a very useful paper, I see the following problems with the current version:

 - The logical connections between the different parts of the paper are not clear. For example, how do the "basic requirements" of Table 2 map to the "principles" in Section 1? And are the principles presented in the beginning the *outcome* of this research (this is what lines 29+ seem to suggest) or are they *assumptions* of the approach to be discussed and evaluated (this is how they seem to be treated in Section 5).

 - It is not clear whether the authors consider software citations to be just the first step towards a long-term vision, or whether they consider software citations the overall final solution. It seems that the first is the case, but the long-term vision is not discussed.

## Experimental design

This paper doesn't have an experimental design in the strict sense, as it is more of a position paper than a research article. The PeerJ guidelines state that "the submission should clearly define the research question", which is currently not the case for this paper. However, I see a research question between the lines, which could be phrased as "how can citations be applied to software products to account for their increasing importance in scientific research?". By making such a research question explicit, the PeerJ requirements can be met.

The use cases described in Section 3 form the main method to answer the implicit research question. Given the importance of these use cases for this paper, I think reference [18] with the details about these use cases should be published in a more official way, either on a site like ArXiv or FigShare, or maybe even as supplemental material or appendix for this paper. I think having these use cases in the appendix of this paper would be the best solution, which would also increase the impact of these use cases and would strengthen the paper in general.

## Validity of the findings

As noted above, the logical structure of the paper is unclear, and therefore it is not clear what exactly the main findings are. I think the main findings should be the principles stated in the beginning, and the use cases would then form the main method to arrive at these findings. Alternatively, one could label the principles as "assumptions" and apply the use case study to validate these assumptions. In any case, I think the findings are valid but they should be labeled as preliminary, as it is not possible to arrive at a final conclusion for such kinds of questions. Only the future can tell whether software citations really work out.
Comments for the Author
Below are some more specific comments.

 - line 88: "which will be presented ..." > "which was presented ..."

 - line 89: "We expect that this discussion may lead to a second, final version": So this paper is not the final version? Please clarify.

 - line 97: "the need for credit for application software underscores the need to overhaul the system of credit for all research products.": Very true and very important. But then maybe the concept of a "citation" is obsolete altogether, and we shouldn't be advocating "software citations", but something new altogether? Some more discussion on this would be valuable, I think. This relates to my comment above about a long-term vision.

 - line 238: "Citation is a record of software that is important to a research outcome": This is another important issue, but not much more is said about this. What makes a software "important" to a research outcome? Or, more generally, what is the semantics of a software citation?

 - line 254: "In addition, if the software authors ask that a paper should be cited, that should typically be respected": I think I disagree with that. Whether a paper should be cited or not should *not* depend on whether the given software package tells you to do so. Such pointers can be useful as suggestions, but not more than that in my opinion.

 - Lines 308+: You don't imply that this list is complete, but wouldn't an identifier of a software *branch* be another important type of identifier? For example, the Windows "version" of a software package. Also, I see in what situation one would use (1) or (2) with respect to software citations, but what is the purpose of (3) in the context of citations?

 - Line 325: "other software may be available as a service": This makes a huge difference, doesn't it? I think some more discussion on this would be helpful. For example, with software services it can be hard to find out what the official name of the software is, let alone the developers or version numbers. Also, does a software that is only available as a service (e.g. REST API) violate the Accessibility principle (5)?

I find it a bit weird to quote passages from the same paper like "The Accessibility principle (5) states that “....”" (line 329 and others).

In the discussion about Unique identification (lines 292+), I miss the discussion of hash values as version identifiers, as applied by Git for instance. As the first author is affiliated with GitHub, I assume this aspect was left out intentionally, but why? As basically all software is nowadays maintained with version control systems such as Git, these identifiers come for free and are by design unique. So, I would think they are an important aspect to discuss for software citations.


# Reviewer 2 (Graham Klyne)

## Basic reporting

[The submission must adhere to all PeerJ Computer Science policies]

This was not specifically checked by me, but I see no indication that it violates any reasonable policies.

[The article must be written in English ...]

Then paper is written in clear and respectful English. I found it easy to read.

[The article should include sufficient introduction and background...]

Apart from the principles themselves, I found the background provided to be very useful, relevant and well-referenced.

[The structure of the submitted article should conform to one of the templates...]

I believe the variation in structure from the norms suggested paper is well suited to its purpose. (See also my response at "Validity of findings".)

[Figures should be relevant to the content of the article...]

The two tables are relevant and helpful, though I did have a slight problem with the legibility of my printed copy of Table 2 (page 5). The distinction between solid and open circles was not immediately clear to me, and I might suggest using a slightly larger version of these symbols.

[The submission should be ‘self-contained,’ should represent an appropriate ‘unit of publication’...]

The submission appropriately addresses the topic indicated by its title ("principles"), and material deferred to separate publication ("technical solutions" and "examples") seems to be an entirely reasonable separation of concerns.

[All appropriate raw data has been made available in accordance with our Data Sharing policy]

N/A

[Formal results should include clear definitions of all terms and theorems, and detailed proofs]

N/A

## Experimental design

N/A - see "Validity of findings"

## Validity of the findings

The paper does not present a specific research finding, and as such does not feature a research question and experimental procedure that are expected of such papers. However, I think it makes in important contribution to the acceptance of software as part of the process and output of research activity, and reflects a consensus formed among a significant community of researchers. As such, I believe it justifies a place in the formally published literature.

The motivation for the work is clearly stated, and the paper adds clarity and depth to discussion of the role of software in research, and its attendant citation as such.

The process by which the proposed principles were arrived at is described across sections 1-4, and relevant information is referenced, so the principles articulated have a clear provenance and basis in research practice.

(I note that some research fields recognize "method papers", and I would judge this submission by the the standards of such papers rather than as a presentation of a specific research finding.)

## Comments for the Author

The following comments are offered for the authors' consideration. I don't think any affect the fundamental value of the paper as presented.

Lines 32-35: as a justification for treating software differently from data, I found this passage raised more questions than answers, and that the comments here were uncompelling and unsupported. For example, some published data is updated on a frequency comparable with some software (e.g. the bi-monthly release schedule of FlyBase is comparable with many software projects - http://flybase.org/static_pages/docs/release_schedule.html). Also, I think the distinction between data and software is less clear-cut than the authors suggest (e.g. is a schema or stylesheet data or software?). I would see the difference between software and data as more akin to the difference between research methods and research findings, but that is just a personal opinion. My suggestion would be that this justification is not really necessary to the overall purpose of the paper, and might be dropped without significant loss of value.

Line 57, et seq: [Nit] I would find this easier to read if the sentence introducing the list of reasons were moved to the same page as the list itself.

Line 88: "will be presented" refers to an event now in the past: change to "was presented"?

Line 113: [Nit] "work using software" appears to be very broadly scoped, and could apply to just about any activity using a computer. Suggest "research using software".

Table 2, page 5: I had a problem with the legibility of my printed copy of this table. The distinction between solid and open circles was not immediately clear to me. I might suggest using a slightly larger version of these symbols, or maybe more distinct symbol shapes.

Table 2, page 5: [Comment] This table contains a lot of information, and much food for debate. I was surprised by some ommissions, which may mean that I wasn't fully understanding the concepts being presented:

(a) I find it hard to imagine any of the use cases not benefiting from availability of a "Description", especially 1, 2, 9, and 16.
(b) I would have expected "Indexed citations" to be useful for 5: getting credit.
(c) For publishing a software paper, I would expect all of the basic requirements other than "Indexed citations" to be at least beneficial.
(d) For 12: build a software catalog/registry, would there not be a role for indexed citations?
(e) For 16: Store software try, I'd expect pretty much all of the Basic requirements other than "Indexed citations" to be relevant, and particularly "Description" and "Keywords".
(f) I think there is one use-case missing, which I think is commonly faced by researchers: viz. "Evaluate suitability of software for a given task" - I think this is distinct from discovery, and typically involves making a choice between different available software packages, or to use an existing package, modify an existing package or develop something new.

Line 175: [Nit] "in(1)" Missing space?

Lines 241-242: "Similarly, the software metadata that is recorded as part of data provenance should be a superset of the metadata recorded as part of software citation." I found this non sequitur (or am not seeing the logical connection). I can imagine reasons to cite software that does not form part of the provenance chain of results presented (e.g. alternatives considered).

Lines 245-247: "In general, we intend the software citation principles to cover the minimum of what is necessary for software citation for the purpose of software identification. Other use cases (e.g., provenance, reproducibility) may lead to additional requirements (i.e., enhanced metadata)." This statement feels to me to be at odds with table 2, which presents "Use cases and basic metadata requirements for software citation", which includes "reproducibility" as a use-case. This leaves me wondering if the use cases in table 2 are going beyond what is strictly needed for the purposes of software citation.

Line 327-328: "When software exists as both source code and another type, we recommend that the source code be cited". The term "exists" here doesn't seem quite right to me. E.g., proprietary software may "exist" as source code, but be unavailable. Suggest "exists and is accessible" or just "is accessible"?

Line 348: "Updates to this document". This paper is being presented for consideration as a part of the formal academic record - as such, I don't think "this document" is something which may be updated. Suggest "Updates to these principles".
