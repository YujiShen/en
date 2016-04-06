+++
date = "2016-08-14T16:11:58+05:30"
title = "Testing Note 3"
draft = "true"
+++


Currently five cell types are supported:

1. A "Text Cell" lets you edit rich-text in-place. It supports images and links too.
2. A "Code Cell" packs the awesome ACE code editor, with syntax highlighting support for 120+ languages, 20+ themes, automatic indent and outdent, code completion, and much more.
3. A "Markdown Cell" lets you write in Markdown with inline formatting and custom CSS options.
4. A "LaTeX Cell” uses MathJax to typeset mathematical equations in your notes.
5. A “Diagram Cell” lets you create sequence diagrams and flowcharts from text.
<!--more-->
### Text Cell

This is a **text cell** with *some* simple* formatting*.

This is *an example* of a text cell with complex styles applied.

You can change text formatting using the toolbar at the top, or with keyboard shortcuts. Look under the “`Format`” menu for all the formatting options and keyboard shortcuts.

### Code Cell

```js
// This is a code cell set to the JavaScript mode

void hello()
{
    console.log("Hello World!");
}
```

```css
/* Placeholder for custom user CSS mainly to be overridden in profile/static/custom/custom.css This will always be an empty file in IPython */
/* comment out this line to bring the toolbar back */
 html, body {
   overflow-y: hidden 
}
 div#header {
   background-color: #fdf6e3;
}
 div#site {
   margin:0;
   padding:0;
   border-width: 0;
}
 div#maintoolbar, div#header-container{
   display: none !important;
}
 div#notebook-container {
   padding-left: 5px;
   width: 1070px;
   background-color: #fdf6e3;
}
 div.navbar-collapse {
   background-color: #fdf6e3;
}
 div#notebook {
   border-top: none;
}
 div.input {
   width: 135ex;
}
 div.input_area {
   border: 2px ridge #93a1a1;
}
 div.output_subarea {
  /*margin-left:40px;
  */
   max-width: 123ex;
}
 div.output_area pre {
   font-size: 15px;
  /*font-family: consolas;
  */
   word-break:normal !important;
}
 div.text_cell {
   width: 135ex;
}
 div.text_cell_render {
   font-size: 16px;
   line-height: 145%;
}
 .rendered_html pre, .rendered_html code {
   background-color: #E6E6E6;
}
 .CodeMirror {
   font-size: 15px;
   font-family: monacob, monospace;
   line-height: 145%;
}
/* Style for syntax highlighting*/
 .cm-s-ipython.CodeMirror {
  background: #fdf6e3;
   color: #073642;
}
 .cm-s-ipython div.CodeMirror-selected {
  background: #073642 !important;
}
 .cm-s-ipython .CodeMirror-gutters {
  background: #fdf6e3;
   border-right: 1px solid #93A1A1;
   padding-right:5px;
}
 .cm-s-ipython .CodeMirror-linenumber {
  color: #93A1A1;
}
 .cm-s-ipython .CodeMirror-cursor {
  border-left: 1px solid #657b83 !important;
}
 .CodeMirror pre {
  color: #586E75;
}
 .cm-s-ipython span.cm-comment {
  color: #93A1A1;
}
 .cm-s-ipython span.cm-atom {
  color: #6c71c4;
}
 .cm-s-ipython span.cm-number {
  color: #D33682;
}
 .cm-s-ipython span.cm-meta {
  color: #268bd2;
}
 .cm-s-ipython span.cm-property, .cm-s-ipython span.cm-attribute {
  color: #859900;
}
 .cm-s-ipython span.cm-keyword {
  color: #748B00;
}
 .cm-s-ipython span.cm-string {
  color: #2AA198;
}
 .cm-s-ipython span.cm-operator {
  color: #859900;
}
 .cm-s-ipython span.cm-builtin {
  color: #B58900;
}
 .cm-s-ipython span.cm-variable {
  color: #586E75;
}
 .cm-s-ipython span.cm-variable-2 {
  color: #268bd2;
}
 .cm-s-ipython span.cm-def {
  color: #268BD2;
}
 .cm-s-ipython span.cm-error {
  background: #dc322f;
   color: #ffffff;
}
 .cm-s-ipython span.cm-bracket {
  color: #586e75;
}
 .cm-s-ipython span.cm-tag {
  color: #dc322f;
}
 .cm-s-ipython span.cm-link {
  color: #6c71c4;
}
 .cm-s-ipython .CodeMirror-matchingbracket {
   text-decoration: underline;
   color: #073642 !important;
}


```

```python
@decorator(param=1)
def f(x):
    """ Syntax Highlighting Demo
        @param x Parameter"""
    s = ("Test", 2+3, {'a': 'b'}, x)   # Comment
    print s[0].lower()

class Foo:
    def __init__(self):
        byte_string = 'newline:\n also newline:\x0a'
        text_string = u"Cyrillic Я is \u042f. Oops: \u042g"
        self.makeSense(whatever=1)
    
    def makeSense(self, whatever):
        self.sense = whatever

x = len('abc')
print(f.__doc__)
```

