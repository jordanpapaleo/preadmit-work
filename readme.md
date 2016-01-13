#Pre-Admittion Work

## Build an About Me page
This whole process shouldn't exceed 10 working hours... This gives us the best view into your capabilities. Some of this is going to require googling to find resources on the internet, and some of it will be available right here in the Units.

The objective is to complete each unit then move onto the next one but keeping the same project and advancing it. Below are a list of steps and instructions broken into these units, please follow along and do your best to personalize your own About Me web page.

This is something that's required knowledge for gaining entry to the course you've applied to, so do your best to show us what you're made of and get as far as you can in around 10 hours!

Must have a complete About Me Page to be considered for the course, you will review this in your instructor interview.

Remember this should just be a couple files at most. When complete please archive (`.ZIP`) and send to your admissions contact. Good Luck! 

Units to complete:

## Unit 1:

### HTML part 1: Intro

HTML is style language, not a logical one. So to start making an HTML page the only thing you have to understand is what a tag is and how to use it.

### HTML part 2: Tags

A tag is any set of keywords surrounded by the less-than '<' and greater-than '>' symbols. Most of the time they are paired as an opening and closing tag as follows, the closing tag is slightly different, notice the preceding forward slash '/' to the tag name or keyword: `<html></html>`

### HTML part 3: index.html file

- The `index.html` file is where the style languages are written in plain text
- Open a text editor, macs can `CMD+Space` and type "TextEdit" and open that application
- Lets add some text to this file in the form of tags and save it as `index.html`

### Browser part 1: Open index.html file

**Way 1:** CMD+Space -> "Terminal" -> $ "open /Users/myUserName/Desktop/index.html"
**Way 2:** Open your favorite browser, select "open file" from the File menu in the apple menu bar, and navigate to the file and select "open"
**Way 3:** Navigate to the file in Finder and double click

### Browser part 2: Refresh The Page with Saved Changes

Now that there are some tags saved into the index.html add a couple more tags, and save the file
To see the changes, instead of closing the tab or window and reopening the file via one of the ways above, the page can simple be refreshed.

- Refresh: Pressing the F5 key on your keyboard while your browser is in focus will refresh the page and get the latest content... yes this works for every web page.
- Refresh: There's also a little refresh icon :emoji_1f503:  ( This looks different per browser and is in different locations ) you just click and the page will reload and get the latest content, again: yes this works for every web page.

### HTML part 4: Wrapper tags ( html / head / body )

HTML documents must be outlined in a valid and proper way to do everything to do with HTML and there are three tags that outline most of this. We'll talk about nesting a little later, but just trust us on these for now.

- **`<html></html>`:** This tag goes at the beginning and end of the entire HTML document. Anything outside of these tags can not be ensured to show up or interact with the page in any expected way
- **`<head></head>`:** This tag sets inside of the _`<html></html>`_ tags and contains all of the meta data and the title of the web application. NOTE: Anything inside this tag will NOT show up in your browser
- **`<body></body>`:** This sets right inside the _`<html></html>`_ tags after the closing </head> tag and contains any content or tags that you wish to display to the end user of your web page

### HTML part 5:

#####`<p></p>`, `<div></div>`, and `<img />` tags... All of these tags belong inside the main `<body></body>` tags

- The `<p></p>` tag is for displaying paragraphs of text
- The `<div></div>` tag is used as a block element to push other elements around and create space as well as a visual carriage return
- The <img /> tag is a little different as it's a self closing tag, notice no closing tag. This can display an image either from the local host, or from a remote location.

```html
<img src="http://img.ur/images/me.jpg" />
<img src="/Users/myUserName/Pictures/me.jpg" />
```

### Unit 1 wrap up: Now that our hands a little dirty...
##### Try adding custom content to all these tags that were just randomly placed in the HTML document... and don't be afraid to google for answer to questions that arise during building.

- Add a personal picture
- Add some content to a paragraph
- Place that paragraph somewhere around aforementioned personal picture


## Unit 2:

### HTML part 6: Nesting Tags

Having already run into this out of necessity it should already be apparent that any some tags can be nested inside of others. What are the rules? Which can be inside which? Are there always parent and always children? How does it know? There's a lot of questions to be answered and it's all pretty simple:

- **Rule 1:** The `<html>` tags are the first and last tag of the document
- **Rule 2:** The `<head>` and `<body>` are only direct children of the <html> tags
- **Rule 3:** The `<title>`, `<style>`, `<link />`, `<script>`, and `<meta />` tags all go in the head
One exception, if the `<script>` is not a library or framework it should go directly before the closing `</body>` tag
- **Rule 4:** Everything else goes inside `<body>` tags
- **Rule 5:** Anything else goes... no really, you can nest anything inside of anything. There are some small exceptions to this rule surrounding `<input>` and `<labels>` tags and some others, but we'll save those for later
Go edit the index.html and move things around a little to utilize the new nesting rules just covered!

### HTML/CSS: Attributes
Every HTML tag can take attributes and some tags require attributes for them to be at all useful.
Exmples:

