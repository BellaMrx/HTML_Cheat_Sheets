# HTML Cheat Sheets

All HTML5 elements and their attributes.

Detailed information about HTML can be found here - [HTML Guide](https://github.com/BellaMrx/HTML_Guide) - Detailed guide about HTML5 (all basics for HTML) + templates.


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


### Global HTML attributes
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `accesskey` | A keyboard shortcut for accessing an element: `<a href="#" accesskey="h">...</a>` |
| `class` | Specifies a class name for the element, which is commonly used in practice usually used for stylesheets: `<h1 class="intro">Important</h1>` |
| `contenteditable` | With this you define whether the content of an element may be changed (true) or not (false): `<p contenteditable="true">...</p>` |
| `contextmenu` | A context menu appears when the user interacts with it, such as a for example, a right mouse click. With contextmenu you can to customize this menu. The value must be the id of a menu element. |
| `data-*` | The attribute can be used to embed user-defined data attributes in an HTML element, e.g. to query it with getAttribute(data-...) to retrieve it. |
| `dir` | Defines the running direction of texts for the content of the HTML Element. Possible values are `ltr` (left to right), `rtl` (right to left) or auto: `<p dir="rtl">Right to left</p>` |
| `draggable` | This allows you to specify whether a user can drag an HTML element with the mouse button pressed (true) or not (false): `<p draggable="true">Warpable</p>` |
| `dropzone` | This specifies whether a dragged element should be copied or linked when dropped on the element. element should be copied, moved or linked. Currently this attribute is not yet supported by any web browser. |
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


## HTML elements for text markup
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<abbr>...</abbr>` | The element is used for abbreviations or acronyms. The title attribute is also often used for this element, where the meaning of the abbreviation is written out and displayed by the web browser as a tooltip when the user hovers over it: `<abbr title="value-added_tax">VAT.</abbr>` |
| `<address>...</address>` | This element should be used to note the contact information of the author or owner of a page or article. |
| `<b>...</b>` | With this element you can mark up a text that is to stand out from the from the usual continuous text. Usually, this text is displayed in bold. However, the b element should not be misused for formatting purposes, for which you should use CSS instead. However, you should use the b element only if no more suitable HTML element is appropriate for this text. For highlighting you should use `<em>`, for an important text `<strong>` and to mark up text `<mark>` should be preferred. |
| `<bdi>...</bdi>` | This defines an area for a bidirectional text that could be formatted in a different could be formatted in a different direction. This element is useful when a text is taken from a database or from a user input where the writing direction is not known. |
| `<bdo>...</bdo>` | This element is used to change the text direction within a continuous text. This is very useful, for example, when you want to display a text that is written from right to left (such as Hebrew or Arabic) |
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
| `<q>...</q>` | Identify individual words or text passages as quoted or spoken text. The web browser then usually places this text between quotation marks. |
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
| `<wbr>...</wbr>` | This defines an optional line break within a word. The line break only occurs at this point if it is necessary for optimal display in the web browser, so that the reader does not have to reader does not have to scroll to the right. |


### HTML attribute for `<bdo>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `dir` | This global attribute must be used by the bdo element to specify the to specify the direction. The following two values are allowed are allowed:  `dir="rtl"`: right to left, `dir="ltr"`: left to right |


### HTML attribute for `<blockquote>` and `<q>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `cite` | This allows you to specify the URL to the source from which the citation originated. For books, you can also include a link to the corresponding book page or to a web store where the book can be purchased. |


### HTML attributes for `<del>` and `<ins>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `cite` | This allows you to specify the URL to a source that contains the reason for this change marker. |
| `datetime` | This allows you to specify the date and time of the change (e.g.: YYYY-MM-DDThh:mm:ssTZD). |


### HTML attribute for `<time>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `datetime` | With this you make a machine readable date and time specification. |


## Form and input elements
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<button>...</button>` | With this you define a button similar to `<input type= "submit">`, except that you can include additional graphics and use other use other HTML elements. |
| `<datalist>...</datalist>` | This defines a predefined list of options for a single-line text field for an input element. The datalist element uses autocompletion, where the user sees a kind of dropdown list of predefined values. Using the listAttribute in the input element, the element is linked to a datalistElement. You define the individual options of the list using the option element and value attribute. |
| `<fieldset>...</fieldset>` | With the fieldset element you can combine several form elements like input fields into a logical group. Many web browsers additionally frame this area visually. You can also use the legend element to define a heading for this group. |
| `<form>...</form>` | Use this element to define the HTML forms in the HTML document. |
| `<input>` | With this you define an input field into which the user can enter different types of data. What kind of data this is and how the input element is represented depends on the typeAttribute used. |
| `<label>...</label>` | Marks a text as a simple text label in the form. Using attribute, you can associate the text label with an input element and thus have a label set for an input field. |
| `<legend>...</legend>` | Use the legend element to specify a heading for a fieldset group. |
| `<meter>...</meter>` | This element is used to visualize a certain magnitude of scalar values with a state indicator and with the help of various HTML attributes. |
| `<optgroup>...</optgroup>` | This allows you to define suboptions grouped in an extensive select selection list. |
| `<option>...</option>` | This is used to define the individual entries of a select selection list, from which the user can choose. |
| `<output>...</output>` | The output element specifies an output area for the result of calculations. This makes the output element the counterpart of the input element, so to speak. |
| `<progress>...</progress>` | This allows you to visualize a progress bar or a history for a task such as a questionnaire or a download. For a dynamic progress indicator, you need a scripting language such as JavaScript. |
| `<select>...</select>` | This allows you to define a selection list with fixed entries in a form from which the user can select an entry. An entry in the list, on the other hand, you define within the select element with the option element. |
| `<textarea>...</textarea>` | Use this element to create a multiline text input field. |


### HTML attributes for `<form>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `accept-charset` | This is used to specify the character set for the form data. Common values are UTF-8 for Unicode or ISO-8859-1 for Latin. In theory, however, you can use any character set. However, no web browser can handle all character sets. Therefore, to be on the safe side always use a widely used character set (such as UTF-8). |
| `action` | With this you specify the URL or path to a file that is called with a submit button when submitting. Often, this is a (PHP) script that evaluates the entered form data evaluates. |
| `autocomplete` | This allows you to enable autocompletion with the value `on` (= default value) and disable it with the value `off`. |
| `enctype` | Defines how the data should be encoded when sent to the server. Only needed if `method="post"`. |
| `method` | Specifies the HTTP method how the data should be transferred. With the default value get the data is sent with the URL and with `post` in the HTTP body. |
| `name` | Sets a name for the form. The name is often used when evaluating other scripts. |
| `novalidate` | This is a standalone attribute that allows you to skip validating form elements when the form is submitted. |
| `target` | This sets the target window of the calling content. Possible values for this are:  `_self` , `_blank`, `_top`, `_parent` |


### HTML attributes for `<input>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `accept` | This allows you to specify the type of a file that will be accepted by the server. This attribute only makes sense in conjunction with `type="file"` for uploading files. |
| `alt` | An alternative text if the graphic cannot be displayed. This attribute only makes sense in connection with graphical controls like `type="image"` |
| `autocomplete` | This allows you to enable autocompletion with the value `on` (= default value) and disable it with the value `off`. |
| `autofocus` | As soon as the web page is loaded, the input field gets the focus, and data can be entered. The attribute is a stand-alone attribute. Correctly, only one element in a form should contain this attribute. |
| `checked` | This allows you to pre-select a checkbox (`type="checkbox"`) or a radio button (`type="radio"`) when the page is loaded. |
| `disabled` | This stand-alone attribute allows you to disable an input field so that it cannot be selected and is grayed out. |
| `form` | With this you determine with which form an input field is linked. The value must be the id attribute of a form element. With attribute it is possible to note an input field outside the form element. |
| `formaction` | Here you specify the URL or path to be called when submitting an input. This attribute overrides the actionAttribute of the form element and only makes sense in conjunction with `type="submit"` and `type="image"`. |
| `formenctype` | Defines how the data should be encoded when sent to the server. Only needed if `method="post"`. This attribute overrides the enctype attribute of the form element and only makes sense with `type="submit"` and `type="image"`. |
| `formmethod` | Specifies the HTTP method how the data should be transferred. With the default value get the data is sent with the URL and with post in the HTTP body. This attribute overrides the method attribute of the form element and only makes sense with `type="submit"` and `type="image"`. |
| `formnovalidate` | This is a standalone attribute that allows you to skip validating form elements when the form is submitted. This attribute overrides the novalidate attribute of the form element and only makes sense with `type="submit"` and `type="image"`. |
| `formtarget` | This sets the target window of the calling content. This attribute overrides the target attribute of the form element and makes only makes sense with `type="submit"` and `type="image"`. |
| `height` | Defines the height of an input element. Makes sense only with `type= "image"`. |
| `list` | As value you pass the id attribute of a datalist element with predefined options for auto-completion. |
| `max`,`min` | This allows you to specify the minimum or maximum value for an input field. You can use these two attributes for the following input fields: `type="number"`, `type="range"`, `type="date"`, `type= "datetime"`, `type="datetime-local"`, `type="month"`, `type="time"` and `type="week"`. |
| `maxlength` | This sets the maximum length of characters. |
| `multiple` | With the boolean attribute you can allow the user, to enter more than one value. This attribute works with `type="file"` and `type="email"`. |
| `name` | Sets a name for the input element. The name is often used when evaluating other scripts. |
| `pattern` | This allows you to define a regular expression as a search pattern, which must match the contents of the input field. |
| `placeholder` | This allows you to define a simple text as a placeholder, which is displayed as long as the input field is empty. It makes sense that this is a hint or help with regard to what the user should enter here (e.g. your e-mail address in the case of an text input field for an e-mail). |
| `readonly` | When you use this standalone attribute, it is not possible to modify the input element is not possible. The input field is read only. |
| `required` | With this standalone attribute you specify that this input field has to be must be filled in before it can be submitted. This attribute can be used for the following input elements: `type="text"`, `type="search"`, `type="url"`, `type="tel"`, `type="email"`, `type= "password"`, `type="date"`, `type="number"`, `type="checkbox"`, `type= "radio"` and `type="file"`. |
| `size` | This sets the visible width of the visible input element in characters. This attribute can be used with the following input elements: `type="text"`, `type="search"`, `type="tel"`, `type="url"`, `type="email"` and `type="password"`. |
| `src` | This sets the URL to a graphic for a button of type `type="image"`. |
| `step` | This is used to specify the value of the increment (interval) with which the control field can be changed. This attribute can be used with the following input elements: `type="number"`, `type="range"`, `type= "date"`, `type="datetime"`, `type="datetime-local"`, `type="month"`, `type= "time"` and `type="week"`. |
| `type` | This sets the type of the input field. Since HTML5 many new types have been added here.  |
| `value` | With this you set the value of an input element. Depending on the type of the input field, this value is used differently. |
| `width` | Defines the width for the input element. This value only makes sense in conjunction with `type="image"`. |


### Types of `<input>` elements for the `type` HTML attribute
| Type               | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `type="button"`    | Button |
| `type="checkbox"`  | Checkbox |
| `type="color"` | Color selection |
| `type="date"` | Date selection |
| `type="datetime"` | date and time selection |
| `type="datetime-local"` | local date and time selection |
| `type="email"` | e-mail address |
| `type="file"` | File selection |
| `type="hidden"` | hidden input field |
| `type="image"` | graphical control element (button) |
| `type="month"` | month selection |
| `type="number"` | number field |
| `type="password"` | password input field |
| `type="radio"` | radio button |
| `type="range"` | slider button |
| `type="reset"` | Reset button |
| `type="search"` | Search input field |
| `type="submit"` | Submit button |
| `type="tel"` | Phone number |
| `type="text"` | one-line text field (default value) |
| `type="time"` | Time selection |
| `type="url" ` | URL input field |
| `type="week"` | Week selection |


### HTML attributes for `<textarea>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `autofocus` | Once the web page is loaded, the textarea element gets the focus, and data can be entered. |
| `cols` | Specifies the width of the text box. This is the number of characters that can be entered per line in a multiline text input field. |
| `disabled` | With this attribute standing alone you can deactivate the text field. |
| `form` | This specifies which form the text field is linked to. The value must be the id attribute of a form element. With this attribute it is possible to note a textarea field outside the form element. |
| `maxlength` | This allows you to set the maximum number of characters that can be entered into the multiline text input field. |
| `name` | Sets a name for the textarea element. The name is often used when evaluating other scripts. |
| `placeholder` | This allows you to define a simple text as a placeholder, which is displayed as long as the input field is empty. It makes sense that this is a hint or help with regard to what the user should enter here. |
| `readonly` | If you use this stand-alone attribute, it is not possible to change the text field. The input field will be read-only. |
| `required` | With this single attribute you specify that this text field must be filled in before the form can be submitted. |
| `rows` | This specifies the number of visible lines in the multiline input field. |
| `wrap` | This lets you specify how line breaks in the multiline text field are to be should be handled when you submit the form. With the default value `wrap="soft"` no additional line breaks will be added (only the ones you manually inserted yourself). With the second possible value `wrap="hard"` will add all the line breaks made by cols will be added. In this case, of course the cols attribute must also be defined with a value. |


### HTML attributes for `<button>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `autofocus` | Once the web page is loaded, the button element gets the focus and is immediately selected. |
| `disabled` | With this attribute standing alone you can deactivate the button. |
| `form` | This specifies which form the button is linked to. The value must be the id attribute of a form element. With this attribute it is possible to note a button outside the form element. |
| `formaction` | Here you specify the URL or path to a server program, to be called when the form is submitted. This attribute overrides the action attribute of the form element. |
| `formenctype` | Defines how the data should be encoded when sent to the server. Required only if `method="post"`. This attribute overrides the enctype attribute of the form element. |
| `formmethod` | Specifies the HTTP method how the data should be transferred. With the default value get, the data is sent with the URL and with post in the HTTP body. This attribute overrides the method attribute of the form element. |
| `formnovalidate` | This is a standalone attribute that allows you to skip validating form elements when the form is submitted. This attribute overrides the novalidate attribute of the form element. |
| `formtarget` | This sets the target window of the calling content. This attribute overrides the target attribute of the form element. |
| `name` | Sets a name for the button element. The name is often used when evaluating other scripts. |
| `type` | Sets the type of the button. Possible values are: `type="button"`, `type="reset"`, `type="submit"` |
| `value` | Sets a value for the button |


### HTML attributes for `<select>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `autofocus` | As soon as the web page is loaded, the selection list gets the focus and is immediately selected. |
| `disabled` | With this attribute alone you can deactivate the selection list. |
| `form` | This specifies which form the drop-down list is linked to. The value must be the id attribute of a form element. With this attribute it is possible to note a select list outside of the form element. |
| `multiple` | With this stand-alone attribute you specify that multiple items in the selection list can be selected by holding down the (Ctrl) or (cmd) key. |
| `name` | Sets a name for the select element. The name is often used when evaluating other scripts. |
| `required` | With this stand alone attribute you make it necessary that the user to select an item in the drop-down list before the form can be submitted. |
| `size` | This sets the number of options that are visible at the same time in the selection list. |


### HTML attributes for `<meter>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `form` | This specifies which form the state indicator is linked to. The value must be the id attribute of a form element. With this attribute it is possible to note a state indicator outside of the form element. |
| `high` | This sets a lower limit to the upper range of the scale. If this attribute is missing, `high` is initialized with the value of `max`. |
| `low` | This sets an upper limit to the lower range of the scale. If this value is missing, `low` is initialized with the value of `min`. |
| `max` | This sets the maximum value of the scale. If you do not use this attribute, `max="1"` will be used. |
| `min` | With this you define the minimum value of the scale. If you do not use the attribute, `min="0"` is used. |
| `optimum` | This sets the optimum value of the scale. This value should lie between the value of `min` and `max`. |
| `value` | The value is absolutely required. With it you set the current value of the state. The value should be between `min` and `max`. |


### HTML attributes for `<optgroup>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `disabled` | With the standalone attribute you can disable the entire group with option elements in the optgroup element. |
| `label` | This creates a visible label for the optgroup element. |


### HTML attributes for `<option>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `disabled` | With this standalone attribute you can disable the option. |
| `label` | This allows you to define a shorter version of a text label for an option element. |
| `selected` | Marks an option as preselected when the document is loaded. |
| `value` | This sets a value that is passed to the server. |



### HTML attributes for `<label>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `for` | With this attribute you define to which input element this text label is bound to. As value you have to use the id attribute of the input element to which you want to bind this text label. |
| `form` | This specifies which form the text label is associated with. The value must be the id attribute of a form element. With this attribute it is possible to write the text label outside the form element. |


### HTML attributes for `<fieldset>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `disabled` | This stand-alone attribute allows you to disable grouping. |
| `form` | This specifies which form this grouping of elements is associated with. The value must be the id attribute of a form element. With this attribute it is possible to note the grouping outside the form element. |
| `name` | Sets a name for the fieldset element. The name is often used when evaluating other scripts. |


### HTML attributes for `<output>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `for` | With this attribute you determine to which input element(s) the output element is bound. As value you have to use the id attribute of the input element to which you want to bind this output element. This way you establish the relationship between the result of a calculation and the elements used for the calculation. |
| `form` | This specifies which form the output element is associated with. The value must be the id attribute of a form element. With this attribute it is possible to note the output element outside the of the form element. |
| `name` | Sets a name for the output element. The name is often used when evaluating other scripts. |


### HTML attributes for `<progress>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `max` | With this you determine the maximum number of steps possible. |
| `value` | Here you specify how many steps have currently been executed. |


## Frames
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<iframe>` | The iframe element is preferably used to embed documents and other web pages. |



### HTML attributes for `<iframe>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `height` | Specifies the height for the iframe element. |
| `name` | Specifies a name for the iframe element. |
| `sandbox` | This allows you to run the document used in the `<iframe>` with a higher security constraint. Possible values for this are allow-same-origin, allow-top-navigation, allow-forms, and allow-scripts. |
| `seamless` | With this attribute standing alone, the document used in `<iframe>` is embedded as part of the web page, which means that the stylesheet definitions and link targets of the current document (can) also be applied to the content of the embedded document. |
| `src` | This specifies the address to the source document to be embedded in the iframe element. |
| `srcdoc` | This allows you to insert HTML code as a resource in the embedded frame instead of referencing it with the src attribute. |
| `width` | With this you set the width for the iframe element. |


## HTML elements for images and graphics
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<area>...</area>` | With this stand-alone element you define the individual reference-sensitive areas of a reference-sensitive graphic. An area element is always enclosed by a map element. |
| `<canvas>...</canvas>` | This element creates an empty drawing surface (canvas) on which you can draw simple graphics with the Canvas 2D API, among other things. |
| `<figure>`,`<figcaption>` | The figure element is used to group and label media content such as photos, videos, annotations, code samples, illustrations, and tables are logically grouped and labeled. The figcaption element, on the other hand, lets you add a caption for the figure element. The figcaption element can be noted as the first or last element within the of the figure element. |
| `<img>` | The img element alone is used to include a graphic file in the HTML document. The HTML attributes `src` and `alt` must be used with this element. Mind you, the graphic itself is only referenced here and is not part of the HTML document. |
| `<map>` | With this element you initiate the definition of the reference-sensitive graphic. The id or name attribute is passed the (anchor) name of the usemap (anchor) name of the usemap attribute of an img element that contains the link-sensitive graphic. With this you practically first create the relationship between a graphic with `<img>` and the map with `<map>`. Inside the map area, use the area elements to note the clickable areas of the reference-sensitive graphic. |
| `<picture>` | With this container element, you can reference multiple image sources and let the browser select and load the appropriate image from different image from different image versions and load it. The picture element itself does but is only a container for the source elements it contains or the img element with the reference to the image source(s). Multiple image sources are specified with the source element. As a fallback, an img element is used at the end. |



### HTML attributes for `<area>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `alt` | Allows you to specify an alternative text that will be displayed when the if the link-sensitive graphic is not displayed. For valid valid HTML, this attribute must also be used with any area element when the href attribute is used. |
| `coords` | Here you specify the coordinates for the reference sensitive area. These are absolute values that you must separate with commas. |
| `download` | You use this to specify a URL or path name to a file that can be can be downloaded when the user clicks the link. |
| `href` | Here you specify the link for the reference target of the link-sensitive area that will be called when the user clicks on it. If attribute is not used, this area element is not a hyperlink. |
| `hreflang` | This specifies the language of the reference target of the reference-sensitive area. |
| `media` | This allows you to specify the media type of the link or a resource. |
| `rel` | This specifies the type of relationship between the current document and the link. Possible values are: `rel="alternate"`: link to an alternate version of the document, `rel="author"`: link to the author of the document, `rel="bookmark"`: permanent URL to create a bookmark, `rel="help"`: links to a help document, `rel="license"`: links to copyright information for the document, `rel="next"`: the next document in a selection of documents, `rel="nofollow"`: links that search engines should not follow(e.g. commercial advertising page), `rel="noreferrer"`: The web browser should not send an HTTP referrer header when the user follows the link, `rel="prefetch"`: specifies that the target resource should be cached, `rel="prev"`: the previous document in a selection of documents, `rel="search"`: the target document should be prefetched in the cache of the cache, `rel="tag"`: a keyword for the current document. |
| `shape` | This determines the type of area for the reference-sensitive area of a reference-sensitive graphic. The possible values for this are: `shape="circle"`: a circle with the coordinates x (center from left), y (center from top) and r (radius) for the coord attribute, `shape="rect"`: a rectangle with the coordinates x1, y1 (upper left corner) and x2, y2 corner) and x2, y2 (bottom right corner) for the coord attribute, `shape="poly"`: a polygon with the coordinates x1, y1, x2, y2, ..., xn, yn (from the upper left corner) for the coord attribute. |
| `target` | This sets the target window for the content to be called. Possible values for this are: `_self`: (default value) output in the same window, `_blank`: output in a new window or tab, `_top`: Output in the body of the window, `_parent`: output in the calling window. |
| `type` | Sets the MIME type of the destination address. |


