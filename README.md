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
When we look at the accessibility tree, we can see that it treats the content as separate text containers. this results in poor experience, such as each letter being read individually. to improve this we use Aria.
Aria is a powerful tool that greatly enhance web accessibility and is worth exploring further. Aria provides the necessary tools to make your site accessible to everyone.

# Formatting HTML
In HTML comments are inserted by typing "<!-- comments -->". These comments are disregarded by the browser, but code editors like Notepad++ can display commented code or remarks in a grayed-out fashion. 
This feature helps developers quickly identify when code is commented out and prevents any confusion when it does not function as expected.
People used to capitalize all their HTML elements, but as HTML evolved, the web industry embraced the idea of using lowercase letters for everything. The broswer isn't affected either way.
Some HTML elements are short like <i> and <p> while some are long like <article> and <video>. The reason for this is that when HTML was first created, computer scientist were focused on optimizing file size due to limited computer resources. 
As technology advanced and computer memory expanded, it became less crucial to save a few characters and more important to prioritize code readability and understanding for humans. Hence, newer HTML elements started using complete words instead of abbriviations. This change made it easier for english-speaking people to comprehend the code.
Nowadays, the length of an element can give us a clue about how long it has been in existance.
A bunch of elements in this course and most of them have a opening and closing tag. The newer HTML elements always have both tags, but for some of the older elements the are no closing tags.

# Unusual characters
The symbols < > and & are important characters in HTML.
In the demo, we used something called character entity in HTML. These entities are formatted like this: an ampersand, ashort code and a semicolon. When we use these in HTML files, they are converted into the specific characters we want. we applied this technique to replace every instance of greater-than or less-than symbols with their corresponding character entities.

#HTML Navigation and linking

# HTML Links
When we want to create a link, we use the "A" element, which stands for "anchor". to do this, we need to add a "href" attribute with a URL enclosed in quotes. This URL is where the link will take us. 
The term "href" stands for "HyperText reference", a nerdy phrase from the past.
By default, the "A" element is inline and can be placed within a paragraph or any other text. Links are not limited to just text but we can wrap them around images or even more complex elements like teaser cards. This allows us to create a group of linked elements.
When linking to another website or a specific page on a web, you can include the entire URL. It doesn't matter if it has a trailing slash or not. These types of URLs are called "Absolute URLs" because they point to a precise location on the web. 
In an absolute Url, the HTTP or HTTPS part must be included which stands for "HyperText Transfer Protocol". This protocol defines the rules of communication on the web and is crucial for linking.
When creating links as developers or content creators, we need to include them ourselves. This protocol is one of the significant inventions when the web was created. This is how links are made using absolute URLs.

# HTML URL Pathways
When forming links, absolute URLs are one option. When linking to something within the same site and domain as the page containing the link, a relative URL can be used instead.
Creating a relative URL is not only useful for the "A" element(linking), but it is also a skill used to reference image files, video files, CSS, Javascript files or any other where a files pathis specified.
To form a URL, you need to grasp how files are organized. filenames comes with extensions like ".html", "jpg", "CSS", "js", whereas directories or folder names have no extentions. The Slashes in a Url indicate that we should look deeper into the file structure or go one level down.
Creating well structured and elegent URLs for web page is an art. it is worth considering how your URLs impact user experience and search engine results. Craft URLs carefully.
Using relative URLs can be extremely helpful, especially when working on a project that moves from server to server.
URLs can be either relative or absolute. Relative URLs are based on the current files location, while absolute URLs start from the root of the website. By using folders and index.html files, we can create clean and user-friendly URLs.

# Navigation
Each link is wrapped in an element with the correct URL, and then enclosed in a "<li>" element to create a list of links. To maintain order, wrap the whole list in a "<ul>"element which represents an unordered list. Finally, encompass the entire menu in a "<nav>" element to indicate that it is the site's navigation.
To give the menu a visual appearance, apply CSS styling. Without CSS styling, it appears as a plain list, however, we want screen readers and assistive devices to understand that it is a main menu.
Assign the role "navigation" to the "<nav>" element, which signifies that it represents the main navigation of the page. Include an "aria label" for the main menu, providing a descriptive label that can be read alound by a screen reader.

# HTML Working with Graphics and Images
When we want to add images to a web page, we use the image element, which is simply written as "<img src="image.jpg" alt="brown dog" width="400" height="300">"
there are 4 attributes that need to be included for every image
1. We have the source attribute(SRC), which tell the browser which image file to load.
2. than we have the alt attribute(ALT), which provides a text description for the image.
3. lastly we have the width and height attributes, which determine the size of the image. so every image should have all four of these attributes.
The Image's URL is pasted in the source, and than the image starts loading. Add an ALT attribute, which serves as a replacement for when the image cannot be seen.
Make the ALT text interesting. There is no need to make a lengthy description just focus on what it depicts. You have the option to make the ALT text funny or poetic, and if there is nothing significant to convey about the image, simply leave the ALT text blank.
If the ALT is omitted altogether, there is a chance that the image filename will be read aloud, and we definitely do not want that to happen.
It does not matter whether the height or width is specified first. In HTML, the order of attributes within an element can be whatever you prefer.