```html
<img src="image.jpg" />

<div class="className"></div>
<span id="id"></span>
<link rel="stylesheet"  href="stylesheet.css" />
```

All of the words you see inside the **<** & **>** symbols other than the tag keywords are attributes. These attributes have many uses, some of which are detailed here:

| Attribute | Tags        | Basic Use                                                               | Potential Values |
|-----------|-------------|-------------------------------------------------------------------------|------------------|
| `class`   | Almost All  | Style and query selection via scripting language                        | Any String Value |
| `id`      | All         | Place tag into memory for quick access via scripting (also for style)   | Any String Value |
| `src`     | img, script | Links to a file to be processed by the browser                          | File URL         |
| `href`    | a, link     | Hyptertext reference                                                    | URL              |
| `name`    | Most        | This attribute had a different purpost depending on the element, google | String Value     |

There are so many only a ffew are listed above, jump over to [W3Schools](http://www.w3schools.com) if you wish to find more attributes and what they do. Try not to take some of thier code suggestions as best practices though as they show you how things can be done, not the best way to do them always.

### CSS part 1: `<style>` tag & example: 

#### What's CSS, and why do we need it?
##### CSS adds style to the page while removing the style formatting from the HTML page

- Notice the `<style></style>` tags are actually HTML. It's a special tag that allows the writing of CSS into the HTML document. Remember, these tags goes between the `<head></head>` tags.
- Anything between the `<style></style>` tags is considered CSS and will be processed by the browser in such a way. I mention this because it means all the text in between these tags must be valid CSS.

Block Example (with tag as selector):

```css
p{ }
/* OR */
p{

}
```

Property/Value Example:

```css
property: value;
```

( The colon and semi colon are important for every line )

### CSS part 2: Rules

There are multiple different ways to define which tags are selected by the css rules, here's a couple examples:

```css
<style>
/* CLASS EXAMPLE */
.className{ }

/* Try to mostly use the classes, and these much less if at all for style */
/* ID EXAMPLE */
#id{ }

/* TAG EXAMPLE */
a{ }
</style>
```
### CSS part 3: Basic properties

- **color:** The color property can be defined in many different ways, but the easiest is to just use a plain english color.
- **background:** The background is a little more complicated, it can take a color, but it can also take an image link.
- **text-align:** Text align takes in 4 values of `left`, `right`, `center`, or `justified`.
- **font-size:** this can be set in pixels, points, emphasis or relative emphasis.
- **font-family:** this is where you sent the font style, what the actual 'font' is.

| Property    |       Example                                        |
|-------------|------------------------------------------------------|
| color       | `color: darkRed;`                                    |
| background  | `background: url("http://img.ur/something/img.jpg")` |
| text-align  | `text-align: center;`                                |
| font-size   | `font-size: 12pt;` or `12px;` or `12em;` or `12rem;` |
| font-family | `font-family: arial times;`                          |

<br />

## Unit 3:

### Research part 1:  Google properties of the tag being used to style

CSS Part 3 shows us only a couple examples of basic properties and their possible values. go to http://www.google.com and try to find some more examples of css properties and add them to your CSS to give a little more shine to your About Me Page

### HTML part 7:  `<a>` tag:
This is probably one of the most useful tags and it will be used a lot. This is one of those tags that was mentioned above being pretty much useless all by itself. How to use it's properties to make it useful:

- The `href` property gives us a link to another location on the internet
 - Local: `<a href="someOther.html">Some Other</a>`
 - External `<a href="http://www.stackoverflow">Stack Overflow</a>`
- The `target` property sets where the link will open and how
 - New Window / Tab: `<a href="http://www.stackoverflow" target="_blank">Stack Overflow</a>`
 - Same Window / Tab: `<a href="http://www.stackoverflow" target="_self">Stack Overflow</a>`
 - Parent frame: `<a href="http://www.stackoverflow" target="_parent">Stack Overflow</a>`
 - Full body of the window: `<a href="http://www.stackoverflow" target="_top">Stack Overflow</a>`

There are more attributes but the above ones are the important ones... remember there are some attributes such as `class` and `id`.

### HTML part 8: <link /> & style.css file

The <link /> tag is entirely useless without any properties, can't even be styled.
Needs to be in the `<head></head>` tag

- `href` property is the link to the CSS document
- `rel` attribute can be be many values, right now the only important one is `stylesheet`

**Example:** `<link rel="stylesheet" href="style.css" />`

Once you've linked that file and created it, you can move all your CSS over to that file. You do NOT need the `<style></style>` tags surrounding your css in this file, the linking takes care of this with the `rel` property.


### CSS part 5: Advanced Properties

- `border`: This simply gives the border a bunch of different options here's an example, take note that this is a composite and the border property. _Default is no border._ EXAMPLE: `border: thin solid black;`
- `border-radius`: This changes the corners on the element and rounds them by a radius pixel count
- `border-radius: 2px` This would be 50% of a 4px wide element
- `padding`: This pushes the content inside the element away from the border (whether there is a border or not actually visible)
- `padding: 4%;`
- `margin`: This pushes the element around relative to other block elements.
- `margin: 3px;`

Try making that picture of yourself a circle now, and add more flair too... 