### HTML attributes for `<canvas>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `height` | This specifies the height of the artboard. |
| `width` | This defines the width of the artboard. |


### HTML attributes for `<img>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `alt` | Allows you to specify an alternative text that will be displayed if the image could not be loaded. This attribute is required for valid HTML. |
| `height` | With this you specify the height of the image source. |
| `ismap` | This allows you to declare the image source as a reference-sensitive graphic with a server-side evaluation. |
| `src` | This specifies the URL to the image source you want to reference. The specification can be absolute or relative. Besides the alt attribute this attribute is required for valid HTML. |
| `usemap` | Use this to mark the image source as a reference-sensitive graphic. The value is a URI that leads to a place where the corresponding map element is noted. Since this map element is usually in the same file, this value is specified with a leading gate character and the name of the anchor (`usemap="#anchor"`). |
| `width` | This specifies the width of the image source. |


### HTML attributes for `<map>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `name` | Here you specify the name (without #) of the reference-sensitive graphic that you specified in the img element with the usemap attribute. You must use the attribute. |


### HTML attribute for `<source>` in combination with `<picture>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `media` | This allows you to use media queries to create breakpoints for the images you want to load. |
| `srcset` | With this you specify a comma-separated list with the image sources. For each specified image source you can also specify the width and pixel density (default value: 1x). |
| `src` | This is used to specify the URL to an image source. |
| `size` | a comma-separated list with a media characteristic and the size specification |
| `type` | This sets the MIME type for the image resource. |


