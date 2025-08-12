# Guidelines for Thesis Writing

So, you are writing a thesis! Whether you’re doing an MSc or PhD, writing a thesis involves much more than putting words on a screen. It needs clarity of thought and effective communication. Going through the process can help us become better writers and researchers.

In the sections below, you can find some notes that I have compiled throughout the years when supervising students. They contain (to some extent, opinionated) tips for making academic writing more effective, including different aspects—structure, tone, grammar, and LaTeX usage. The document also includes a few methodological resources that go a bit beyond what we would strictly call _writing_.

If you have any suggestions for improving these guidelines, don't be shy to send a pull request my way.


## Academic writing

### Writing the Abstract 

An abstract should succinctly summarize the *entire* document, including background, objectives, methods, key findings, and conclusions. That being said, you can and should allow more characters for the more important parts of the document, such as the results. 

Abstracts can also use a [structured format](https://dl.acm.org/doi/abs/10.1007/s10664-008-9075-7), with each paragraph being explicitly labeled with what it is trying to convey. 

As an example, for a research proposal, the abstract could have around six short paragraphs:
* Context: Wider topic, general motivation (why is it important to work on the topic)
* Related work: What are the key aspects we can learn from related work, and to what extent does previous work not satisfy us (and the world)
* Objectives: what you want to achieve, what do you want to contribute that adds to what the world already knows
* Methods: What research methods do you propose to apply
* Work plan: Very high-level view of what you plan to do and when
* Preliminary work: If anything, what have you already started doing, and the main conclusion

### General writing style

* *Keep a consistent narrative voice.* Choose between “we” or “I” and remain consistent throughout the text. Both are grammatically correct, but I tend to prefer “we”, as it sounds more inclusive and less self-centered than repeating “I did this, I did that”.

* *Favor active voice.* While passive voice is acceptable, the active voice typically leads to clearer, more engaging prose. Using active voice also leaves fewer doubts regarding whether we are talking about our own work or someone else's. For example: “We analyzed the data” is preferable to “The data was analyzed.”

* *Avoid contractions.* For example, write “it is” instead of “it’s” and “do not” instead of “don’t.” This keeps the tone more formal. 

* *Use proper conventions for quoting and for paraphrasing.* When quoting verbatim, always use quotation marks and include a citation. Italics may be used for emphasis. When paraphrasing, quotation marks aren’t needed, but referencing remains essential.

* *Avoid using document elements as the main sentence subjects.* For example, rather than “The previous section shows...” write “The analysis in the previous section shows...”.

* *Capitalize references to document elements.* Expressions like “Section 3.2”, “Table 4”, or “Figure 5” are [proper nouns](https://en.wikipedia.org/wiki/Proper_noun) and, as such, they are usually capitalized.

* *Avoid referring to sections as "sub-sections".* Irrespective of how deep they appear in the document structure, it suffices to refer to them as "sections". 

* *Write compound adjectives with a hyphen.* A [compound adjective](https://www.woodwardenglish.com/lesson/compound-adjectives-in-english/) is a combination of two or more words acting as a single idea. The words in a compound adjective should be linked through a hyphen. For example, “high-level analysis” instead of “high level analysis”. 

* *Use "that" and "which" in different cases.* Use "that" for restrictive clauses (essential to the sentence's meaning) and "which" for non-restrictive clauses (which add non-essential information). For example: “The method that we selected...” vs. “The method, which was developed in 2019, ...”. See https://english.stackexchange.com/a/490277

* *Define acronyms upon first use.* Always write the full term with the acronym in parentheses the first time (e.g., “Systematic Literature Review (SLR)”).

### Tables and figures

* *Make titles of figures and tables descriptive.* If they are long, that's fine, but confirm that your "list of figures" and "list of tables" at the beginning of the document [use shorter versions](https://tex.stackexchange.com/a/11580).

* *Choose a proper placement for table and figure captions.* With most styles and templates, [table captions appear above the tables and figure captions below the figures](https://tex.stackexchange.com/questions/3243/why-should-a-table-caption-be-placed-above-the-table). This aligns with how we naturally interpret tables (top-down) and figures (bottom-up).

* *Place figures after their first mention.* Try to ensure that figures are always mentioned in the main text, and that it happens before the actual figure appears, to support the logical flow when reading the document.

### Formatting with LaTeX

* *Use typographic emphasis appropriately.* Use:
  * Bold for key structuring terms (`\textbf{}`)
  * Italics for emphasis or foreign words (`\textit{}`)
  * Teletype for code or technical terms (`\texttt{}`)
  * Small caps for names of software patterns (`\textsc{}`)

* *[Use dashes appropriately](https://www.merriam-webster.com/grammar/em-dash-en-dash-how-to-use)*:
  * Use a common dash (-), also called a hyphen, for joining compound words (e.g., well-known, high-speed) or for breaking words at the end of a line.
  * Use an "endash" for representing a range of numbers or dates (e.g., 2010–2020, the Boston—New York flight).
  * Use an "emdash" for replacing commas, parentheses, or colons in certain cases to add a more dramatic effect or clarity (e.g., The answer—the one he gave—was unexpected).

* *Avoid inconveniently-placed line breaks.* Prevent some elements from being separated over line breaks. You can do so by inserting a non-breaking space (~) instead of a space before \cite{} or \ref{}. For example, `Section~\ref{some_ref}` instead of `Section \ref{some_ref}`. This keeps citations and labels visually connected to their references.

### Visualizing information

* *Avoid pie and dognut charts*, as explained in the article _[Save the Pies for Desert](https://www.perceptualedge.com/articles/visual_business_intelligence/save_the_pies_for_dessert.pdf)_.

* *Design tables to effectively convey your message.* There are many factors to consider when communicating data, but designing an effective table is more often a matter of making formatting simpler. The animation below illustrates a few techniques that you can use.

![image](figures/remove-and-move-to-improve-data-tables.gif)

### References

* *Clarify author references.* When referring to work by multiple authors, use [“et al.”](https://en.wikipedia.org/wiki/List_of_Latin_phrases_(E)#et_alii) (e.g., “Smith et al. [42] found ...”).

* *Ensure the references are complete.* Typically, most of the references of a thesis will be included to support a review of the state of the art. Confirm that all of them include at least the names of the authors, the title, the name of the journal (in the case of journal publications), the name of the conference (in the case of conference publications), the name of the publisher, and the year of publication. Pay attention to LaTeX compilation errors, because most of the fields that are missing in the references will appear there.

### Review and refinement process

* *Say your writing.* When you have a first draft, [read it out loud](https://martinfowler.com/bliki/SayYourWriting.html).

### Precautions when releasing a version of your manuscript

Unless we are talking about a working version shared with a small [circle of trust](https://www.scrumbook.org/product-organization-pattern-language/development-team/circle-of-trust.html), always ensure that in versions of the document that you submit to the appraisal of others (use this as a quick checklist):

* The front matter (cover, abstract, table of contents) is complete and accurate.
* The abstract summarizes the entire document, that is, it includes the most essential information from each chapter, giving more relevance to the objectives and final results.
* The "list of figures" and "list of tables" at the beginning of the document feature appropriate captions (e.g., not too long; not including citations)
* All figures, tables, and citations are correctly placed and referenced throughout the document.
* You ran the text through spelling and grammar checkers (e.g., Grammarly).


## Research design

In your writing, it's important to clearly distinguish the relevance of your work (the "why") from its goals (the "what") and from the methods you will use to reach those goals (the "how").

### Motivating the work (the "why)

* _Start with "why?"._ Explain clearly [why someone should care to read the rest of your document](https://martinfowler.com/bliki/SayYourWriting.html) before you explain what you intend to build or contribute, and how you propose to get there.

### Setting the goals (the "what")

* *Find appropriate research questions.* A research question often needs to be refined through a few iterations. Good research questions should be:
 * Clear — Easily understood, using established and unambiguous terms.
 * Specific – Focused on a well-defined topic or phenomenon, so that the research remains manageable and can yield meaningful results.
 * Falsifiable – The question is framed so that we can use empirical means to show that something is not supported by evidence.
 * Feasible – We can answer the question with the available time, resources, skills, and access to data or participants.
 * Original – Addresses a gap in current knowledge, challenges a common assumption, or seeks to provide a new perspective.
 * Conducive to discussion – Avoid questions leading to simple yes/no answers; good questions require analysis and allow a direct answer, but also foster discussion and depth.

### Setting the methods (the "how")

* *Clearly describe the design of your study(ies).* Always present the logical structure of your study, ideally with a visual diagram illustrating the steps and their expected outcomes. This helps the reader understand how the different parts of the methodology fit together.

### Reporting the results

* *Beware the use of the term "significant".* I usually reserve its use for statistically proven findings (e.g., p-value < 0.05) to avoid ambiguity.



## Preparing a research poster

 * Advice on templates and information – https://colinpurrington.com/tips/poster-design/
 * An example: https://github.com/yijunyu/demo/blob/master/doc/fast-poster-A0.pdf


## Preparing your thesis defense

The thesis defense marks the culmination of all the work you’ve done during a relevant chapter of your life, and it deserves to be honored properly. Therefore, it's not surprising that some people will easily get caught in anxiety. Do your best to prepare well, but don't forget to face the moment as a celebration of everything you’ve achieved.

A few aspects of *preparing well* are:
* Stick religiously to the time you have to present your work. This usually means training, training, training, and training again to get the time right. It's much preferable to finish a couple of minutes early than it is to finish a couple of minutes late.
* Anticipate possible questions of jury members, and incorporate them in the presentation
* Doing a final dry-run with your supervisor(s) and extended research team, if there is one, and listening to their feedback.


## Tools and resources

Tools I strongly advise:
  * overleaf.com - Write the document and easily share it with (and collect feedback from) your advisor(s). Keep a local git clone of the document, though.
  * grammarly.com - Check the state of your grammar and general writing. 

Other useful tools:
  * litmaps.com: Visual tool to explore related literature.
  * elicit.com: AI assistant for literature search and evidence synthesis.

Further resources
  * [ACM Empirical Standards](https://www2.sigsoft.org/EmpiricalStandards/docs/standards) – Choose the most appropriate research methods to answer your research questions, and use them well.
  * [Systematic, scoping, and rapid reviews: An overview](https://www.lib.sfu.ca/about/branches-depts/rc/writing-theses/writing/literature-reviews/systematic-scoping-rapid-reviews) – Choose the kind of review is right for you.


## Further references about what a PhD is

* [A PhD in Numbers](https://davidstutz.de/a-phd-in-numbers/), by David Stutz – Example of  *what a PhD can look like in terms of everyday work*.
* [How to get a PhD](https://discovery.up.pt/permalink/351PUCS_INST/19qmr6j/alma990005724620108801), by Estele Phillips – Book on the different concerns to consider and best practices when doing a PhD.
 





