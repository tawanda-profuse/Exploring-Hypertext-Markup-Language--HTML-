# The World Wide Web

Hypertext Markup Language, which is shortened to HTML is a computer programming language that is used to produce web pages. The syntax for HTML is represented as tags that are surrounded by angle brackets i.e. **`<>`**. The tags that are used to define a web page can have a closing tag or they can be self closing.

HTML has been around for quite some time, the current version is HTML5 which is the standard for web 3.0 — the third and latest generation of web technologies. Cascading Style Sheets (CSS) is used to complement HTML because on its own a web page would simply be black text on a white page without aesthetics or a layout, which would not engage users of a website because part of what makes a website intriguing is the user interface design.

With advances in technology and increased user demands, new technologies and tools have been invented to make websites including [static site generators](https://www.cloudflare.com/learning/performance/static-site-generator/), and [content management systems](https://en.wikipedia.org/wiki/Content_management_system) such as Wordpress. These are compiled and interpreted as HTML because web browsers cannot comprehend any other language. This means that all information that is rendered in a browser is displayed as HTML regardless of where it is sourced from.

## Attributes

HTML tags can be defined to contain attributes which are extended syntax to declare an additional output. Some attributes can further style an element or tag while others can reference an external resource for a website to access. Attributes are placed inside the opening tag for example; **`<h1 class="green">Example Heading</h1>`**. The attribute in use here is *class* which is a way of grouping elements within CSS.

## Head Element

HTML allows you to write your content in anyway that you want, however, there are standards that are generally accepted for layouts. The **`<head>`** tag is placed at the top of an html file and contains configuration information that will be used by the web page. This includes things like CSS files for styling, Javascript code, Web page title, and meta tags among others. The **`<head></head>`** tag is not self closing, it has a closing tag and can accept attributes such as **`lang`** which defines the language that a web browser should use to display words. 

## Body Element

The body element is placed immediately after the head tag and creates a semantic definition. Much like our bodies, the head is placed above the body in vertical order. The body tag contains all of the things that we see on a web page, all of the visual elements are placed between the opening and closing `<body>`. Essentially, we cannot see anything defined between the head tags because that is only for configuration purposes, so only the browser can read it. Have a look at the diagram below that I designed to explain HTML layout.

**If HTML was a person**
![An image of a person to represent the layout of html tags](human_html)

## Division Tag

The division tag is written as **`<div>`** and it has a closing tag. It defines a section on web a page which can further be defined to display vertically or horizontally using CSS rules. The **`div`** tag can only be placed inside the HTML body and it can contain all other HTML visual tags which are mentioned in the following sections. This tag is important to create the layout of a page.

## Heading Tags

Heading tags display large text and there are 6 available in HTML. These are **`<h1>`**, **`<h2>`**, **`<h3>`**, **`<h4>`**, **`<h5>`**, and **`<h6>`**. The size of a heading tag is defined by the number with 1 being the largest and 6 being the smallest. On a typical web page, the h1 would be the title of the page and all the following tags can be used as sub headings.

## Paragraph Tag

All text placed inside the paragraph tag will be formatted and displayed as a block of text. It is written as **`<p>`** and if placed beneath a heading tag will create a paragraph and a heading much like a magazine or book. We can replace the paragraph tag with the **`<pre>`** tag which preserves the format of text, for example:

```
<pre>
    The quick big brown 
    fox jumped over 
    the lazy
    programmer.
</pre>
```

This will output in the same way that it was written:

![An example output of preformatted text in HTML](pre_html)

Whereas paragraph text will output like this:

```
<p>
    The quick big brown 
    fox jumped over 
    the lazy
    programmer.
</p>
```

![An example output of paragraph tag text in HTML](ptag_html)

## Image Tag

Web pages look boring when they don't have pictures or photos, I even went to great lengths to include photos in this article. There are some websites on the internet that are rich in textual information but if you are a visual learner like me, you may find it difficult to concentrate on the screen. The HTML image tag is defined as **`<img src="#" alt="Some text">`**. The **src** or source attribute is important because the URL of the image should be placed inside the quotation marks as its value. The **alt** attribute is not mandatory but it serves the purpose of describing the image. It is also handy for disabled people because screen readers can pronounce the contents of the picture. The image below is an example of the image tag without a source:

[An example output of an image text](alt_text)

## Anchor Tag

The anchor tag. In my opinion this is the most essential HTML element. The *'H'* in HTML stands for Hypertext, which is the primary purpose of the world wide web AKA the internet — to link one source with another. Hypertext is dynamic text that has access to the resources of another web page. For instance, if you clicked on [**this**](https://andrew-tech.netlify.app) you would get redirected to my websites home page so please make sure to visit. That is hypertext. The anchor tags syntax is **`<a>Link Text</a>`** and should be accompanied by a **href** attribute which has a value of a URL to another web page. 

Some common attributes for anchor are:

- **href**: The value of this attribute is the URL which this element will redirect the user to after clicking.
- **target**: Specifies the action to be taken by the web browser after clicking the link.
- **class**: The value is accessible by CSS for styling and Javascript.
- **id**: Similar to *class* in functionality but ideally used with Javascript only.

The following representation of the anchor tag redirects a user to my website using **href**, opens in a new tab using **target** and, gives the tag a **class** and an **id**.

`<a href="https://andrew-tech.netlify.app" target="_blank" class="sampleClass" id="sampleId">Redirect here!</a>`

## Script Tag

As you may already know, HTML is ideally associated with CSS and Javascript. In order to utilize Javascript in HTML we need to include it using the **`<script></script>`** tags. In addition, if I wanted too use CSS in my web page I would use the **`<style></style>`** tags. This works in one of two ways...

1. Writing Javascript inside the same file as HTML, you will need to place your tags inside the **head** element:

```
    <script>
        var textSample = "Coding is fun!";
   
        console.log(textSample);
    </script>
```

2. Alternatively, you could access a Javascript file by referencing its URL path:

```
    <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
```

By so doing, your website can access all the declarations made with Javascript which adds interactivity to your site. When both are combined with CSS, you get a website that is perfectly laid out, designed, and functional.

## Label Tag

As the name suggests, this tag simply creates a label for a particular element. It is very good for describing an input inside a web form. You could use the **`<label>`** tag anywhere but since there are standards to follow it is best accompanied by an input tag.

## Input Tag

The input tag is available as many different types and defines the kind of information a user can enter into a web form. So think back to when you created your Twitter account, you had to enter some data inside text boxes which are essentially HTML input tags. You can also follow me on Twitter [@drewcavemen](https://twitter.com/drewcaveman). There are several input tags which are specified by the attribute called **type**. 

The various input types are:

1. **type="text"** - Accepts any character keyboard character such as text, number, or symbol.
2. **type="email"** - This accepts any text that contains the "@" symbol, without it the form will not be saved.
3. **type="password"** - The text will be obscured by symbols as the user enters it. 
4. **type="date"** - This opens a context menu that renders a calendar for the user to select a combination of month, day, and year.
5. **type="number"** - This text box only accepts numeric values.
6. **type="file"** - A button appears that can be clicked to open the devices file explorer and the selection will be uploaded.
7. **`<textarea></textarea>`** - This is not particularly an attribute but it is a tag that allows for multiline text like a message or a comment on a social media post.

Here is an example of all the input types together:

```
        <h1>My Web Form</h1>
        <div>
            <label for="acceptName">Name:</label>
            <hr>
            <input id="acceptName" type="text">
        </div>
        <div>
            <label for="acceptEmail">Email:</label>
            <hr>
            <input id="acceptEmail" type="email">
        </div>
        <div>
            <label for="acceptPassword">Password:</label>
            <hr>
            <input id="acceptPassword" type="password">
        </div>
        <div>
            <label for="acceptDate">Date:</label>
            <hr>
            <input id="acceptDate" type="date">
        </div>
        <div>
            <label for="acceptNum">Phone Number:</label>
            <hr>
            <input id="acceptNum" type="number">
        </div>
        <div>
            <label for="acceptFile">Upload:</label>
            <hr>
            <input id="acceptFile" type="file">
        </div>
        <div>
            <label for="acceptMessage">Message:</label>
            <hr>
            <textarea cols="50"></textarea>
        </div>
```

***Example output of the code:***
![Example output of the code](inputtypes)

Not to worry, I've put the code on GitHub via this link: [Source code](https://github.com/tawanda-profuse/Exploring-Hypertext-Markup-Language--HTML-). Now, go ahead and have a look at this ice cream company called 'Sweetooth' that I designed a website for. It's not a real company, just some creativity on my end. The source code is available [here](https://github.com/tawanda-profuse/sweetooth-ice-cream). The project includes other HTML elements that I did not go over in this article so make sure to have a look at each one of them.

---

Here's another article I wrote about [***How My Cat Inspired Me to Be a Better Web Developer***](https://andrew-tech-blog.herokuapp.com/articles/how-my-cat-inspired-me-to-be-a-better-developer).
 
---

### ***~ Thank you for reading***