Code cells support syntax highlighting for 120+ languages, 20+ themes, automatic indent and outdent, code folding, multiple cursors and selections, code completion, tab triggers, Vim/Emacs keybinding, etc. You can read more about the awesome Ace editor on its website (<http://ace.c9.io/>).

### Markdown Cell

Markdown cells support standard Markdown syntax as well as GitHub Flavored Markdown (GFM). Open the preview to see these rendered.

### Basics 好吧。。。这个字体怎么这么扁呢？
我勒个去啊。。。

# H1
## H2
### H3
#### H4
##### H5
###### H6

---

*italic*, **bold**, ~~Scratch this.~~

Test how this incline Code interact with `inline code`

```python
@decorator(param=1)
def f(x):
    """ Syntax Highlighting Demo
        @param x Parameter"""
    s = ("Test", 2+3, {'a': 'b'}, x)   # Comment
    print s[0].lower()

class Foo:
    def __init__(self):
        byte_string = 'newline:\n also newline:\x0a'
        text_string = u"Cyrillic Я is \u042f. Oops: \u042g"
        self.makeSense(whatever=1)
    
    def makeSense(self, whatever):
        self.sense = whatever

x = len('abc')
print(f.__doc__)
```

### Lists

1. First ordered list item
2. Another item
  * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

### Quote
I want to test the margin of top and bottom of Quote.

> Peace cannot be kept by force; it can only be achieved by understanding. Peace cannot be kept by force; it can only be achieved by understanding.

I want to test the margin of top and bottom of Quote.
### Links

[I'm an inline-style link](https://www.google.com)
http://example.com

You can also create a link to another note: (Note menu -> Copy Note Link -> Paste)
[01 - Getting Started](quiver:///notes/D2A1CC36-CC97-4701-A895-EFC98EF47026)

### Tables

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

### GFM Task Lists

- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed


Name    | Age
--------|------
Bob     | 27
Alice   | 23


### Inline LaTeX

You can use inline LaTeX inside Markdown cells as well, for example, $x^2$.

### LaTeX Cell

LaTeX cells make it easy to typeset math equations. For example,

\begin{align}
  \nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} & = \frac{4\pi}{c}\vec{\mathbf{j}} \\\nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\\nabla \cdot \vec{\mathbf{B}} & = 0
\end{align}

Open the preview to see how it's rendered.

Inline LaTeX is also supported, for example, $x^2$.

You can also add custom macros in Preferences, and they will be available in all LaTeX cells.

### Diagram Cell

Diagram cells let you create sequence diagrams and flowcharts from text.

Please check the syntax here:

* Sequence diagram: <http://bramp.github.io/js-sequence-diagrams/>
* Flowchart: <http://flowchart.js.org/>

Open the preview to see how the following examples are rendered.

Sequence diagram example:

```java
package queues;
//import edu.princeton.cs.introcs.*;

import java.util.Iterator;
import java.util.NoSuchElementException;

public class Deque<Item> implements Iterable<Item> {
    private Node first;
    private Node last = null;
    private int size;

    private class Node {
        private Item item;
        private Node next;
        private Node pre;

        public Item getItem() {
            return item;
        }
        public Node getNext() {
            return next;
        }
        public Node getPre() {
            return pre;
        }
    }

    // construct an empty deque
    public Deque() {
        size = 0;
    }

    // is the deque empty?
    public boolean isEmpty() {
        return first == null;
    }

    // return the number of items on the deque
    public int size() {
        return size;
    }

    // add the item to the front
    public void addFirst(Item item) {
        if (item == null) {
            throw new NullPointerException("Should not add null item.");
        }
        Node oldfirst = first;
        first = new Node();
        first.item = item;
        first.next = oldfirst;
        first.pre = null;
        size++;
        if (size == 1) {
            last = first;
        } else {
            oldfirst.pre = first;
        }
    }

    // add the item to the end
    public void addLast(Item item) {
        if (item == null) {
            throw new NullPointerException("Should not add null item.");
        }
        Node oldlast = last;
        last = new Node();
        last.item = item;
        last.next = null;
        last.pre = oldlast;
        size++;
        if (size == 1) {
            first = last;
        } else {
            oldlast.next = last;
        }
    }

    // remove and return the item from the front
    public Item removeFirst() {
        if (isEmpty()) {
            throw new NoSuchElementException("Deque is empty.");
        }
        size--;
        Item item = first.item;
        if (size == 0) {
            first = null;
            last = null;
        } else {
            first = first.next;
            first.pre = null;
        }
        return item;
    }

    // remove and return the item from the end
    public Item removeLast() {
        if (isEmpty()) {
            throw new NoSuchElementException("Deque is empty.");
        }
        size--;
        Item item = last.item;
        if (size == 0) {
            first = null;
            last = null;
        } else {
            last = last.pre;
            last.next = null;
        }
        return item;
    }

    // return an iterator over items in order from front to end
    public Iterator<Item> iterator() {
        return new DequeIterator();
    }

    private class DequeIterator implements Iterator<Item> {
        private Node current = first;

        public boolean hasNext() {
            return current != null;
        }

        public void remove() {
            throw new UnsupportedOperationException("Remove() is not supported.");
        }

        public Item next() {
            if (!hasNext()) {
                throw new NoSuchElementException("There is no next element.");
            }
            Item item = current.item;
            current = current.next;
            return item;
        }
    }

    // unit testing
    public static void main(String[] args) {
        Deque<Object> deque = new Deque<Object>();
        StdOut.println(deque.isEmpty());
        deque.addLast(1);
        deque.addFirst("s");
        deque.removeLast();
        //deque.removeFirst();
        deque.addFirst(1.2);
        for (Object s : deque)
            StdOut.println(s);
        StdOut.println(deque.isEmpty());
    }
}
```

Flowchart example:

```markup
st=>start: Start:>http://www.google.com[blank]
e=>end:>http://www.google.com
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes
or No?:>http://www.google.com
io=>inputoutput: catch something...

st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
```
{{% latex %}}

