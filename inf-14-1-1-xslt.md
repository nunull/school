# xpath

* "/" ?
* attribute: @
* belibieger node: //
* all: *
* current: .

## functions

* count()
* name()

## achsen

* preceding-sibling::
* following-sibling::

# xsl

* xsl:stylesheet
	* version="1.0"
	* xmlns:xsl="http://www.w3.org/1999/XSL/Transform"
* xsl:output
	* method="html"
	* encoding="utf-8"
	* indent="yes"
* xsl:value-of
	* select="xpath"
* xsl:template
	* attributes:
		* match="xpath"
		* name="name"
* xsl:if
	* test="xpath = ''"
* xsl:for-each
	* select="xpath"
* xsl:text
	* disable-output-escaping="yes"
* xsl:apply-templates
* xsl:call-template
	* name="name"
