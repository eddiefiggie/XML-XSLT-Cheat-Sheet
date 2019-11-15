<?xml version="1.0" encoding="utf-8" ?>
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
    <xsl:output method="html"/>

    <xsl:template match="/">

        <html>
            <head><title>Grocery List</title></head>

            <body>

                <xsl:for-each select="groceries/item">
                    <a href="#{generate-id(description)}">
                    <xsl:value-of select="description" /></a><br />
                </xsl:for-each>


                <xsl:for-each select="groceries/item">
                    <xsl:sort select="description" order="ascending" data-type="text" />
                        <h3><a description="#{generate-id(description)}">
                            <xsl:value-of select="description" />
                        </a></h3>

                        <p>Purchase <xsl:value-of select="description" /> from <xsl:value-of select="store" />.</p><br />



                </xsl:for-each>

            </body>
        </html>



    </xsl:template>

</xsl:stylesheet>
