# the web platform

una lista di tecnologie facenti parte secondo chatgpt della web platform: 

- HTML (Hypertext Markup Language)
- CSS (Cascading Style Sheets)
- JavaScript
- HTTP (Hypertext Transfer Protocol)
- Web Browsers (Chrome, Firefox, Safari, Edge, etc.)
- APIs (Application Programming Interfaces)
- XML (eXtensible Markup Language)
- JSON (JavaScript Object Notation)
- AJAX (Asynchronous JavaScript and XML)
- Web Servers (Apache, Nginx, IIS, etc.)
- DNS (Domain Name System)
- URL (Uniform Resource Locator)
- SSL/TLS (Secure Sockets Layer/Transport Layer Security)
- Cookies
- Responsive Web Design
- Web Standards (W3C, WHATWG)
- Front-end Frameworks (React, Angular, Vue.js)
- Server-side Languages (PHP, Python, Ruby, etc.)
- Databases (MySQL, PostgreSQL, MongoDB, etc.)
- Content Management Systems (WordPress, Drupal, Joomla, etc.)
- Web Security (Cross-Site Scripting, Cross-Site Request Forgery, etc.)
- Single-page Applications (SPAs)
- Progressive Web Apps (PWAs)
- Web Accessibility (WCAG - Web Content Accessibility Guidelines)
- Multimedia (Audio, Video) Support (HTML5, codecs)
- WebRTC (Web Real-Time Communication)
- Web Storage (localStorage, sessionStorage)
- Web Workers
- Browser DevTools (Inspect, Console, Network, etc.)
- Web Assembly (Wasm)

# html
Oxford dictionary of computer science

HTML (hypertext mark-up language) A form of *SGML intended for use on the World Wide Web. A particular feature of HTML is the use of tags that include information about *hyperlinks, either to other places in the document or to other documents on the Web. Text surrounded by these tags is usually underlined and in a different colour when displayed by the browser, and can be clicked to jump to the link. HTML has a set of basic tags, mostly defining format rather than content, although some *browsers use nonstandard tags. The current version is HTML5. See also CSS, DHTML, XHTML, XML.

https://www.britannica.com/technology/HTML

HTML, in full hypertext markup language, a formatting system for displaying material retrieved over the Internet. Each retrieval unit is known as a Web page (from World Wide Web), and such pages frequently contain hypertext links that allow related pages to be retrieved. HTML is the markup language for encoding Web pages. It was designed by the British scientist Sir Tim Berners-Lee at the CERN nuclear physics laboratory in Switzerland during the 1980s. HTML markup tags specify document elements such as headings, paragraphs, and tables. They mark up a document for display by a computer program known as a Web browser. The browser interprets the tags, displaying the headings, paragraphs, and tables in a layout that is adapted to the screen size and fonts available to it.

HTML documents also contain anchors, which are tags that specify links to other Web pages. An anchor has the form <A HREF= “http://www.britannica.com”> Encyclopædia Britannica</A>, where the quoted string is the URL (universal resource locator) to which the link points (the Web “address”) and the text following it is what appears in a Web browser, underlined to show that it is a link to another page. What is displayed as a single page may also be formed from multiple URLs, some containing text and others graphics.

https://www.britannica.com/technology/SGML

SGML, in full standard generalized markup language, an international computer standard for the definition of markup languages; that is, it is a metalanguage. Markup consists of notations called “tags,” which specify the function of a piece of text or how it is to be displayed. SGML emphasizes descriptive markup, in which a tag might be <emphasis>. Such a markup denotes the document function, and it could be interpreted as reverse video on a computer screen, underlining by a typewriter, or italics in typeset text.  
SGML is used to specify DTDs (document type definitions). A DTD defines a kind of document, such as a report, by specifying what elements must appear in the document—e.g., < Title >—and by giving rules for the use of document elements, such as that a paragraph may appear within a table entry but a table may not appear within a paragraph. A marked-up text may be analyzed by a parsing program to determine if it conforms to a DTD. Another program may read the markups to prepare an index or to translate the document into PostScript for printing. Yet another might generate large or enhanced type or audio for readers with visual or hearing disabilities.

https://www.britannica.com/technology/markup-language

markup language, standard text-encoding system consisting of a set of symbols inserted in a text document to control its structure, formatting, or the relationship between its parts. The most widely used markup languages are SGML (Standard Generalized Markup Language), HTML (Hypertext Markup Language), and XML (Extensible Markup Language). The markup symbols can be interpreted by a device (computer, printer, browser, etc.) to control how a document should look when printed or displayed on a monitor. A marked-up document thus contains two types of text: text to be displayed and markup language on how to display it.



# documenti html5 
```html
<!DOCTYPE html>
<!--document type declaration-->
<html lang="en">
<!--document root element-->
<!--language information-->
<head>
<!--document head-->    
    <meta charset="UTF-8">
    <!-- generic metainformation-->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <!-- generic metainformation-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- generic metainformation-->
    <title>Document</title>
    <!--document title-->
</head>
<body>
    
</body>
</html>
```
___
```html
<!DOCTYPE html>
```
https://www.w3schools.com/tags/tag_doctype.asp

The declaration is not an HTML tag. It is an "information" to the browser about what document type to expect.

https://html.spec.whatwg.org/multipage/syntax.html#the-doctype

