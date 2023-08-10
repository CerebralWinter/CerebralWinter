# documenti html5 

## template di un documento vuoto
```html
<!DOCTYPE html>
<!--document type declaration-->
<html lang="en">
<!--document root element-->
<!--language information-->
<head>
<!--document head-->    
    <meta charset="UTF-8">
    <!-- -->
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
<html lang="it"></html>
```
https://html.spec.whatwg.org/multipage/dom.html#attr-lang

The lang attribute (in no namespace) specifies the primary language for the element's contents and for any of the element's attributes that contain text. Its value must be a valid BCP 47 language tag, or the empty string. Setting the attribute to the empty string indicates that the primary language is unknown.
___
```html
<head></head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/head?retiredLocale=it

The <head> HTML element contains machine-readable information (metadata) about the document, like its title, scripts, and style sheets.

https://www.w3.org/TR/html401/struct/global.html

The HEAD element contains information about the current document, such as its title, keywords that may be useful to search engines, and other data that is not considered document content. User agents do not generally render elements that appear in the HEAD as content. They may, however, make information in the HEAD available to users through other mechanisms.
___

___
```html
<head>
    <meta>
</head>
```
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta


The meta HTML element represents metadata that cannot be represented by other HTML meta-related elements, like base, link, script, style or title.

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