## HTML elements for audio and video
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<audio>...</audio>` | This element allows you to play audio files without special extensions. |
| `<source>...</source>` | This element allows you to provide different versions of media content for audio and video files. |
| `<track>...</track>` | This allows you to add text data as subtitles or captions while playing video and audio files. |
| `<video>...</video>` | This element allows you to play video files without special extensions. |


### HTML attributes for `<audio>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `autoplay` | The audio file is played automatically when the web page finishes loading. |
| `controls` | Displays a bar with controls such as play, pause, etc., that allow the user to control the audio file. |
| `loop` | When the audio file has finished playing, this attribute plays it again. |
| `muted` | The sound of the audio file is muted with this attribute. |
| `preload` | This allows you to specify how the audio file should be preloaded when the web page is loaded. The following values are possible: `preload="auto"`: (default) The web browser should load the complete audio file when the page is loaded; `preload="metadata"`: Only the metadata should be loaded, when the page is loaded; `preload="none"`: The browser should not load the audio file at all when the page is at all when the page is loaded. |
| `src` | This specifies the location (URL) of the audio file. |


### HTML attributes for `<source>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `media` | Allows you to specify the media type of the link or a resource. |
| `src` | You use it to specify the location (URL) of an audio or video resource. |
| `type` | This sets the type for the audio or video resource. Regarding the video element for video files, you can choose from the following types: `type="video/ogg"`: Ogg format; `type="video/mp4"`: MP4 format; `type="video/webm"`: WebM format. And for the audio element for audio files you can use the following types: `type="audio/mpeg"`: MP3 format; `type="audio/ogg"`: Ogg format; `type="audio/wav"`: WAV format. |