A DOCTYPE is a required preamble.

DOCTYPEs are required for legacy reasons. When omitted, browsers tend to use a different rendering mode that is incompatible with some specifications. Including the DOCTYPE in a document ensures that the browser makes a best-effort attempt at following the relevant specifications.

https://www.w3.org/TR/html401/struct/global.html

A valid HTML document declares what version of HTML is used in the document. The document type declaration names the document type definition (DTD) in use for the document (see [ISO8879]).

___
___
```html
<html></html>
```
https://www.w3schools.com/tags/tag_html.asp

The <html> tag represents the root of an HTML document.

The <html> tag is the container for all other HTML elements (except for the <!DOCTYPE> tag).

Note: You should always include the lang attribute inside the <html> tag, to declare the language of the Web page. This is meant to assist search engines and browsers.

https://www.w3.org/TR/html401/struct/global.html

After document type declaration, the remainder of an HTML document is contained by the HTML element. Thus, a typical HTML document has this structure:
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
"http://www.w3.org/TR/html4/strict.dtd">
<HTML>
...The head, body, etc. goes here...
</HTML>
```
___



```html
<html lang="en"></html>
```
https://html.spec.whatwg.org/multipage/dom.html#attr-lang

The lang attribute (in no namespace) specifies the primary language for the element's contents and for any of the element's attributes that contain text. Its value must be a valid BCP 47 language tag, or the empty string. Setting the attribute to the empty string indicates that the primary language is unknown.

https://www.w3.org/TR/html401/struct/dirlang.html#language-info

This attribute specifies the base language of an element's attribute values and text content. The default value of this attribute is unknown.
___
```html
<head></head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head?retiredLocale=it

The <head> HTML element contains machine-readable information (metadata) about the document, like its title, scripts, and style sheets.

https://www.w3.org/TR/html401/struct/global.html

The HEAD element contains information about the current document, such as its title, keywords that may be useful to search engines, and other data that is not considered document content. User agents do not generally render elements that appear in the HEAD as content. They may, however, make information in the HEAD available to users through other mechanisms.

___
```html
<head>
    <meta>
</head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta


The meta HTML element represents metadata that cannot be represented by other HTML meta-related elements, like base, link, script, style or title.

https://www.w3.org/TR/html401/struct/global.html#meta-data

HTML lets authors specify meta data -- information about a document rather than document content -- in a variety of ways.

___
```html
<head>
    <meta charset="UTF-8">
</head>
```
https://www.w3schools.com/tags/att_meta_charset.asp

The charset attribute specifies the character encoding for the HTML document.

___
```html
<head>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
</head>
```
https://www.geeksforgeeks.org/what-does-meta-http-equivx-ua-compatible-contentieedge-do/

Meta Tag: A tag with the http-equiv attribute set to “X-UA-Compatible” and the content attribute set to “IE=edge” is used to force Internet Explorer (IE) to use the latest version of the rendering engine. Regardless of the document’s compatibility mode.

___

```html
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
</head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag

width
Controls the size of the viewport. It can be set to a specific number of pixels like width=600 or to the special value device-width, which is 100vw, or 100% of the viewport width. Minimum: 1. Maximum: 10000. Negative values: ignored.

initial-scale
Controls the zoom level when the page is first loaded. Minimum: 0.1. Maximum: 10. Default: 1. Negative values: ignored.

https://www.w3schools.com/css/css_rwd_viewport.asp

This gives the browser instructions on how to control the page's dimensions and scaling.
___

```html
<head>
        <title></title>
</head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title

The Document Title element. The contents of a page title can have significant implications for search engine optimization.

___
```html
<body></body>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/body

The body HTML element represents the content of an HTML document. There can be only one body element in a document.
___

# template di una landing page

al template di cui sopra, viene aggiunto:

```html
<head>
    <!-- Collegamento a Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap" rel="stylesheet">
</head>
```
```html
<head>
    <!-- Collegamento a Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>       
```
```html
<head>    
    <!-- Collegamento al file CSS -->
    <link rel="stylesheet" href="./style.css">
</head>
```
```html
<body>
 <!-- Menu di Navigazione -->
    <nav id="main-nav">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">Chi Sono</a></li>
            <li><a href="#skills">Competenze</a></li>
            <li><a href="#contact">Contatti</a></li>
        </ul>
    </nav>
</body>    
```
```html
<body>
    <!-- Sezioni -->
    <section id="home">
        <h1>Benvenuto nel mio sito personale</h1>
        <p>Scopri le mie competenze Full Stack.</p>
        <p></p>
    </section>

    <section id="about">
        <h2><i class="fas fa-user"></i> Chi Sono</h2>
        <p>Sono un sviluppatore Full Stack con esperienza in vari linguaggi e tecnologie.</p>
        <p></p>
    </section>

    <section id="skills">
        <h2><i class="fas fa-cogs"></i> Competenze</h2>
        <ul>
            <li>HTML, CSS, JavaScript</li>
            <li>React, Angular, Vue.js</li>
            <li>Node.js, Express</li>
            <li>Database management</li>
        </ul>
    </section>

    <section id="contact">
        <h2><i class="fas fa-envelope"></i> Contattami</h2>
        <p>Email: info@example.com</p>
        <p>Telefono: 123-456-7890</p>
        <p></p>
    </section>

</body>    
```
