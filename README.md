# HTML Cheat Sheets

## HTML Basic Elements
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<!-- ... -->`     | `<!-- -->` is strictly speaking not an HTML element. You can use it to add a comment. Text written between `<!-- and -->` is not displayed in the web browser. For example: `<!-- I am comment -->` |
| `<!DOCTYPE>`       | Defines the document type used, which is always `<!DOCTYPE html>`. is. The `<!DOCTYPE>` declaration is also not an HTML element, but rather a hint for the web browser about the HTML version in which the document was document was written.|
| `<body>...</body>` | Defines the document body with the content area of the HTML document. |
| `<br>`             | Inserts a forced line break at the noted position. The element has no end tag. |
| `<h1>...</h1> - <h6>...</h6>`| Defines a heading |
| `<hr>`             | Defines a topic change in the HTML document, e.g. to separate two different thematic contents. The element has no end tag |
| `<html>...</html>` | Defines the actual HTML document and is also the root element of the HTML document. The `<html>` tag is effectively the container for all other HTML elements. |
| `<p>...</p>`       | Defines a paragraph of text. The web browsers usually add space before and after a p element. |
| `<title>...</title>` | Defines the title of an HTML document. This element is required by every HTML document to be valid HTML. |


## Global HTML attributes
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `accesskey` | A keyboard shortcut for accessing an element: `<a href="#" accesskey="h">...</a>` |
| `class` | Specifies a class name for the element, which is commonly used in practice usually used for stylesheets: `<h1 class="intro">Important</h1>` |
| `contenteditable` | With this you define whether the content of an element may be changed (true) or not (false): `<p contenteditable="true">...</p>` |
| `contextmenu` | A context menu appears when the user interacts with it, such as a for example, a right mouse click. With contextmenu you can to customize this menu. The value must be the id of a menu element. |
| `data-*` | The attribute can be used to embed user-defined data attributes in an HTML element, e.g. to query it with getAttribute(data-...) to retrieve it. |
| `dir` | Defines the running direction of texts for the content of the HTML Element. Possible values are `ltr` (left to right), `rtl` (right to left) or auto: `<p dir="rtl">Right to left</p>` |
| `draggable` | This allows you to specify whether a user can drag an HTML element with the mouse button pressed (true) or not (false): `<p draggable="true">Warpable</p>` |
| `dropzone` | This specifies whether a dragged element should be copied or linked when dropped on the element. element should be copied (copy), moved (moved) or linked (link). Currently this attribute is not yet supported by any web browser. |
| `hidden` | If you use the stand-alone attribute, the HTML element is no longer relevant and should no longer be displayed: `<p hidden>Not visible!</p>` |
| `id` | With this you define a unique ID for an HTML element. This ID is very often used for CSS and JavaScript or to set a link to a specific HTML element on the same page. |
| `lang` | Defines the language of the HTML element's content: `<p lang="es"> ¡Buenos días!</p>` |
| `spellcheck` | This determines whether you perform a spell check on the content of the HTML element (true) or not (false): `<textarea spellcheck="true"></textarea>` |
| `style` | This allows you to set an inline CSS for an HTML element: `<h1 style="color:red">red font</h1>` |
| `tabindex` | This sets the order of HTML elements when the user presses the user presses the tab key: `<a href="#" tabindex="1">Link 1</a>` |
| `title` | This allows you to specify additional information for an HTML element which is displayed as a tooltip by many web browsers: `<a href="#" title="Weblink">Link</a>` |
| `translate` | Google Translate may be translated (yes) or not (no). Alternatively you can also specify `class="notranslate"` as fallback. |


## HTML elements for styles and semantics
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<article>...</article>` | With the article element you define an independent logical part within a web page, which should therefore be independent from the rest of the page content. Useful examples of the element would be blog articles, forum postings, or even user comments for articles. |
| `<aside>...</aside>` | You can use the aside element for marginal information about an article. This area can just as easily be a sidebar in a finished a sidebar in a finished layout. |
| `<details>...</details>` | Use the details element to show or hide additional information about a document content interactively on user request without CSS or JavaScript. |
| `<dialog>...</dialog>` | The dialog element creates a dialog box or a window and makes it easy to use HTML to display an interactive pop-up dialog or modal dialog on a dialog on a web page. |
| `<div>...</div>` | Used to split a content in a general area or section. In practice, `<div>` is often used together with CSS to design the layout of a web page. Much of what was structured with `<div>` before HTML5 is now implemented with the new elements such as `<article>`, `<aside>`, `<section>`, `<header>`. `<div>` should therefore only be used for things for which there are no suitable HTML elements. |
| `<footer>...</footer>` | Defines a footer usually at the end of a web page, article or section. It is recommended that this element contains information about the author of the document, copyright information, contact information, etc. |
| `<header>...</header>` | Defines a header area usually at the beginning of a web page, article or section. It is recommended that this element contains the heading, an introductory text or a navigation aid. |
| `<section>...</section>` | This element allows you to subdivide the content of a document or article into topic-specific or standalone content. |
| `<span>...</span>` | The element is used to group inline elements within a paragraph, for example, to style this area with CSS or manipulate it with JavaScript. |
| `<style>...</style>` | You use this to define the stylesheet information for an HTML document. If you want to use an external stylesheet file, you must use the take the standalone `<link>` tag. |
| `<summary>...</summary>` | The element defines a visible heading for the details element. In conjunction with `<details>` this heading can be clicked and expanded and collapsed. |


