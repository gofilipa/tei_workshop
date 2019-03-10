[<<<Previous  ](README.md)  [Next>>>](what_is_xml.md)

# What is TEI?

Before defining TEI, let's first take a look at some TEI code. Here is an example of some TEI encoding that indicates a piece of text has been struck out.

    <line>This is a <del>paragraph</del>line of text</line>

To those who are familiar with it, TEI, at first glance, looks a lot like HTML. Both use a tagging structure that encloses textual elements to indicate something about those elements. However, while HTML encodes how text should *appear* on a webpage, in the form of titles, headings, paragraphs, or links, TEI encodes the *content* of the text, in addition to some description about its appearance. 

Once a text is marked up with TEI, the relevant elements can be searched, processed, and rendered to facilitate scholarly research. It can be used to create any of the following: digital editions and archives, teaching anthologies, research corpora and collections, and many other forms of publication.

## Defining TEI

TEI stands for *Text Encoding Initiative*, and it defines a set of guidelines for the encoding of text. In more technical terms:

> TEI it is a **markup schema** for representing the **structural, renditional,** and **conceptual features of texts**. TEI guidelines are based off **XML**, the eXtensible Markup Language, and were developed and are currently maintained by an academic collective known as the **TEI Consortium**.

Let's take apart this definition, bracketing (for now) the references to the TEI-C and XML, which we will discuss later. 

*Markup Schema*:
- *markup* means annotation or other descriptive marks within a text that instruct a compositor or typist how a particular passage should be printed or laid out. All printed texts are *implicitly encoded* (or marked up) in the sense of punctuation, capitalization, disposition of letters around the page, even the spaces between words. Markup helps the human reader determine where one word ends and another begins, or how to identify gross structural features such as headings or simple syntactic units such as dependent clauses or sentences.
- *schema* indicates a model. Another way to think of it is as an instantiation of a theory, a set of rules or standards to be followed for that theory.

Markup schema, in other words, is a series of marks that indicate how a text ought to be presented on a page or screen. As such, there is an emphasis on the physical aspects of text such as chapter, paragraph, or poem structure, but as you will see, markup also applies to non-physical textual elements, such as textual content or the agencies of writers/editors. 

*Structural*, *Renditional*, and *Conceptual* elements:
- Structural: concerns the structures of text, divisions, orderings, such as titles or chapters. 
- Renditional: concerns how text renders visually on a page or screen, such as spacing and alignment.
- Conceptual: concerns the content of text, its cultural or personal references.

Markup therefore describes some aspect of the text by adding additional organizational, visible, or informational elements about that text. These elements range from the more objective, physical traces on the page/screen to the more subjective ideas and assumptions about meaning and references behind the visible elements. 

## Textual Ambiguity 

With TEI, a text is encoded into a computer in a way that is searchable, presentable, and readable (i.e. interpretable) by the human. Encoding with TEI also adds the benefit of making the text *sustainable*. Because the format of the TEI itself is built from a non-invasive markup language (XML), it can be preserved over time and across computer programs,and will outlast more stylized file formats like a Microsoft Word document. 

While this makes TEI documents increasingly portable, it also creates the potential for problems regarding the handling of textual data. As humanists well know, textual data is open to interpretation. However, in order to be useful, the computer (and TEI specifically) imposes a certain level of fixity on textual data.

Though the strict tagging schema of TEI may inadvertantly encourage encoders to resolve a text’s ambiguity, it does a good job addressing the more fixed and disambiguated textual elements in a way that reflects widespread *consensus* about these, while opening itself to more complex tasks. 

The Women Writers Project, a group of academics who work with TEI to encode women's writing, adequately frames how TEI uses its *inherent extensibility* to harness consensus while opening itself to more complex issues in text encoding. According to the WWP:

>Unlike many standardization efforts, the TEI ... *explicitly accommodat[es] variation and debate within its technical framework.* The TEI Guidelines are designed to be both **modular** and **customizable**, so that specific projects can choose the relevant portions of the TEI and ignore the rest, and can also if necessary create extensions of the TEI language to describe facets of the text which the TEI does not yet address.”

In other words, TEI is built from a language that allows its users,in turn, to build their own version of that language. As a result, there is potential for representing the elements necessary to a project by customizing these elements on a project-by-project basis. It also allows encoders to mix and match existing modules in order to meet their specific needs. 

Though this doesn't solve all issues relating to textual ambiguity, it's a start. In the next section, we are going to look a little bit at XML to get a glimpse of its potential for extensibility. 

[<<<Previous  ](README.md)[Next>>>](what_is_xml.md)
