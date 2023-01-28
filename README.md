# HTML_Cheat_Sheets

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
| `open` | This is a standalone boolean attribute, and it specifies, when used, that the details element is expanded when the page is loaded. Without using this HTML attribute, the content of the details element is collapsed by default. 
`<details open>`
 `<summary>Copyright 2022</summary>`
 `<p> - by Rick Sample.</p>`
 `<p>All content and graphics ...</p>`
`</details>` |
