[<<<Previous  ](preliminary.md)  [Next>>>](practice.md)

# Elements for Primary Source Encoding 

We are now going to look at some useful elements from the Primary Source Encoding module of the guidelines. These elements represent only a subset of possible elements of this module, which itself is only a subset of the TEI guidelines (the guidelines having over 500 elements total!). The elements below are selected because they are (1) commonly used in this module and (2) directly relevant to the kind of encoding we will be doing today. They are the following: 
    
    <sourceDoc>

    In primary source encoding, this element is equivalent to the "body" tag in HTML. It encloses the entire second half of the document, and begins after the end tag of the <teiHeader>. The document, therefore, should be structured like this:

        <?xml>
        <TEI>
            <teiHeader>
                <...>       ### header
            </teiHeader>
            <sourceDoc>
                <...>       ### body
            </sourceDoc>
        </TEI>
    
    <surface>

    This is another element that encloses the main body of the document, nested just under the <sourceDoc> element. The document, therefore, should look like this:
        
        <?xml>
        <TEI>
            <teiHeader>
                <...>          ### header
            </teiHeader>
            <sourceDoc>
                <surface>
                    <...>       ### the rest of your encoding will go in this section
                </surface>
            </sourceDoc>
        </TEI>

Now we have the basic structure of a primary source document in place. We can now turn to the individual lines of the document, and encode it line by line. 
    
    <line>

    This indicates that a new line has begun in the manuscript. For a diplomatic transcription, you need to enclose each line with the <line></line> tags, otherwise the line will continuously run across the page. 
    
    <add> and <del>

    Words or phrases that have been added or deleted in the source text may be recorded using <add> and <del>. Information about the actual rendition of the additions and deletions can be provided in the @rend attribute, such as a strikethrough. Additionally, the place of the addition may also be recorded using the @place attribute, such as “above” or “below”, which would display the text either above or below the current line. 

    While the @rend attribute can be used to record general visual aspects, the <add> element has a specific @place attribute, for indicating where the addition is located. The <del> element cannot use the @place attribute. If you need to use the @place attribute, encode with the <add> element, and combine with @rend set to the value "strikethrough".

        Example:

        <add>added text goes here.</add>
        <add place="above">this text will appear above the current line.</add>
        <del rend="strikethrough">deleted text, with a strikethrough, goes here.</del>

    <mod>

    Additions and deletions with a causal relationship may be grouped by the <mod> element. This is only necessary if more than one action (adding or deleting) affects the same piece of text, such as a deletion that was then replaced with an addition. 

        Example: 

        <mod>
            <del>deleted text</del>
            <add>added text</add>
        </mod>

    <gap>

    Where areas in the copy text cannot be read with confidence, <gap> should be used with the @reason attribute indicating that the difficulty of transcription is due to illegibility. In those cases where you cannot read the text, you may encode with the following (leaving no space or text between the tags): 

        <gap reason="illegible"></unclear>


## Putting it all together

Here is an example of how some of the above elements might look in your TEI document.
        
    <line>This is the 
        <mod>
            <del rend="strikethrough">wrong</del>
            <add place="superlinear">right</add>
        </mod>
    way to encode with TEI.
    </line>

[<<<Previous  ](preliminary.md)  [Next>>>](practice.md)