### HTML attributes for `<track>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `default` | If multiple subtitles or captions are used, this attribute will with this attribute, a track element is used as the default. In a group of related track elements only one element may contain this attribute. |
| `kind` | This sets the type of label for the track element. |
| `label` | visible text label for the title of the track |
| `src` | This is used to specify the URL to the WebVTT file to be included. |
| `srclang` | This lets you specify the language of the embedded subtitles. |


### HTML attributes for `<video>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `autoplay` | The video file is played automatically when the web page has finished loading. |
| `controls` | Displays a bar with control functions such as play, pause, etc., with which the user can control the video file. |
| `height` | With this you specify the height of the video to be displayed. |
| `loop` | When the video file has finished playing, it will be played again with this attribute. |
| `muted` | The sound of the video file is muted with this attribute. |
| `poster` | This allows you to specify a URL to an image that will be displayed, as long as or when the video is not available (for example, if it has not yet been has not been loaded). |
| `preload` | This allows you to specify how the video file should be preloaded when the web page is loaded. `preload="auto"`: (default) The web browser should load the complete video file when the page is loaded; `preload="metadata"`: Only the metadata should be loaded when the page is loaded; `preload="none"`: The web browser should not load the video file at all at all when the page is loaded. |
| `src` | This specifies the location (URL) of the video file. |
| `width` | This sets the width of the video to be displayed. |


