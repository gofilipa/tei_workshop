[<<<Previous  ](what_is_tei.md)  [Next>>>](TEIC.md)

# What is XML?

XML, or *eXtensible Markup Language*, is not actually a language, but a framework for creating more specific markup languages. TEI evolved from XML, and XML itself evolved from SGML ("Standard Generalized Markup Language"), which was an effort to come up with a standard way of annotating documents.

As a modular, extensible XML schema, TEI is made specifically to render humanities textual data. But it carries with it many aspects and qualities that are inherent to XML and SGML. 

- First, a basic design goal of XML is to ensure that documents encoded according to its provisions can move from one hardware and software environment to another without loss of information. "eXtensible" means that you can extend, or customize it. You can create your own tags. TEI itself is an example of XML’s eXtensibility! 

Compared to HTML, a more common tagging language, XML is:
- extensible: it does not consist of a fixed set of tags;
- XML documents must be *well-formed* according to a defined syntax---tags must nest properly, that is, you must always close the last tag you opened before closing a previous one.
    >&lt;sentence>This is &lt;emphasis>bad&lt;/sentence>form.&lt;/emphasis> 

    >&lt;sentence>This is &lt;emphasis>good&lt;/emphasis>form.&lt;/sentence>
- In general, XML is more interested in the meaning of data than in its presentation. HTML, by contrast, concerns itself with how elements are laid out on the screen.

### The Hierarchy --- Problems to Come

Due to the parent-child relationship between XML and TEI, there are some issues with XML that TEI inherits. One of the most concerning ones, in my opinion, is the *hierarchical* nature of XML. Here is a quote by David Birnbaum which explains what I mean:

>XML is a way of modeling a textual document as an ordered hierarchy, or tree, so that it can be explored with computational tools. Humanities scholars use XML to represent their documents because the tree model is convenient both as a logical representation (some aspects of the inherent structure of documents are tree-like) and for programming purposes (computers can process tree representations efficiently).

[<<<Previous  ](what_is_tei.md)[Next>>>](TEIC.md)

## Sources

[Birnbaum, David J. “What is XML and Why Should Humanists Care?”](http://dh.obdurodon.org/what-is-xml.xhtml)