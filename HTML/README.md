# HTML 🖥️
 - It stands for Hyper Text Markup Language.
 - It is used mainly for ``Presentation`` purpose.
 - ``Markup`` refers to ``Marking up the content`` so that it can be presented exactly as required.
 - HTML to browser will display the presentation as need by the user.


## Evolution of HTML:

 - In Early 1960's GML and SGML are the languages used for ``Markup``.
 - Generic Markup Language and StandardGenericMarkUp Language were designed by CERN[Council for European Research and Nuclear] Labs.
 - In early 1990's ``Time Berner lee`` introduced ``WEB`` and a language for "WEB" that is ``HTML``[Open Source].
 - IETF(Internet Engineering Task Force) these people developed HTML for several years up to HTML3.1.
 - In 2004 ``WHATWG``(Web Hypertext Application Technology Work Group) took the responsibility of HTML and started the 
    version ``HTML4.0``.
 - Official website of WHATWG is "whatwg.org".
 - The latest version of HTML is ``HTML5``(2014).


### FAQs :-
#### Whats new in HTML5?
    HTML5  introduced new features to make webpages more browser and SEO friendly.
    SEO refers to "Search Engine Optimisation".
    Responsive Designs[users using webapplication using phones, so website should provide facility for user to use website]

## Browser Architecture 🌐💻🛠️

A ``browser`` is a software tool that allows users to access webpages on a client device. Popular browsers include:
- Chrome
- Firefox
- Edge
- Safari

Each browser consists of the following components:
### 1. User Interface (UI)
This includes elements such as the title bar, address bar, refresh button, etc., that allow users to interact with the browser.

### 2. Browser Engine
The browser engine is responsible for converting HTML and CSS into a format that the browser can understand. Different browsers use different browser engines, such as:

- **Gecko** (used by Firefox)
- **WebKit** (used by Safari)
- **Blink** (used by Chrome and Edge)
- **Chakra** (used by older versions of Edge)
- **SpiderMonkey** (JavaScript engine for Firefox)

### 3. Rendering Engine
This component is responsible for the presentation of processed content. It interprets the content from HTML and CSS into a visual display on the screen.

### 4. JavaScript Interpreter
Browsers use JavaScript for interactive functionality. The JavaScript interpreter converts JavaScript code into a format the browser can execute.

### 5. Networking
The networking component manages all network activities in the browser, including:

- Loading resources such as images, scripts, and stylesheets
- Handling the number of requests made per page
- Measuring the time taken to load content

### 6. UI Backend
This component contains the logic responsible for rendering the user interface, including buttons, checkboxes, and other input controls.

### 7. Data Persistence
Browsers store user data in different formats to enhance user experience, including:

- **Local Storage**: Stores data across sessions
- **Session Storage**: Stores data for the duration of a session
- **Cookies**: Store small amounts of data for stateful interactions with websites

## HTML Parsing in Browser

### Flow 
Markup 
   -> bytes 
      -> characters 
         -> Tokens [Tags] 
            -> Elements [Nodes] 
               -> DOM 
                  -> Layout 
                     -> Rendering 
                        -> Painting

*HTML       - presenting DOM* <br>
*JAVASCITPT - Modifying  DOM*

- HTML present content on browser using elements arranged in hierarchial order called "DOM".
- There are 100's of elements.

### HTML Elements are classified into 5 categories
### a. Normal elements
- Elements which return a presentation directly on call back [without any additional attributes].
- Elements in HTML are built by using tags.
- Normal Elements require a start tag and end tag.
- Normal Elements will start returning presentation but can’t stop implicitly.
- They require explicit end tag.
- Usually require start and end tags.
	
- Example:
```HTML
<b>HELLO</b>
```
### b. Void Elements
- Void elements refer to elements that don’t return any presentation directly upon being rendered.
- The term "void" indicates that they have no return type.
- They can return specific content and stop implicitly.
- Void elements do not require an "end tag."

Example:
```html
<img src="image.jpg" alt="Image description">
```
### c. Raw Text Elements
- These elements are presented without a tag.<br>
		eg:: Temparature20C 45000/-<br>
		     Temparture&deg;C &#8377;45000/-
		     
Example:
```html
&copy; ©
&#8377;
&deg;
```

### d. RC Data Elements
- RC Data Elements, or Rich Text Content Elements, do not allow any other elements within their context.

Example:
```html
<textarea>
    Hello
    <b>pwian's</b>
</textarea 
```

### e. Foreign Elements
- Foreign elements are those that are not natively understood by every browser.
- You need to import a library that enables browser compatibility with these elements.

Example:
- SVG
- MathML
- Canvas


## HTML Page Structure

- Every HTML file must have static extensions called ".html or .htm"
- Every HTML page starts with documentation declaration from HTML5 version.<br>
 			<!doctype html><br>
	It is a indication to the browser engine that i am using latest features of HTML, if we don't specify the doctype then the
	browser engine understands the HTML has "HTML4" version.

- Every HTML page must have a documentation scope, It specifies the start and end of the document in browser.
#### eg: 
      <html> 
		document scope
		</html>

    eg#1.
	<!DOCTYPE html>
	<html>
        	document-1
	</html>
	<html>
        	document-2
	</html>
	     Note: If some changes needs to be done in document-1, then it creates a problem because browser does the below things
	<!DOCTYPE html>
	<html>
        	document-1 document-2
	</html>
   

