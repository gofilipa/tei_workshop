[<<<Previous  ](README.md)  [Next>>>](what_is_xml.md)

# What is TEI?

### Defining TEI

**TEI stands for *Text Encoding Initiative*. Put most simply, TEI is a set of guidelines for the encoding of text. In more technical terms, it is a *markup schema* for representing the *structural, renditional,* and *conceptual features of texts*.** 

**TEI guidelines are based off XML, the eXtensible Markup Language, and were developed and are currently maintained by a scholarly and academic collective known as the TEI Consortium.**

Let's take apart this definition, bracketing (for now) the references to the TEI-C and XML, which we will discuss later. 

*Markup Schema*:
- *markup* means annotation or other descriptive marks within a text that instruct a compositor or typist how a particular passage should be printed or laid out. All printed texts are *implicitly encoded* (or marked up) in the sense of punctuation, capitalization, disposition of letters around the page, even the spaces between words. Markup helps the human reader determine where one word ends and another begins, or how to identify gross structural features such as headings or simple syntactic units such as dependent clauses or sentences.
- *schema* indicates a representation of a theory in the form of an model. Another way to think of it is as an instantiation of a theory, a set of rules or standards to be followed for that theory.

Markup schema, in other words, is a series of marks that indicate how a text ought to be presented in physical form. As such, there is an emphasis on the physical aspects of text such as chapter, paragraph, or poem structure, but as you will see, markup can also apply to non-physical textual elements, such as textual content or the agencies of writers/editors. 

*Structural*, *Renditional*, and *Conceptual* elements:
- Structural: concerns the structures of text, divisions, orderings (such as chapters). 
- Renditional: concerns how text renders visually on a page or screen, such as spacing and alignment.
- Conceptual: concerns the content of text, its meaning, cultural or personal references.

Markup therefore describes some aspect of the text, either by adding additional organizational, visible, or informational elements about that text. These elements range from the more objective, physical traces on the page/screen to the more subjective ideas and assumptions about meaning and references behind the words. 

## EXAMPLE--IMAGE FROM WWP?????

### Incommensurability 

With TEI, a text is encoded into a computer in a way that is searchable, presentable, and readable (interpretable) by the human. Encoding with TEI also adds the benefit of making the text *sustainable* across platforms. Because the format of the TEI itself is built from an extensible and non-invasive markup language (XML), it is widely useable and customizable, and will outlast more stylized file formats like a Microsoft Word document. 

While this makes TEI documents increasingly portable, it also creates the potential for problems regarding the handling of textual data. As humanists well know, textual data is open to interpretation. However, in order to be useful, the computer (and TEI specifically) imposes a certain level of fixity on textual data. In every text, there are what Jerome McGann calls “incommensurable elements”---elements that cannot be quantified, pinned down, or “tagged” in a fixed way. 

Though the strict tagging schema of TEI may inadvertantly encourage encoders to resolve a text’s inherent incommensurability, it does a good job addressing the more fixed and disambiguated textual elements in a way that reflects widespread agreeement *consensus* about these, while opening itself to more complex tasks. 

These questions, posed by the WWP, adequately frame how TEI might face such challenges: 

- How can the many disciplines and communities within the humanities domain find common ground in a single encoding language? 
- How do we agree on the level of detail that is necessary or appropriate in describing our textual materials? 
- How do we reconcile the advantages to be gained by consistency and agreement with the need for individual specialization? 
- How do we handle the truly idiosyncratic and unexpected? 

According to the WWP:

>Unlike many standardization efforts, the TEI addresses these and similar questions by *explicitly accommodating variation and debate within its technical framework.* The TEI Guidelines are designed to be both **modular** and **customizable**, so that specific projects can choose the relevant portions of the TEI and ignore the rest, and can also if necessary create extensions of the TEI language to describe facets of the text which the TEI does not yet address.”

In other words, TEI is built from a language (actually, a meta-language) that allows its users, in turn, to build their own version of that language. There is a potential here for representing the elements necessary to your project project by constructing these elements yourself. It also allows you to mix and match existing modules in order to meet your specific needs. 

Though this doesn't solve all issues relating to textual incommensurability, it's a start. In the next section, we are going to look a little bit at XML to get a glimpse of its potential for modularity and extensibility. 

[<<<Previous  ](README.md)[Next>>>](what_is_xml.md)

## Sources

[McGann, Jerome. *Radiant Textuality: Literature after the World Wide Web.* 2001.]

[*Women Writers Project*, "What is the TEI?"](https://wwp.northeastern.edu/outreach/seminars/tei.html).

[*Consortium of Text Encoding*, "TEI: Text Encoding Initiative".](https://tei-c.org/)
