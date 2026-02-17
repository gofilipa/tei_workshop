[<<<Previous  ](elements.md)[Next>>>](next_steps.md)

# Try it yourself!

Now we are beginning the fully hands-on part of the workshop. Before getting started, you will need access to the following: 
- First, a text editor (one of your group members should download **Sublime** or **VS Code**, or you will need to borrow a laptop which has VS Code installed).
- Second, access to **the starter text**, below, which you can download or copy/paste into your text editor. 
- Third, access to a **validator**, [via this link](https://www.teibyexample.org/exist/tools/TBEvalidator.htm), where you can periodically copy and paste your code to see if it is valid, in other words, having no mistakes.
- Fourth, access to the **manuscript images** which you will be encoding, check pages 20-21.
    ![Link to the Manuscript at the Morgan Library](https://www.themorgan.org/collection/oscar-wilde/the-picture-of-dorian-gray)

## Setting up a Text Editor

If you don't already have a text editor on your computer, you should download [VS Code](https://code.visualstudio.com/download). 

Go to the home page and download the editor. Then open the package and follow the steps to install and open. 

## The Starter Text

To get you started, I'm providing you with a boilerplate starter text, containing the XML and header info at the top, as well as the basic structure of the body. That way, you can jump right into encoding the lines of the manuscript. Copy and paste the following text into your text editor, or download [this file](https://github.com/gofilipa/tei_workshop/blob/master/dorian_gray/starter_text.xml) to open it right in your text editor:

    <?xml version="1.0" encoding="UTF-8"?>
    <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/tei_all.rng" type="application/xml" schematypens="http://relaxng.org/ns/structure/1.0"?>
    <?xml-model href="http://www.tei-c.org/release/xml/tei/custom/schema/relaxng/tei_all.rng" type="application/xml"
    schematypens="http://purl.oclc.org/dsdl/schematron"?>
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
                    <p>Wilde, Oscar. "The Picture of Dorian Gray: Original Manuscript." MS. 1889. Morgan Library and Museum. New York, NY.</p>
                </sourceDesc>
            </fileDesc>
        </teiHeader>
        <sourceDoc>
            <surface>
            <line>Greek. The harmony of soul and</line>
                    <line>body---how much that is! We in</line>
                    <line>our madness have separated the two,</line>
                    <line>and have invented a realism that</line>
                    <line>is bestial, an ideality that is</line>
                    <line>void. Harry! Harry! If you only</line>
                    <line>knew what Dorian Gray is<add place="above">to me</add>! You</line>
                    <line>remember that landscape of mine, for</line>
                    <line>which Agnew offered me such <gap reason="illegible"></gap>a</line>
                    <line>
                        <gap reason="illegible"></gap>
                        <add place="above">huge</add>
                        price, but which I would
                    </line>
            </surface>
        </sourceDoc>
    </TEI>

*Keep in mind that all of your work will now fall between the last &lt;line> tag and the last &lt;surface> tag.*

[Next>>>](next_steps.md)
