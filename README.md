### trix
---
https://github.com/basecamp/trix

```
bin/setup
bin/blade build


```

```js
localStorage["editorState"] = JSON.stringify(element.editor)
element.editor.loadJSON(JSON.parse(localStorage["editorState"]))

element.editor.insertString("Hello")
element.editor.recordUndoEntry("Insert Text")

element.editor.activateAttribute("quote")
element.editor.increaseNestingLevel()
element.editor.decreaseNestingLevel()

element.editor.undo()
element.editor.redo() 

element.editor.insertString("Trix")
element.editor.setSelectedRange([0, 4])
element.editor.activateAttribute("href", "https://trix-editor.org/")

element.editor.setSelectedRange([2, 4])
element.editor.deactivateAttribute("bold")

element.editor.activateAttribute("italic")
element.editor.insertString("This is italic")

element.editor.deleteInDirection("forward")
element.editor.setSelectedRange([0, 4])
element.editor.deleteInDirection("forward")
element.editor.insertString("Hello")
element.editor.setSelectedRange([0, 5])
element.editor.activateAttribute("bold")
element.editor.setSelectedRange([1, 1])
element.editor.deleteInDirection("backward")
element.editor.setSelectedRange([1, 1])

var attachement = new Trix.Attachment({ content: '<span class="mention">@trix</span>' })
element.editor.insertAttachment(attachment)

var file = document.querySelector("input[type=file]").file
element.editor.insertFile(file)

element.editor.setSelectedRange([0, 0])
element.editor.insertHTML("<strong>Hello</strong>")

var rect = element.editor.getClientRectAtPosition(0)
[rect.left, rect.top]

element.editor.setSelectedRange([0, 0])
element.editor.insertString("Hello")

element.editor.setSelectedRange(1)
element.editor.setSelectedRange([1])
element.editor.setSelectedRange([1, 1])

element.editor.moveCursorInDirection("backward")
element.editor.expandSelectionInDirection("forward")

var document = element.editor.getDocument()
document.isEqualTo(element.editor.getDocument())

element.editor.getSelectedRange()
element.editor.setSelectedRange([0, 1])

var element = document.querySelector("trix-editor")
element.editor

element.editor.getDocument()

var document = element.editor.getDocument()
document.toString()
```

```
<trix-editor class="trix-content"></trix-editor>

<div class="trix-content"></div>
```


