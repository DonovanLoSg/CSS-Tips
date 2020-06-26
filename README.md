![by Donovan](http://resume.donovanlo.sg/images/donovanlogo150x131.png)  

# CSS Styling Tips

<div id="howto">

This are some simple tips I use. It's a result of compiling and digesting those CSS syntax and lessons.  

</div>

## Catch the Problem before It Happens

You wouldn't want to find out you page looks different or have certain problem after you have completed all the styling, would you?

### Use a CSS Reset

In case you didn’t know, every browser has its own default ‘user agent’ stylesheet, that it uses to make unstyled websites appear more legible.

(Ever wondered why Submit buttons look different in every browser?) A CSS Reset give developer a better control of the style, but that also means that the developer has to style from the basics, including H1 to H6.

(explanation: [https://meyerweb.com/eric/tools/css/reset/index.html)](https://meyerweb.com/eric/tools/css/reset/index.html)

### Include a diagnostics CSS

Don't worry, it won't break your code.

If your codes are good, this will most probably be invisible. [https://meyerweb.com/eric/tools/css/diagnostics/diagnostic.css](https://meyerweb.com/eric/tools/css/diagnostics/diagnostic.css)

(explanation: [https://24ways.org/2007/diagnostic-styling)](https://24ways.org/2007/diagnostic-styling)

## Bull's eye identification

It will difficult to make changes to an element if you can't easily identify an element.

You will know what I mean if you are using JavaScript, DOM, jQuery etc.

### Identifying the target

If you need to target an individual element, use #id.

e.g. #hero-image

If that content element appears only once per page, identify them uniquely by their purpose on the page.

They can follow their semantic html tags.

e.g. #header-something, #main-something, #footer-something

### Classify the targets

If they appears more than one time, use class for identification, still following semantic tags whenever possible.

e.g. .header-something, .main-something, .footer-something

It should help to cover most of the items on the page. Else you can also create a special id or class to ease identification.

e.g. #map-restaurant, #diagram-family-tree

If a content element need to chain more than three selectors to pinpoint it, it’s too many.

e.g. body > section > div > p > p > ul > li > ul > li> span

## Eagle view style

### Comment your stylesheet.

Add lines of comments like what you would do in the page itself.

e.g.  
/****** main content *********/  
/****** footer content *********/

It will ease the job of locating a certain rules.

It's even more obvious if you can open the html file and the css file side by side to do the styling.

### Group common effect

If it's a certain style that may apply to different parts of the page, describe the style

e.g.  
.border-green {border: 1px solid green};  
.margin-zero {margin: 0};

## Prevent Cross Infection

Sometimes, after you style a page to your liking, then you realized that you have unintentionally affected the layout on the other pages of the side.

Sometimes, the css file can get very long if there are many pages and there's many elements using Id.

### Use separate CSS files

Use a common css file for the common items in every page of the site.

e.g. style.css

Then add another css file that belong exclusively to each page.

class="examples"e.g. home.css, contact.css, article.css

This way, it will be easy to know whether the rules you are changing will affect the other pages.

## Structure, Content before Styling

Know how your web pages will be divided into so you know where the content will go to.

### Scenerio

[not available in markdown, refer to index.hml]



As for the CSS Tags, I would recommend this article: [Comprehensive CSS Cheat Sheet + PDF](https://www.onblastblog.com/css3-cheat-sheet/)"
