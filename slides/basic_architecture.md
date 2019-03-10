[<<<Previous  ](modules.md)  [Next>>>](preliminary.md)

# Basic Architecture

In this next section, I'm going to review all of the necessary components to create a TEI document. A lot of this information will be overwhelming for beginners, so it's important to emphasize that you *don't need to know all of it*. These guidelines will stay right here (and much more is easily available through a google search) for you to refer to as you work through your encoding. Even experienced TEI encoders often refer to the guidelines or a web search to refresh certain rules and concepts. 

The most important takeaway from this page--which you *do* need to understand--is the dual structure of the TEI document, that includes a header section and a body section. Let's jump into the header.

## The Head

Like HTML, every TEI document consists of a two parts, a head and a body. We will begin with the head, which describes the source text's metadata, and go through each element in the head one by one. 

Under the DTD declaration, the first line of any TEI document contains the **&lt;TEI>** element itself, which contains an attribute that points to a *namespace*. This namespace is simply used to make sure there are no errors in processing the element names. Accordingly, the TEI element looks like the following:

    <TEI xmlns="http://www.tei-c.org/ns/1.0">

Including this **&lt;TEI>** element, the first four elements which make up most of the header are the following, nested from outer to inner element: 

**&lt;TEI>** -- declaries the document is a TEI document, and nests the entire document\
**&lt;teiHeader>** -- nests the header section \
**&lt;fileDesc>** -- nests the "file description" section \
**&lt;titleStmt>** -- nests the title of the source \
**&lt;title>** -- contains the title of the source

As you might have guessed, each of these opening tags is followed by an end tag. The TEI element, being the most outer tag, encloses all the text on the document. It's end tag looks like this: **&lt;/TEI>**

Like the title elements, the next two elements are also nested by the fileDesc. These are the publication and source info.

**&lt;publicationStmt>** -- nests information concerning the publication or distribution of a source text.\
**&lt;sourceDesc>** -- describes where the source text was derived or generated, typically a bibliographic statement.

Though this might seem like a lot, there are many *more* elements that you could include in the header to describe metadata about the source text. The ones above are only the *minimum* required by the TEI schema. All together, properly nested and populated, the header should look soemthing like this:


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

This is a lot of information for now--but don't worry! For our class exercise, you don't need to work with the header at all. Your encoding work will be focusing solely on the body section. So, if the header is TMI for now, you can always come back to it later. 

## The Body

The body section is the second half of a TEI document, and it forms the main section of the document. When a TEI document is transformed, all you will see is the body section. It is important to remember that this section, *along with the header*, is enclosed by the TEI tags.

The header section ends with a TEI header end tag: **&lt;/teiHeader>**. The body section begins with a **&lt;sourceDoc>**. This tag will enclose the entirety of the body, and is nested within the **&lt;TEI>** tag, which encloses the whole document, including the header. these outer tags for the head and body, therefore, look like this:

    <TEI> # this opens the TEI document
        <teiHeader> # this opens the head
            <...> # header info goes in here
        </teiHeader> # this closes the head
        <sourceDoc> # this opens the body
            <...> # body info goes in here
        </sourceDoc> # this closes the body
    </TEI> # this closes the TEI document

For our purposes, you might think of the **&lt;sourceDoc>** element a "body" tag in HTML. It functions in just the same way. 

Besides **&lt;sourceDoc>**, we will also be using the **&lt;surface>**, which is nested inside the **&lt;sourceDoc>** element. The **&lt;surface>** element defines a *written surface* as a two-dimensional coordinate space. Basically, it creates a plane where you can then pinpoint specific coordinates for written elements to appear, kind of like making a literal map of the textual surface. That being said, you don't need to use the coordinate function (though it can be beneficial). You can simply indicate that a surface exists, and move on to transcribing the elements within that surface. 

## Problems Arise!

By now, you will have seen that the basic structure of TEI is hierarchical. Elements are nested within elements, and without this proper form, the code won't process properly. 

But there is another sense to TEI's hierarchy. The constraints of parent elements will determine the usage and properties of their child elements. The result is that some aspects that one might want to encode, like gender, for example, struggle against rigid requirements of TEI's hierarchy (where gender is contained within the **&lt;person>** element). 

This became an issue for a group of people who were digitizing the memoir of Lili Elbe (also known as *The Danish Girl*), one of the first people to go through gender affirmation surgery. In the memoir, the speaker (which can be indicated with the **&lt;person>** element), inhabits a variety of gender expressions as they go through their transition. The issue was that the TEI wouldn't allow the editors to ascribe multiple or shifting gender identities to a single person, let alone multiple gender personalities within one speaking entity. The hierarchical structure of TEI simply does not allow it. The encoders explain:

> The deeper we got into mark-up, the more evident it became that the categories and hierarchies available to us were inadequate for our task. We not only had to deal with the occasional difference in gender attribution across the editions, but we also had to identify a male subject who at times presents himself as masquerading as a woman, at others as being inhabited by one, and who eventually becomes a woman, in a life history narrated retrospectively from the perspective of Lili Elbe. (Caughie et al. 3)

On the one hand, it's frustrating to come up againt such obstacles in research, especially when they create what appears to be an impasse in the encoding work, and TEI is to blame. On the other hand, by creating such difficult situations, TEI itself can be seen as a tool for revealing (without resolving) complex textual data. In that case, it can be very useful, even if it's not practical. 

This closes the overview portion of the workshop. In the next section, we are going to begin the hands-on tutorial, staritng with a group brainstorm on our goals for encoding. After that, I will demonstrate you might implement the guidelines, using the manuscript of Dorian Gray as our source text.

[<<<Previous  ](modules.md)  [Next>>>](preliminary.md)