### HTML attribute for `<details>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `open` | This is a standalone boolean attribute, and it specifies, when used, that the details element is expanded when the page is loaded. Without using this HTML attribute, the content of the details element is collapsed by default. `<details open><summary>Copyright 2022</summary><p> - by Rick Sample.</p><p>All content and graphics ...</p></details>` |


### HTML attributes for `<style>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `media` | Specifies the media type or device for which this style is to be used. |
| `type` | Specifies the MIME type of the stylesheet language, which for CSS is `"text/css"`. In current HTML, this specification is no longer mandatory, as it was in HTML 4.01, because CSS is used as default if no other specification is made. |


### HTML elements for text markup
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<abbr>...</abbr>` | The element is used for abbreviations or acronyms. The title attribute is also often used for this element, where the meaning of the abbreviation is written out and displayed by the web browser as a tooltip when the user hovers over it. tooltip when the user hovers over it with the mouse: `<abbr title="value-added_tax">VAT.</abbr>` |
| `<address>...</address>` | This element should be used to note the contact information of the author or owner of a page or article. |
| `<b>...</b>` | With this element you can mark up a text that is to stand out from the from the usual continuous text. Usually, this text is displayed in bold. However, the b element should not be misused for formatting purposes, for which you should use CSS instead. However, you should use the b element only if no more suitable HTML element is appropriate for this text. For highlighting you should use `<em>`, for an important text `<strong>` and to mark up text `<mark>` should be preferred. |
| `<bdi>...</bdi>` | This defines an area for a bidirectional text that could be formatted in a different could be formatted in a different direction. This element is useful when a text is taken from a database or from a user input where the writing direction is not known. |
| `<bdo>...</bdo>` | This element is used to change the text direction within a continuous text. continuous text. This is very useful, for example, when you want to display a text that is written from right to left (such as Hebrew or Arabic) |
| `<blockquote>...</blockquote>` | With this you usually quote a text from another source.  |
| `<cite>...</cite>` | This element should be used since HTML5 to mark up a title of books, movies, music, exhibitions, paintings, etc. This element should not be used for people.  |
| `<code>...</code>` | Within a continuous text you use this element to draw the text as computer code. If you want to mark up multiple lines as computer code you should use the pre element. |
| `<del>...</del>` | A change marker that you use to represent text within body text as deleted and no longer valid. The counterpart to this element is `<ins>`. |
| `<dfn>...</dfn>` | You mark a text that you write down in between as a definition. You can use it, for example, to mark a defined term which you will explain in the subsequent text. |
| `<em>...<em>` | You should use this element if you want to emphasize words or passages linguistically. If, on the other hand, you only want to bring a word or passage into focus, you should use `<strong>` instead |
| `<i>...</i>` | Since HTML5, you should use this element for content specific technical terms, a thought, scientific names or foreign language words. Should only be used when no other fits. |
| `<ins>...</ins>` | A change marker that you can use to show a text as newly inserted within a continuous text as newly inserted. The counterpart to this element is `<del>`. |
| `<kbd>...</kbd>` | This element should be used to mark a letter, a word or a word or passage in the continuous text as a keyboard input. |
| `<mark>...</mark>` | This element should be used to mark words or passages in a continuous text as marked text. In practice, you could use `<mark>`, for example, to highlight a search term you have found. |
| `<pre>...</pre>` | This is used to mark up preformatted text. All whitespace characters are displayed in the web browser as they appear in the text. Usually, this text is also output in a monospace font. |
| `<q>...</q>` | Identify individual words or text passages as quoted or spoken text. text. The web browser then usually places this text between quotation marks. |
| `<ruby>`,`<rt>`,`<rp>` | Enclosing content for Ruby annotations to indicate the pronunciation of East Asian characters. |
| `<s>...</s>` | Mark a text as no longer valid or obsolete. For replaced or deleted text, you should use the del element instead. |
| `<samp>...</samp>` | You should use the element for an exemplary screen output of programs. |
| `<small>...</small>` | This allows you to mark a text as small print information, such as is used for copyright information, license information or legal notices. |
| `<strong>...</strong>` | You can use this to mark words or text passages that are particularly important in terms of content in order to give the text a special signal or warning effect. |
| `<sub>...</sub>` | This element is used to lower text. The element is often used in mathematical and chemical formulas, for example. |
| `<sup>...</sup>` | This sets the text noted in between higher. The element is also used more often in mathematical and chemical formulas formulas. |
| `<time>...</time>` | The element is used to mark up date and time information so that this information is also readable and thus usable by search engines, for example. |
| `<u>...</u>` | This allows you to underline text as proper noun underlining, such as is common in Chinese writing, or incorrect words. The text is usually underlined by the web browser. |
| `<var>...</var>` | This allows you to mark up a text as a variable or constant that is used, for example, in a mathematical expression or with an identifier of a variable in a programming language. |
| `<wbr>...</wbr>` | This defines an optional line break within a word. word. The line break only occurs at this point if it is necessary for optimal display in the web browser, so that the reader does not have to reader does not have to scroll to the right. |
