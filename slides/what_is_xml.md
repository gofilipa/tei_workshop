[<<<Previous  ](what_is_tei.md)  [Next>>>](modules.md)

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

## XML declaration

Every TEI document begins with an XML declaration, which specifies the *type* of document as well as how a computer might *process* that document, validating it against your chosen schema, in this case, a TEI schema. This is formally known as the *DTD*, or *Document Type Definition*. For the purposes of this workshop, you don't need to know exactly what this complicated code says, but you do need to know that it's necessary for the computer to know how to process the TEI. You might think of this code as the section of the document that establishes and specifies the relationship between TEI and its parent language, XML.

    <?xml version="1.0" encoding="UTF-8"?>
    <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/tei_all.rng" type="application/xml" schematypens="http://relaxng.org/ns/structure/1.0"?>
    <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/tei_all.rng" type="application/xml"
        schematypens="http://purl.oclc.org/dsdl/schematron"?>

## The Hierarchy - Problems to Come!

Due to the parent-child relationship between XML and TEI, there are some issues with XML that TEI inherits. One of the most concerning ones, in my opinion, is the *hierarchical* nature of XML. Here is a quote by David Birnbaum which explains what I mean:

>XML is a way of modeling a textual document as an ordered hierarchy, or tree, so that it can be explored with computational tools. Humanities scholars use XML to represent their documents because the tree model is convenient both as a logical representation (some aspects of the inherent structure of documents are tree-like) and for programming purposes (computers can process tree representations efficiently).

This tree structure inherent in each XML document poses problems for data that does not readily fit into a hierarchical scheme. For example, .... 

[<<<Previous  ](what_is_tei.md)[Next>>>](modules.md)