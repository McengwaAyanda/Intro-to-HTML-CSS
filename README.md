# Intro-to-HTML-CSS
These are the basics of web development.

# HTML Introduction
HTML is a standard markup language for creating web pages.
HTML describes the structure of the web page
HTML consists of a series of elements that tell the browser how to display the content.
HTML elements labels pieces of elements such as "Headings", "paragraphs", "Links" etc.

# Text Formatting
HTML uses tags, which are enclosed in less-than and greater-than symbols, to mark different elements.
HTML tags come in two types: opening tags and closing tags. e.g the opening tag for a paragraph is <p> , and the closing tag is </p>
These tags work together to define elements, which are like packages containing content. some elements, like paragraph contain require both opening and closing tags
while others do not
The HTML document is basically a bunch of HTML elements nested inside each other.
The browser pays attention to this structure and builds a big family tree that shows how everything is related. it is called a Document Object Model (DOM) tree.
It is important to pay attention to where we open and close our HTML tags and how we nest elements within each other. this helps convey meaning about the content and interfaces

# HTML Headlines
Web pages usually contains headlines, headings, subheading when dealing with lengthy text, these elements serve the purpose of dividing the content to smaller digestable chunks.
The HTML elements used for marking up headlines come in 6 different types: h1, h2, h3, h4, h5 and h6. when view in a browser, each headline has a distinct visual effect.
These elements convey a sense of hierarchy in how the browser interprets and communicates about the page.
The h1 is the largest and most prominent, while the h6 is the smallest and least attention grabbing. The other elements fall somewhere in between in terms of prominance and importance.
The choice of the headline level is not based on appearance but on its meaning. It makes sense to use h1 for the main title and h2 for the subheading after the title.
The hierarchical system of the headlines gives meaning browser, distinguishing what is most important to what is less important, It also ensures that all article headlines share the same type, h2,
which is crucial for screen reader users who rely on consistent hierarchical information to navigate the page.

# HTML Bold and Italics
There are 4 elements in HTML that allow us to mark text as bold or italicized. Two of them '<em>' and '<strong>', convey meaning  and serve a language-related purpose. The other two, '<i>' and '<b>' do not
carry any specific meaning and are solely for visual styling 

# HTML lists
There are 3 types of lists: Ordered list, unordered list and definition list
 # Unordered list
Unordered list are the most commonly used type. each item in the list is enclosed in an <li> element, which represent a list item.
To define the entire list and specify its type, we wrap all the items in a <ul> element, which stands for unordered list.
If you want to make our code more readable, indent the list items by adding some space or tabs before each other. However, this indentation does not affect how this page looks.
The default appearance of the list markers is determined byt the browser, but we choose <ul> not solely for its appearance. It is the appropriate choice for conveying meaning and we can use CSS to change the look.
 # Ordered list
 Ordered list is similar to unordered list but with slight difference. Instead of using <ul> to wrap the list items, we use <ol>.
 The term 'ol' stands for ordered list, indicating that the is a specific order to the items in the list.
  # Definition list
Definition list is used when we want to create a lits that resembles a key-value pair in computer science. Instead of just items, we have terms and thier corresponding descriptions.
To create a definition list, we use specific elements. The term or key is enclosed in a <dt>tag, which stands for definition term. The description or value is enclosed in a <dd>tag, which stands for definition description.
The entire list is wrapped in a <dl>tag representing the definition list. interestingly, the <dd>tags and <dt>tag are placed side by side without any additional wrapper around them.