## HTML elements for links
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<a>...</a>` | This element is used to mark and create the hyperlinks (also called references) to other web pages and anchors are marked and created. |
| `<link>` | This allows you to create a logical relationship of the current document to another document. The element is placed in the header data of the head element. Even though the element creates a kind of hyperlink, it cannot be used to create clickable hyperlinks. For that you have the a element. |
| `<nav>...</nav>` | The element is actually more of a section element, but since this element is also recommended to be used for navigation bars and menus for an unsorted list of links to other pages. |


### HTML attributes for `<a>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `download` | With this attribute standing alone, the link specified in the href attribute is offered for download. |
| `href` | This specifies the URL or document where the link goes when the user clicks on the link text or even the graphic between `<a>` and `</a>`. |
| `hreflang` | This allows you to specify the language of the target reference from the href attribute in the form of an IANA (Internet Assigned Numbers Authority) language abbreviation. |
| `media` | With this you set the media type of the link target. |
| `rel` | Describes the relationship between the current document and the link target you specified with the href attribute |
| `target` | This sets the target window of the calling hyperlink that you specified with the with the href attribute. |
| `type` | This allows you to specify the MIME type of the linked resource that you specified with the href attribute. |


### HTML attributes for `<link>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `href` | Use this to specify the target URL to another document that should be related to the current document. |
| `hreflang` | This allows you to specify the language of the target reference from the href attribute in the form of an IANA language abbreviation. |
| `media` | This allows you to specify which media type the target URL in the href attribute uses. |
| `rel` | Describes the relationship between the current document and the link target you specified with the href attribute |
| `sizes` | This allows you to set the sizes for icons, which can be used e.g. with favicons can be used. Multiple values can also be specified here. |
| `type` | Allows you to specify the MIME type for the resource to be included. |


