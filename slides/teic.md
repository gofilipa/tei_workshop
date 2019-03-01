[<<<Previous  ](what_is_xml.md)  [Next>>>](basic_architecture.md)

# Text Encoding Initiative Consortium

## What is the Consortium?

The Text Encodig Initiative is run by a group of people that collectively develops and maintains the standard, called the [Consortium](https://tei-c.org/). This group publishes a set of Guidelines which specify encoding methods for texts in humanities, social sciences and linguistics. 

As I said before, the structure of TEI is modular, and the guidelines are organized into 23 modules. Each module specifies a specific type of text encoding, based on the type of document you want to encode. There are also explanatory modules that explain the basic architecture and function of TEI, as well as how to implement the guidelines. They address everything from representing verse, to dictionaries, to graphs and networks. The full list of modules consist of the following: 

    1 The TEI Infrastructure
    2 The TEI Header
    3 Elements Available in All TEI Documents
    4 Default Text Structure
    5 Characters, Glyphs, and Writing Modes
    6 Verse
    7 Performance Texts
    8 Transcriptions of Speech
    9 Dictionaries
    10 Manuscript Description
    11 Representation of Primary Sources
    12 Critical Apparatus
    13 Names, Dates, People, and Places
    14 Tables, Formulæ, Graphics and Notated Music
    15 Language Corpora
    16 Linking, Segmentation, and Alignment
    17 Simple Analytic Mechanisms
    18 Feature Structures
    19 Graphs, Networks, and Trees
    20 Non-hierarchical Structures
    21 Certainty, Precision, and Responsibility
    22 Documentation Elements
    23 Using the TEI

Within each module, you will find specific guidelines and explanations for that particular type of encoding. They also provide the necessary information for customizing your own TEI schema. As you can see, the guidelines are *extensive* and present a steep learning curve for anyone who wants to fully understand the TEI framework. 

Thankfully, you don't have to know all of the guidelines to use TEI. For this workshop specifically, we will be working with a subset, *[The Represenation of Primary Sources](https://www.tei-c.org/release/doc/tei-p5-doc/en/html/PH.html)*, listed under Module 11. 

Even within this module, things can quickly get complicated. As anyone familiar with textual scholarship or editing knows, there are many approaches to the digitization and transcription of texts. A diplomatic transcription, for example, which attempts to render visual elements of manuscripts as they appear on the page, differs greatly from a critical edition, which exercises editorial intervention to create an authoritative or definitive text. Without going too much into editorial theory, suffice it to say that this module is robust enough to be used toward both kinds of projects. 

Our focus, within the Primary Source module, is on *the diplomatic transcription of manuscripts*. This means that we will focus on a relatively small subset of tags that work to identify and render manuscript elements. For an example of this kind of encoding, refer to the below image from the [Shelley-Godwin Archive](http://shelleygodwinarchive.org/). 

![frankenstein first page](https://github.com/gofilipa/tei_workshop/slide_images/frank_transcription.png)

This archive provides the digitized manuscripts of Percy Shelley, Mary Wollstonecraft Shelley, William Godwin, and Mary Wollstonecraft. The image shows  



That all being said, let’s see an image of TEI with Shelley-Godwin Archive, which shows a CUSTOMIZATION based off, AFAIK, Primary Source Encoding. 
TEI is more and more commonly used by textual scholars who work on transcribing print materials into digital formats. S-GA is an example. 
(Large-scale initiatives such as Early English Books Online (EEBO), The Women Writers Project (at Northeastern), are using the TEI as their underlying encoding model, and the major digital editions now being produced typically use TEI because it offers the most nuanced and rigorous approach to describing the complexities of the edited text currently available. 
Some understanding of text encoding in general, and of the TEI in particular, is thus becoming the equivalent of an understanding of standard editorial practices a few decades ago: helpful for anyone who works closely with texts, and essential for anyone whose research depends on a critical awareness of how scholarly sources are produced and consumed.)
Highlight some common elements: 
Elements - to define the type of content
<del>deleted text</del>
Attributes - to qualify the elements in some way
<del rend=“strikethrough”>deleted text</del>
Comments - ignored by machine, but useful for group coordination
<!— comment>
Start to introduce the hierarchy 
Tags must be nested properly. 
Technical → Theoretical
According to WWP: “The most significant concepts of text encoding, from a scholarly standpoint, are not the technical details but rather the broader ideas about modelling textual information, representational strategies, and editorial method: in fact, the same domain that has been the province of scholarly editing for centuries. What needs to be grasped is how these ideas translate into the digital medium, and what changes when they do.”
“Descriptive markup reveals what the encoder thinks to be implicit or hidden aspects of a text, and is thus an interpretive medium which often documents scholarly research next to structural information about the text” (TBE). 
“Each scholar must have the freedom of expressing their own theory of text by encoding the features they think important in the text.









[<<<Previous  ](what_is_xml.md)  [Next>>>](basic_architecture.md)