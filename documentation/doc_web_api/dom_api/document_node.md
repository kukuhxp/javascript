# DOCUMENT INTERFACE		

# CONSTRUCTOR

## Document()

# INSTANCE CLASS

## document

# INSTANCE PROPERTIES

## all

**Status:** Writable

**Value:** HTML Collection

**Syntax:** document.all


## cookie

**Status:** Writable

**Value:** String

**Syntax:** document.cookie

## domain

**Status:** Writable

**Value:** String

**Syntax:** document.domain

## documentURl

**Status:** Read-only

**Value:** String

**Syntax:** document.documentURl


## URL

**Status:** Read-only

**Value:** String

**Syntax:** document.URL

## head

**Status:** Read-only

**Value:** Element Node

**Syntax:** document.head

## title

**Status:** Writable

**Return Type:** String

**Value:** Title of Document

**Syntax:** document.title

## body

**Status:** Writable

**Return Type:** Element Node

**Value:** Body Element

**Syntax:** document.body

## forms

**Status:** Read-only

**Return Type:** HTML Collection

**Value:** Form Element Collection

**Syntax:** document.forms

## images

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.images

## links

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.links

## embeds

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.embeds

## plugins

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.plugins

## scripts

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.scripts

## fonts

**Status:** Read-only

**Value:** Interface (FontFaceSet)

**Part of:** CSS Font Loading API

**Syntax:** document.fonts

## children

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** document.children

## firstChildElement

**Status:** Read-only

**Value:** Element Node

**Syntax:** document.firstChildElement

## lastChildElement

**Status:** Read-only

**Value:** Element Node

**Syntax:** document.lastChildElement

## implementation

**Status:** Read-only

**Value:** Interface (DOMImplementation)

**Syntax:** document.implementation

## documentElement

**Status:** Read-only

**Value:** Interface (Element Node)

**Syntax:** document.documentElement

## scrollingElement

**Status:** Read-only

**Value:** Interface (Element Node)

**Syntax:** document.scrollingElement


# INSTANCE METHODS

## createElement()

**Parameters:** String, Object

**Return Type:** Element Node

**Syntax:** document.createElement(element name)

**Example:** document.createElement("p")

## createAttribute()

**Parameters:** String, Object

**Return Type:** Attribute Node (Attr)

**Syntax:** document.createAttribute(attribute name)

**Example:** document.createAttribute("src")

## createTextNode()

**Parameters:** String, Object

**Return Type:** Text Node

**Syntax:** document.createTextNode(text)

**Example:** document.createTextNode("JavaScript")

## createComment()

**Parameters:** String, Object

**Return Type:** Comment Node

**Syntax:** document.createComment(data)

**Example:** document.createComment("This is a comment section")

## createDocumentFragment()

**Parameters:** None

**Return Type:** Document Fragment Node

**Syntax:** document.createDocumentFragment() / new DocumentFragment()

## getElementById()

**Parameters:** String, Object

**Return Type:** Element Node

**Syntax:** document.getElementById(id name)

**Example:** document.getElementById("my-id")

## getElementsByClassName()

**Parameters:** String, Object

**Return Type:** HTML Collection

**Syntax:** document.getElementsByClassName(class name)

**Example:** document.getElementsByClassName("my-class")

## getElementsByTagName()

**Parameters:** String, Object

**Return Type:** HTML Collection

**Syntax:** document.getElementsByTagName(tag name)

**Example:** document.getElementsByTagName("button")

## getElementsByName()

**Parameters:** String, Object

**Return Type:** Node List

**Syntax:** document.getElementsByName(name attribute)

## querySelector()

**Parameters:** String, Object

**Return Type:** Element Node

**Syntax:** document.querySelector(css selector)

**Example:** document.querySelector(".my-class")

## querySelectorAll()

**Parameters:** String, Object

**Return Type:** Node List

**Syntax:** document.querySelectorAll(css selector)

**Example:** document.querySelectorAll(".my-class")

## importNode()

**Parameters:** Node, DocumentFragment, Boolean

**Return Type:** Node

**Syntax:** document.querySelector(external node, deep)

## getSelection()

**Parameters:** None

**Return Type:** Object/Null

**Syntax:** document.getSelection()

## elementsFromPoint()

**Parameters:** Number

**Return Type:** Array

**Syntax:** document.elementsFromPoint()

## hasFocus()

**Parameters:** None

**Return Type:** Boolean

**Syntax:** document.hasFocus()

## open()

**Parameters:** None

**Return Type:** Document Node

**Syntax:** document.open()

## write()

**Parameters:** String, Object

**Return Type:** Undefined

**Syntax:** document.write(object)

**Example:** document.write("Hello world")

## writeln()

**Parameters:** String, Object

**Return Type:** Undefined

**Syntax:** document.writeln(object)

**Example:** document.writeln("Hello world")

## close()

**Parameters:** None

**Return Type:** Undefined

**Syntax:** document.close()