# HTML Quotes
These 2 elemnts, <cite> and <blockquote>, serve a semantic purpose. they inform other computers, "Hey this is what it is", additionally, they provide a convenient way to apply custom styling.
The important thing is that elements should be nested within each other in a way that makes sense.
To make things easier, we can use <q> element in HTML which stands for quote.  by using this element the browser will add the appropriate quote marks for us.
Some HTML elements, like <i>, <strong>, <b> and <em> are called inline, because they are meant to wrap around phrases of text that are inline with other content.
There are certain elements in HTML known as block-level elements, like block quotes, paragraphs and unordered lists. These elements essentially  create separate blocks on the page.
Some elements serve as markers for something that is part of a larger enitty, while others represent the larger enitity itself.
HTML attributes provide additional information to HTML elements. in this case, datetime attribute allows us to specify the date or time in a format that computers can understand. We write it like this: <time datetime= "2025-05-02"> May 02, 2025 </time>.
The format of the date within the date time has to be specific. Dates and times have a special format that machines can understand, we need to use that format.
Machines prefer a highly standardized format, and we can also indicate times using the time element. The machine-readable version prefers numbers in the 24-hour clock format and we can choose whether to include seconds and fractions of a second or not.
You can also combine the time and date using the datetime attribute. first you include the date than the time. you have a couple of options for separating them, you can use a T or leave a space.
There are various ways to format the machine-readable time, they are all acceptable and correct, and they apply to many programming languages.

# HTML code, pre and br
By default, code is treated as an inline element, meaning that it remains part of the sentence its in.
The 'Br' element is a simple tag without the opening or closing tag. It does not contain anything inside it, it just indicates where the line needs to break
Pre and code are often combined to display a code block with proper indentation. we have the code, br and pre working together, and these elements are handy for conveying the structure and appearance of code, as well as other types of contents.

# HTML Superscripts, Subscripts and Small text
Superscripts, subscripts and small text can be used where you need to mark up certain bits of content as having a different meaning than the rest.
Subscripts are characters that are set below the normal baseline for text, while Superscript are characters that are set above the normal baseline for text.
Small, sub, and sup are the elements that can help you get the details right when it comes to typography and conveying the full meaning of your content.

# Debugging and troubleshooting HTML code
If you are ever about the markup to use, visit other websites with similar content and use the developer tools to find out which elements they used. it is especially useful if the website was built by a team we admire because studying others' work helps understand how to structure your own HTML

# HTML Attributes
When looking at global attributes in HTML that work universally, we will look at 4 highly useful ones.
The class attribute is the most commonly used. it allows us to assign a reusable name to any element, which can than be styled using CSS, for all elements sharing that class.
Another popular attribute is the Id. it is similar to the class attribute, but we can use unique names once on the entire HTML page. IDs can be used for CSS targeting, but are more specific and can sometimes cause issues.
IDs come in handy when we need to address specific elements in Javascript or targeted links. The uniqueness of an ID name ensures that there will always be one element with that ID, making it useful for interacting with Javascript or links.
Class and ID attributes provide a way to name HTML elements and reference them to other parts of the code stack.
HTML offers many attributes that enhance user interaction and provide hooks into browser power. These attribute such as 'content editable' allow interaction with the screen, keyboard, and assistive devices. They facilitate the editing capability within the browser.
The 'dir' attribute explicitly indicates the direction which the text flows using "LTR" for Left-To-Right and "RTL" for Right-To-Left scripts. These attributes "lang" and "dir" are considered global attributes and can be used on any HTML element.

# Aria Roles
Aria roles are like extra HTML attributes that we can add to HTML elements to make them more meaningful and help browsers understand what they represent. 
Aria roles come into play when we want to provide essential information to assistive technologies like screen readers, braille displays and magnifiers to ensure a website is fully accessible.
The accessibility tree is like a companion to the DOM tree, which the browser creates from the websites content. while the DOM tree represents the HTML structure, the accessibility tree is crucial for assistive devices like screen readers.
When we look at the accessibility tree, we can see that it treats the content as separate text containers. this results in poor experience, such as each letterbeing read individually. to improve this we use Aria.
Aria is a powerful tool that greatly enhance web accessibility and is worth exploring further. Aria provides the necessary tools to make your site accessible to everyone.

# Formatting HTML