# Image formats
The image file itself is a crucial aspect to consider when putting an image on a webpage.It need to be in a file format that web browsers can understand, and there are various options available
We keep coming up with different formats in our pursuit of finding the perfect balance between small file sizes and visually stunning images. we desire a large amount of data to make the image look fantastic, but also minimize the data to ensure faster downloads and prevent excessive data usage for users. Essentialy, we aim for the highest possible quality with the smallest file size achievable. Each file format employes a distinct approach to tackle this challenge, utilizing different techniques to compress the image.
There are four main file formats commonly used on the web these days, each with its own strengths and weaknesses when it comes to compressing images: GIF, SVG, JPG, PNG.

# Responsive Images
CSS offers a solution for displaying images in different sizes to accommodate both large and small screens. The challenge arise when we dealing with big, high-resolution images that contain a large amount of data, resulting in a large file size. This can be problematic for users with limited data plans or slow network as it takes longer to download and can be costly. to fix this issue, consider reducing the size of all your images. This involves making them physically smaller, reducing colored data, and compressing them further, which works well in small screens. However this approach is used universally, users with big screens will end up with low quality and enlarged images.
HTML allows us to deliver different image file to different screen sizes. We can create multiple image files and include them as options to hour HTML code. then the browser and the operating system(OS) takes into account the device's hardware capabilities and network speed to decide on which image to download.
To begin, start with the basic code of loading the image on a webpage. Use an image element with the source attribute that points to the image file, along with ALT text, width, and height. To support different screens, create copies of an image with different resolutions and inform the browser about these options. Then, the device can choose which image to use based on factors like screen density, network connection and user settings. Even if someone has higher-resolution screen, the browser can opt to download a lower-resolution image. 
To demonstrate this, there are four copies of a photo at different widths: 480, 960, 1440, and 1920 pixels. Duplicate the basic HTML code for displaying the image to make changes and compare the results. write code in a usual way, which works well with older browsers and include source attribute pointing to the 1X version of the image, ALT text, Width and Height.
To provide the browser with choices, add the source set attribute. Inside it, list the images on offer, separated by commas. Each entry includes a URL to the file, the resolution (e.g 1X, 2X, 3X, 4X, 1.5X), and so on.The browser will then swap out one version of the image with another based on what it considers best. This technique is ideal for handling different image sizes for retina and high DPI screens 
This is similar to the previous one but instead of specifying the pixel density like 1X, 2X etc, indicate the width of each file: 480w for 480 pixels wide.
The browser now decides which image to show based on device density and viewport width. this could lead to a problem where the chosen image does not fit the layout you want. The browser makes the decision early in the loading process, before it knows the CSS or layout details. It does not know the size of the box where the image will go.
If we know the image will be much smaller than the whole page, we should give the browser more information to make a better choice. Use the sizes attribute in HTML to specify which image to use at different breakpoints. this way, the browser can download the right-sized image for your layout. HTML has powerful options like src set where we can provide a set of images for different resolutions or let the browser choose based on density and viewport width. The sizes allows us to specify how much of the viewport's width the image will take up at each breakpoint. by providing this information in the HTML, we help the browser make intelligent decision, considering network conditions and user preferences.

# Figcaptions and figures
First, show a picture and add a caption to it. Use the figcaption element to wrap the text and designate it as a caption. then put the image and caption together in a figure element. this gives the browser more information about the content, like the relationship between the image and the caption. it is not a regular paragraph or a generic div. this way search engines and AI can understand that these two pieces of content are connected. 
figures can be used for more than just images.e.g use them for interactive graphics. Place it in the same spot as images in the code. The figure and figcaption elements are really useful for anything that serves as a visual illustration or a demonstration of a concept that needs a caption.

# Working with media
 # working with audio
The audio element is different from the image element because it has both the opening tag and closing tag. This makes it more modern and gives it more power and flexibility. just like the image element, we use a source attribute to provide the URL of the audio.
"<audio controls src="audio.mp3"></audio>"
There are different types of audio file formats like MP3, which are not useful on its own and we need to let the browser know that we need it to provide controls like button, timeline and volume control. Using the built-in controls is optional. Instead of using the built-in audio controls, we can create our own controls using JavaScript and HTML media element API. We will add the controls attribute and if the attribute is present that means now there is an audio player on the page. This allows us to play, pause, adjust the volume, see the time and navigate through the timeline. This audio element demonstrate the power of HTML, providing a range of functionality without having to build from stratch.
The are other attributes that can be used with the audio element too. e.g "loop" will make the file repeat from beginning once it reaches the end. "Autoplay" can automatically play the audio as soon as the page is loaded, but be cautious with this one as most people dislike it when audio plays on the web browser without their consent.
The reason the audio element has both the opening tag and closing tag is because the source element can be used to specify multiple audio files, similar to how the picture element is used. 
This can be helpful if a new file format is used that is not supported by all browsers while providing fallback to older ones. to do this, remove the source attribute from the audio element and place it on a separate source element. This accomplishes the same outcome as the previous example but allows for addition of other source elements with alternative audio file formats.