## HTML elements for lists
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<ul>...</ul>` | Use this element to indicate an unsorted enumerated list where the order of the list items is not so important. The individual elements of the list items are added with the li element between the ul element. The bullet is usually displayed as a bullet, but this can be changed with CSS. |
| `<ol>...</ol>` | Use this element to indicate an ordered enumerated list, where the order of the list elements is important. The individual entries of the (mostly) numbered list are also noted here with the li element between the ol element. |
| `<li>...</li>` | With a li element you note the individual list items (or list items) of ordered ol and unordered ul lists. Each li element is a list entry. |
| `<dl>...</dl>` | With this you describe a description list (formerly definition list). Between the dl element you note the expression to be described in the dt element. Expression to be described in the dt element, and the explanation of this expression with the dd element. |
| `<dt>...</dt>` | With this you draw the expression to be explained, which you have noted between the dl element. The description of this expression written in the dt element is written immediately afterwards with the the dd element. |
| `<dd>...</dd>` | The dd element is used for the description of the expression to be explained, which you have marked with a dt element just before. |


### HTML attributes for `<ol>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `reversed` | With this stand alone attribute you invert the numbering which orders the numbering downward (5, 4, 3 ...) instead of upward (1, 2, 3 ...). |
| `start` | This allows you to specify the integer starting value for an ordered ol list for the first li element. |
| `type` | This allows you to specify the type (numbers or letters) of the enumeration. |


### HTML attributes for `<li>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `value` | Sets an integer value for a list item. All subsequent list items are incremented by the value 1. This attribute makes only makes sense for ordered lists with the ol element. |


## HTML elements for tables
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<table>...</table>` | With this element you define an HTML table. Such an HTML table contains many other child elements that you use to define the table's structure of the table (for example, rows and columns). |
| `<caption>...</caption>` | This element allows you to add a caption to the table. The caption element must be placed immediately after the opening `<table>` caption. Also, only one caption can be used per table can be used. By default, the caption is displayed above the table, but with the CSS property `caption-side` and `text-align` you can change this alignment. |
| `<colgroup>`,`<col>` | Use the colgroup element to specify a group of one column in a a table for formatting. This is very useful when you want to apply stylesheets to an entire column, because you do not have to you don't have to repeat the stylesheet for each cell in the same column. With the col element, on the other hand, you specify the column properties for each column in a colgroup element. The col element must be be used inside the colgroup element if the colgroup element does not use a span attribute. |
| `<tbody>...</tbody>` | You can use the element to mark up the main content or body of an HTML table. The element is still often used in in conjunction with the thead and/or tfoot element to divide a table divide a table into multiple sections. Many web browsers also often automatically fill in a missing tbody element when you you view an HTML table without the tbody element using a DOM inspector. |
| `<td>`,`<th>` | Use these elements to draw a single table cell in a table. You use the td element for an ordinary table cell for data, while the th element is used as a table header cell. |
| `<tfoot>...</tfoot>` | You can use the element to mark the table footer or the end of an of an HTML table. The element is often used in conjunction with the tbody and/or thead element to divide a table into multiple sections. |
| `<thead>...</thead>` | You can use the element to mark up the table header or the beginning of an HTML table. The element is often used in tbody and/or tfoot element to split a table into multiple sections. Still divide a table into multiple sections. |
| `<tr>...</tr>` | With this you will draw a new table row. In between you will note the individual table cells (or columns) with the th and td elements. |


### HTML attributes for `<table>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `sortable` | When you use this standalone attribute, you specify, that the data of the table can be sorted. |


### HTML attribute for `<col>` and `<colgroup>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `span` | This allows you to specify how many columns are covered by a group of of table columns (colgroup) or a single table column (col) in the table. Should span in the table. |


### HTML attributes for `<td>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `colspan` | This allows you to specify over how many columns this table cell should span. |
| `headers` | This allows you to specify the ID(s) of the table header cell(s) that are related to or associated with the table cell content. This has no visual effect on the text content of the th element, but this text can be used by screen readers |
| `rowspan` | This allows you to specify over how many rows this table cell should span. |


