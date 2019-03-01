[<<<Previous  ](modules.md)  [Next>>>](primary_source_encoding.md)

# Basic Architecture

## The Head

Like HTML, every TEI document consists of a two parts, a head and a body. Let's start with the head, which describes the source text's metadata, and go through each element in the head one by one. 

The first four elements in the header are the following, nested from outer to inner element: 

**&lt;TEI>** -- declaries the document is a TEI document, and nests the entire document\
**&lt;teiHeader>** -- nests the header section \
**&lt;fileDesc>** -- nests the "file description" section \
**&lt;titleStmt>** -- nests the title of the source \
**&lt;title>** -- contains the title of the source

As you might have guessed, each of these opening tags is followed by an end tag. The TEI element, being the most outer tag, encloses all the text on the document. It's end tag looks like this: **&lt;/TEI>**

Like the title elements, the next two elements are also nested by the fileDesc. These are the publication and source info.

**&lt;publicationStmt>** -- nests information concerning the publication or distribution of a source text.
**&lt;sourceDesc>** -- describes where the source text was derived or generated, typically a bibliographic statement.

Though this might seem like a lot, there are many more elements that you could include in the header to describe metadata about the source text. The ones above are only the *minimum* required by the TEI schema. All together, properly nested and populated, the header should look soemthing like this:


    <TEI xmlns="http://www.tei-c.org/ns/1.0">
    <teiHeader>
        <fileDesc>
            <titleStmt>
                <title>The Picture of Dorian Gray: Original Manuscript</title>
            </titleStmt>
            <publicationStmt>
                <p>Unpublished manuscript</p>
            </publicationStmt>
            <sourceDesc>
                <p>Wilde, Oscar. "The Picture of Dorian Gray: Original Manuscript." MS. 1889. Morgan Library & Museum. New York, NY.</p>
            </sourceDesc>
        </fileDesc>
    </teiHeader>

Other potentially useful tags for the TEI head include: 
**&lt;revisionDesc>** -- summarizes the revision history for a file.
**&lt;changeDesc>** -- groups a number of change descriptions associated with either the creation of a source text or its revision history. Each encoded change is nested by the **&lt;change>** element. 

From another module, the Manuscript Description module, we might be interested in adding an element that describes the identities of the writers in the document. This general tag, **&lt;handDesc> is then paired with a more practical tag, **&lt;handShift> which is used in the areas of the document where the identitity of the writer, or "hand", has changed. 

**&lt;handDesc>** -- contains a description of all the different hands used in a manuscript or other object.
**&lt;handShift>** -- marks the beginning of a sequence of text written in a new hand, or the beginning of a scribal stint.

This is a lot of information for now--but don't worry! For our class exercise, you don't need to work with the header at all. Your encoding work will be focusing solely on the body section. So, if the header is TMI for now, you can always come back to it later. 

## The Body

In the body section, we will be discussing two elements that are relevent to our project, and one element that is 
**&lt;sourceDoc>** \
**&lt;surface>**

<!---
The <surface> has an xml:id attribute. On the <div> element in the transcription we have added a facs attribute. The value of the facs attribute is a url. The value '#graves1938-10-10-1' points to the element with xml:id attribute 'graves1938-10-10-1', that is, the <surface> element. The <surface> element contains the <graphic> element that is an image of the current page. The reason we do this is that we have now explicitly defined the relation between the transcription and the corresponding image files. Later users of the transcription will know what belongs together. What may be more important: applications that want to render the transcription will no longer need to know about the names of the image files. They can just fetch the files that are needed from the location as it is specified in the Guidelines.
<listPerson>
The participant description in the TEI header, <particDesc>, can contain a list of persons (a <listPerson> element containing <person>s). For each <person> we could give a structured description in terms of a number of characteristics (sex, age, etc). But we can also limit ourselves to an informal description using a <p> element.
Whenever a specific person occurs, we can then refer to the description of that person in the header. The element that we will use to refer to the description is the <rs> element. The <rs> element (referring string) is somewhat like a name element, but more generic: names are referring strings, but so are 'her oldest son' or 'the gardener'.
DTD
“If you're using a particular markup language, how do you make sure you use only the proper element and attribute names, properly nested? You validate your XML document against a schema, which contains the the grammar (and vocabulary) for that particular markup language. There a few different formats for schemas, the most well-known of which in the world of documents (as opposed to data) is a DTD (Document Type Definition).” (Hawkins, “Introduction to XML for Text”)



>
