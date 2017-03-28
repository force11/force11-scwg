# Software Citation session at CW17 (https://www.software.ac.uk/cw17), 28 March 2017
- FORCE11: [Software citation working group](https://github.com/force11/force11-scwg) / [PeerJ article](https://peerj.com/articles/cs-86/)
- slides: meetings/software-citation-cw17.pptx in https://github.com/force11/force11-scwg
- notes below by Martin O'Reilly [@martintoreilly](https://github.com/martintoreilly)

## Discussion session
- Responsibility on reviewers to ensure software used to generate research is suitably documented. "We used software" should be unacceptable. Journals should provide guidance for reviewers.
- Now principles are completed, the Software Citation Working Group will shut down and an implementation group will take over.
- There may be a grey area where arguments could be made on both sides about how much detail should be provided.
- What about citing the algorithms used within the software (e.g. the chain of techniques used within the software)?
  - Currently, often a "canonical" paper is cited, with potentially secondary papers referencing new algorithms and capabilities.
  - These secondary papers are often about the algorithm rather than the software.
  - A large number of citations for the "canonical" paper is how impact is demonstrated.
  - Conversely, particular funders may have funded only the later work, so citing these later papers is also necessary to demonstrate value for money.
- How to accumulate credit across multiple versions while citing specific software versions?
  - Chains of citations can work with papers, where papers tend to cite their dependencies. It's less common for software to cite other software (though )
  - Software papers are one option for this
  - Systems that publish software (e.g. Figshare / Zenodo) should support citations in their metadata
  - DOI metadata can include relationships to other DOIs
  - Could potentially look at Frbr (Functional Requirements for Bibliographic Records)
- Most people have published software papers or software (often both)
  - Software papers
  - How to people request citations?
    - Astropy: Points to the paper (mainly due to logistics of manually entering metadata in Zenodo).
    - One software prints references to papers as it runs algorithms as a citation reminder with hotlinks. Users don't read README files.
- State of software was cited while reviewing a paper?
  - Some reviewers have threatened to reject where software wasn't cited appropriately.
  - Some journal house styles effectively forbid referencing software due to style / typesetting rules.
  - Consensus seemed to be that journals generally didn't provide guidance on expectations for software citation.
  - Some journals do proivide guidance (e.g. [AAS](http://journals.aas.org/policy/software.html))

