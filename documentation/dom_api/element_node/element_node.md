
# ELEMENT OBJECT

## Document Node Properties

- document.forms
- document.images

## Document Node Methods

- document.getElementById()
- document.querySelector()
- document.querySelectorAll()
- document.getElementsByClassName()
- document.getElementsByTagName()

# ELEMENT INTERFACE

## Instance Properties:

## attributes

**Status:** Read-only

**Value:** Named Node Map

**Syntax:** Element.attributes / Element[index].attributes

## classList

**Status:** Read-only

**Value:** DOM Token List

**Syntax:** Element.classList / Element[index].classList

## children

**Status:** Read-only

**Value:** HTML Collection

**Syntax:** Element.children / Element[index].children

## firstElementChild

**Status:** Read-only

**Value:** Element Node

**Syntax:** Element.firstElementChild / Element[index].firstElementChild

## lastElementChild

**Status:** Read-only

**Value:** Element Node

**Syntax:** Element.lastElementChild / Element[index].lastElementChild

## id

**Status:** Writable

**Value:** String

**Syntax:** Element.id / Element[index].id

## className

**Status:** Read-only

**Value:** String

**Syntax:** Element.className / Element[index].className

## tagName

**Status:** Read-only

**Value:** String

**Syntax:** Element.tagName / Element[index].tagName

## clientWidth

**Status:** Read-only

**Value:** Number

**Syntax:** Element.clientWidth / Element[index].clientWidth

## clientHeight

**Status:** Read-only

**Value:** Number

**Syntax:** Element.clientHeight / Element[index].clientHeight

## scrollWidth

**Status:** Read-only

**Value:** Number

**Syntax:** Element.scrollWidth / Element[index].scrollWidth


## scrollHeight

**Status:** Read-only

**Value:** Number

**Syntax:** Element.scrollHeight / Element[index].scrollHeight

## innerHTML

**Status:** Writable

**Value:** String

**Syntax:** Element.innerHTML / Element[index].innerHTML

## innerText

**Status:** Writable

**Value:** String

**Syntax:** Element.innerText / Element[index].innerText

## nextElementSibling

**Status:** Read-only

**Value:** String

**Syntax:** Element.nextElementSibling / Element[index].nextElementSibling

## outerHTML

**Status:** Writable

**Value:** String

**Syntax:** Element.outerHTML / Element[index].outerHTML


# INSTANCE METHODS

## append()

**Parameters:** Node

**Return Type:** Undefined

**Syntax:** Element.append(node) / Element[index].append(node)

## replaceWith()

**Parameters:** Node, Node

**Return Type:** Undefined

**Syntax:** Element.replaceWith(old node, new node) / Element[index].replaceWith(old node, new node)

## remove()

**Parameters:** Node

**Return Type:** Undefined

**Syntax:** Element.remove(node) / Element[index].remove(node)

## insertAdjacentElement()

**Parameters:** Number, Element Node

**Return Type:** Element Node

**Syntax:** Element.insertAdjacentElement() / Element[index].insertAdjacentElement()

## insertAdjacentHTML()

**Parameters:** Number, Text Node

**Return Type:** Undefined

**Syntax:** Element.insertAdjacentHTML() / Element[index].insertAdjacentHTML()

## insertAdjacentText()

**Parameters:**

**Return Type:** Undefined

**Syntax:** Element.insertAdjacentText() / Element[index].insertAdjacentText()

# getAttribute()

**Parameters:** String

**Return Type:** String/Null

**Syntax:** Element.getAttribute(attribute name) / Element[index].getAttribute(attribute name)

## setAttribute()

**Parameters:** String

**Return Type:** String/Null

**Syntax:** Element.setAttribute(attribute name) / Element[index].setAttribute(attribute name)

## removeAttribute()

**Parameters:** String

**Return Type:** Undefined

**Syntax:** Element.removeAttribute() / Element[index].removeAttribute()