### HTML attributes for `<th>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `abbr` | This allows you to specify an alternate or shorter text label for the table header cell. This has no visual effect on the the text content of the th element, but this text can be used by screen readers. |
| `colspan` | This allows you to specify over how many columns this table cell should span. |
| `headers` | This allows you to specify the ID(s) of the table header cell(s) that are related to or associated with the contents of other table header cells. This has no visual effect on the text content of the th element, but this text can be used by screen readers. |
| `rowspan` | This allows you to specify over how many rows this table cell should extend |
| `scope` | With this attribute you specify whether a table header cell is a column (col), a row (row), a group of columns (colgroup) or a group of rows (rowgroup). However, this attribute has no effect on the visual display in the web browser, but can be used by but can be used by screen readers. |
| `sorted` | This sets the order of sorting for a column. |


## HTML elements for meta information
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<head>...</head>` | This is the non-displayable header area of an HTML document and contains other elements with important information and resources for the displayable HTML document. |
| `<meta>...</meta>` | With this element you provide additional information to facilitate the management and processing of the file content. The meta elements must be noted within the head element. |
| `<base>...</base>` | This stand-alone base element allows you to note the base URL for relative references in an HTML document. Only a maximum of one base element may be used, and it must be written inside the head element. |


### HTML attributes for `<meta>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `charset` | This specifies the character encoding used for the document. The most common value is probably charset="utf-8" or maybe charset="iso-8859-1". |
| `content` | Here you specify the value of a meta specification. This value is usually associated with the http-equiv or name attribute. |
| `http-equiv` | This allows you to give HTTP instructions in meta specifications. You usually note the value of this HTTP statement in the content attribute. |
| `name` | This is used to specify a name for meta information. Usually you use a name-value pair together with the content attribute. |


### HTML attributes for `<base>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `href` | This specifies the base URL for all relative links in the HTML document. |
| `target` | This defines the default window in which these reference targets should be displayed. Possible values for this are: `_self`: (default) output in the same window; `_blank`: output in a new window or tab; `_top`: Output in the body of the window; `_parent`: output in the calling window; |


## HTML elements for adding other content
| Element            | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `<script>...</script>` | This element allows you to define one or more client-side script areas (such as JavaScript) in the HTML document. You can use this script element in both the head and body elements of the HTML document. If you include an external script with the src attribute, the script element remains empty. |
| `<noscript>...</noscript>` | You can use this element to provide an alternative content or hint if a web browser does not support JavaScript or another scripting language (or is disabled). |
| `<embed>` | This standalone element provides a kind of container for external applications, media, or interactive content not natively supported by the not natively supported by the web browser. |
| `<object>...</object>` | You can also use this element to include active elements that are not natively supported by the web browser into the HTML document. However, unlike the embed element, you can a fallback solution inside the object element because, unlike the element, is not a stand-alone element. Often, the param element is also used inside the object element is often used to pass various parameters to the plug-in of the of the resource to be embedded. The object element can also be used to simply insert another web page into the HTML document. |
| `<param>` | This standalone element is usually used in conjunction with the object element to specify various parameters for a plug-in as well. |


### HTML attributes for `<script>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `async` | If you use this Boolean attribute, the script is executed asynchronously, that is, script execution starts immediately, not after the HTML document is fully loaded. This attribute makes sense only if you have included an external script with the src attribute. |
| `charset` | This allows you to specify a character encoding for an external script specified with the src attribute specified external script. |
| `defer` | If you note this standalone attribute, the external script specified with the src attribute will be executed when the page is loaded |
| `src` | This specifies the URL to an external script file. |
| `type` | This specifies the MIME type of the script. Since this value is `"text/javascript"` since HTML5, you no longer need to use this attribute if you use JavaScript as the scripting language. |


### HTML attributes for `<embed>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `height` | Sets the height for the content to be embedded. |
| `src` | URL Specifies the URL to the external file to embed. |
| `type` | Specifies the media type of the file to embed |
| `width` | Sets the width for the content to be embedded. |


### HTML attributes for `<object>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `data` | This specifies the URL to the external file to be embedded. |
| `form` | This specifies which form the embedded object is linked to. The value must be the id attribute of a form element. |
| `height` | Specifies the height of the embedded object. |
| `name` | This allows you to specify a name for the object. |
| `type` | Use this to specify the media type of the object to be embedded. |
| `usemap` | Name of a map element to control a reference-sensitive graphic. |
| `width` | Lets you specify the width of the object to embed. |


### HTML attributes for `<param>`
| Attribute          | Description                                             |
| ------------------ | ------------------------------------------------------- |
| `name` | Here you specify the name of the parameter for the plug-in. |
| `value` | Here you specify the value of the parameter for the plug-in. |


## Global event attributes for HTML elements
### Event attributes only for `<body>`
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `onafterprint`  	| ... after the document has been printed. |
| `onbeforeprint` 	| ... before the document is printed. |
| `onbeforeunload` 	| ... when the user wants to leave the page, e.g. by clicking on a link. This event attribute takes effect before onunload. |
| `onerror` 		| ... if an error has occurred during the runtime of a script. With this you can catch script errors and react to them separately. |
| `onhashchange` 	| ... if the anchor part of a URL (behind the # sign) has been changed. |
| `onload` 			| ... when the page has finished loading. |
| `onmessage` 		| ... if a message was sent to the active page with the method `postMessage()` page was sent. |
| `onoffline` 		| ... when the web browser switches to offline mode. |
| `ononline` 		| ... when the web browser switches to online mode. |
| `onpagehide` 		| ... when the user navigates away from the web page. |
| `onpageshow` 		| ... when the user navigates to the web page. In principle similar to onload, but the event is fired after onload and also every time, when the web page was loaded - even if the page was loaded from the cache (which onload does not do). |
| `onpopstate` 		| ... when the history of the window has been changed. |
| `onresize` 		| ... when the size of the web browser window changes. |
| `onstorage` 		| ... when a web storage area has been renewed. |
| `onunload` 		| ... when the user leaves the page or the web browser window is is closed. |


### Event attributes for HTML form elements
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `onblur` 			| ... when the element loses focus. |
| `onchange` 		| ... when the value of the element has changed. |
| `oncontextmenu` 	| ... if the context menu was executed with a right mouse click. was executed. However, this only works in conjunction with the contextmenu attribute. |
| `onfocus` 		| ... when an element receives the focus. |
| `oninput` 		| ... when the content is changed by a user input. This is e.g. the case when the user is typing something into a single-line input field. For this reason this attribute only makes sense with the input elements of type password, search and text. But also the textarea element reacts to this. |
| `oninvalid` 		| ... if an invalid entry was made. |
| `onreset` 		| ... if the reset button was clicked. |
| `onsearch` 		| ... if someone types something into the search field (e.g. in the inputElement of type search). |
| `onselect` 		| ... when a text in an element has been selected (highlighted). |
| `onsubmit` 		| ... when someone has clicked the submit button. |


### Event attributes for keyboard actions
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `onkeydown` 		| ... when the user is currently pressing down the key. |
| `onkeypress` 		| ... when the user is holding down the key. |
| `onkeyup` 		| ... when the user releases the key. |


### Event attributes for mouse action
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `onclick` 		| ... when a mouse click was made on an element. |
| `ondblclick` 		| ... when a double click was made on an element. |
| `ondrag` 			| ... when an element is dragged. |
| `ondragend` 		| ... when ending the dragging process. |
| `ondragenter` 	| ... when a dragged element has been dragged to a valid drop target. |
| `ondragleave` 	| ... when a dragged element leaves a valid drop target. |
| `ondragover` 		| ... when a dragged element is directly above a drop element. |
| `ondragstart` 	| ... when the drag operation has been started. |
| `ondrop` 			| ... when a draggable element has been dropped onto a valid drop target. |
| `onmousedown` 	| ... when the mouse button is pressed down over an element. |
| `onmousemove` 	| ... when the mouse pointer is over an element and is moved while is moved. |
| `onmouseout` 		| ... when the mouse pointer leaves an element. |
| `onmouseover` 	| ... when the mouse pointer is over an element. |
| `onmouseup` 		| ... if the mouse button is released while it is over an element. |
| `onscroll` 		| ... when the scrollbar of an element is used. |
| `onwheel` 		| ... when the mouse wheel is rotated up or down over an element. |


### Event attributes for clipboard actions
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `oncopy` 			| ... when the user copies the content of an element to the clipboard. |
| `oncut` 			| ... when the user copies the content of an element to the clipboard using the Cut command. |
| `onpaste` 		| ... when the user inserts a content from the clipboard into an element. |


### Event attributes for video, images, and audio
| Event-Attribute   | Occurs ...                                              |
| ----------------- | ------------------------------------------------------- |
| `onabort` 		| ... when the loading process is aborted. |
| `oncanplay` 		| ... when sufficient data has been loaded into the buffer so that the file is ready for playback. |
| `oncanplaythrough`| ... when the complete data is ready for playback. |
| `oncuechange` 	| ... if a timed cue was changed on the track element. |
| `ondurationchange`| ... if the playing time of the audio or video file has been changed. |
| `onemptied` 		| ... if an error occurs during playback (e.g. transfer error) and the file is no longer accessible. |
| `onended` 		| ... if the audio or video file was played completely to the end |
| `onerror` 		| ... if an error occurred while loading the file. |
| `onloadeddata` 	| ... when the audio or video file is completely loaded. |
| `onloadedmetadata`| ... when the media file metadata has been completely loaded. |
| `onloadstart` 	| ... when it starts loading the media file. |
| `onpause` 		| ... when the media file is paused. |
| `onplay` 			| ... when the media file is ready to be played. |
| `onplaying` 		| ... when it has been started to play the media file. |
| `onprogress` 		| ... when the web browser is in the process of fetching the media file. |
| `onratechange` 	| ... when the playback speed has been changed. |
| `onstalled` 		| ... when the web browser tries to fetch the media file, but this operation does not work for some reason. |
| `onseeking` 		| ... when the user starts to move the current position of the audio or video video file to a new position or skips it. |
| `onsuspend` 		| ... if the web browser wants to fetch the media file, but the process was stopped before the file was finished loading. |
| `ontimeupdate` 	| ... if the playback position in the timeline has been changed. |
| `onvolumechange` 	| ... if the volume was changed while playing the media file. |
| `onwaiting` 		| ... if the media file is paused although it should continue to run. should be executed. This can be the case because more data has to be loaded into the buffer to must be loaded to continue the playback. |


---------------------------------------------------------------------------------
### The End

If you want to know more about HTML then check this out: [HTML Guide](https://github.com/BellaMrx/HTML_Guide).

On my Twitter account [@bella_mrx](https://twitter.com/bella_mrx) you can find more useful stuff about HTML and web development.

Or check out my [GitHub profile](https://github.com/BellaMrx).

Thanks for reading. I hope you enjoyed it or at least learned something.
