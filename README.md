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
MP3s are widely supported in modern browsers, while OGG had some advantages but did not gain much popularity. There may be a new format on the horizon, similar to AV1 video file format, but not widely available. for this reason, there is no second audio format recommended at the moment. nevertheless, it is important to understand the syntax for supporting multiple file formats, as it was crucial in the past and will likely be useful again in the future.
Create multiple files and list them in separate source elements, and the browser will use the first compitable file in the list. 
furthermore, it is possible to provide fallback text within the audio element, which will be displayed if the browser does not understand the audio element at all. This demonstrates the resilience of HTML, where a single set of code can cater to a wide variety of browsers and provide a suitable user experience. The audio element is an excellent tool for embedding audio files and a player on the webpage.   
 
 # working with video
The web has completely changed how we connect and share things, including movies, TV shows, and even teaching. Thanks to the power of the web, we can now easily put videos on web pages using HTML video element.
Just like the audio element, the video element has an opening and closing tag. to display a video, use the source attribute to specify the video file. and if the controls attribute is added, the browser will automatically create a video player.
The first problem has to do with video encoding. For this example, a video file has been created with 480p resolution, compressed using the H.264 codec, and delivered as an MP4 file. 480p means the video has 480 lines of resolution and is 720 pixels wide by 400 pixels tall. It is not HD or 4K, just standard quality. The H.264 codec was chosen because it is widely supported by browsers.
Just like image formats like PNG, SVG, JPEG or GIF, there are different codecs that can be used to encode video files. Video files contain a lot of data, and if not compressed, the become too large to be efficiently transmitted on the internet. Internet videos, therefore, use a mechanism to compress all the data to smaller packages.
There has been various codecs developed throughout the years, such as Real video, Sorenson, Windows Media, Flash, and H.263. From 2015 to 2020, H.264 was the dominant codec used by most people, however H.264 is not open source, it is a patented codec owned by consortium. They charge licensing fees for every device, Operating Systems, Browser, Camera, or anything that wants to record, compress or play H.264 files. And now, they are planning to charge even more in H.265.
In contrast to freely available image formats such as JPEG or GIF, H.264 is proprietary, prompting the inquiry: should video codecs be subject to distinct treatment? Unlike HTML and CSS, which are unpatented and openly accessible, H.264's proprietary nature raises concerns. To tackle this challenge, significant endeavors have been invested in developing an outstanding, open-source video codec devoid of patents.
Reports indicate that the outcome of the WebM versus AV1 discussion remains uncertain. Recent advancements hint at AV1 potentially surpassing H.264 as a video codec and being free from royalty charges. The HTML video element permits the incorporation of numerous source files, facilitating the concurrent utilization of diverse codecs like H.264, WebM, and eventually AV1. This adaptability also applies to audio and image elements, allowing for the specification of multiple file formats using the source element with suitable attributes. The browser will play the first compatible file it identifies.
Now, let's tackle the second obstacle. Imagine there's a 480p video file suitable for users with smaller screens and slower internet connections. However, for those with faster connections craving high-definition (HD) or 4K content, a larger file is necessary. Regrettably, HTML lacks a built-in method for delivering varying video sizes based on network conditions. This limitation arises from the desire for devices to dynamically adjust their resolution choice, factoring in variables like network speed.
To address this challenge, major streaming platforms such as Netflix, Hulu, HBO, YouTube, and Vimeo employ adaptive bitrate streaming. This sophisticated technique involves a server farm of transcoding robots that ensure seamless transition between different resolutions as users stream videos.
Given the complexity involved, it's common for websites to opt for embed codes from video hosting services rather than directly employing the video element. This decision is often made to streamline the process and capitalize on the capabilities offered by such services.
 
 # Working with Captions and subtitles
It's remarkable how websites can incorporate audio and video elements, yet accessibility remains a challenge as not everyone can hear or understand them consistently. Some individuals may be deaf, while others might experience intermittent hearing issues or difficulty comprehending content due to various factors. Even for those who can hear, listening isn't always feasible.
For instance, you might wish to watch a video but cannot use speakers or headphones in certain settings. Alternatively, you might be listening, but the speaker's accent or fast speech pace poses comprehension challenges. You might even be in such a situation right now, relying on captions for video content. Fortunately, the web empowers content providers to offer information in multiple formats simultaneously.
We will utilize the track element linked to a text file to incorporate captions into the video. This element enhances the video player's capabilities, enabling viewers to toggle captions on/off or switch between different subtitle options. On the web, a file format known as ibvtt (web video text tracks) will be employed. It's a straightforward text file with a vtt extension, adhering to a specific convention for providing information. Each line of text in the file is accompanied by a time code indicating when it should appear in the video.
To display these captions on the video, insert a track element within the video element. Similar to the source element, it's one of the options the browser uses to render the video player. On the track element, use the source attribute to specify the file, the kind attribute to indicate that it contains captions, and a label attribute to display the caption option as "English" in the player. Additionally, use the source lang attribute to specify the language and add a default attribute to make this track the default choice when captions are enabled.
Upon insertion, a captioning icon appears. Clicking on it reveals options for turning captions off, enabling automatic captioning, or selecting English captions. The label "English" appears due to the label setting. To provide a Spanish translation as a different subtitle option, another vtt file for Spanish can be created, and another track element can be added to the same video element. This time, set the kind attribute to "subtitles," the source lang attribute to "es" for Spanish, and the label attribute to "Español." As a result, a second choice for subtitles, including Spanish subtitles, appears in the list.
The kind attribute also offers other options. For instance, using "descriptions" enables the creation of a vtt file describing the video's visual elements. Users can select a track that reads these descriptions aloud, making the video more accessible to the visually impaired. Another option is "chapters," which provides a text file listing different sections of the video, allowing users to navigate to specific parts.
In the subsequent section, the utilization of platforms like YouTube or Vimeo, where caption files can be uploaded to provide similar functionality, will be discussed. Captions and subtitles are not only impactful but often legally required. Including them enhances accessibility and inadvertently broadens your audience base. So, incorporate captions and witness your traffic increase!

# Embedding media via IFrames.
Embedding refers to taking content from one site and placing it within the middle of another site's page. 
There exists a broad spectrum of content that can be integrated into a webpage. For instance, this includes a map from Google or Mapbox, a code demonstration from CodePen or Glitch, or even a presentation slide deck from Speaker Deck or Notist. It's a common practice to embed intricate content from a service that manages the technical complexities. Instead of grappling with the development of a mapping service, a slide deck system, a code demonstration platform, or an adaptive bitrate server, one can rely on the toolkit provided by others to handle these tasks. All that's needed is to embed the outcomes onto a website. So, what level of HTML proficiency is required to streamline this process?
You don't necessarily have to grasp every detail because YouTube's engineers have already handled it. However, with your newfound ability to interpret HTML, you can recognize a lot. For instance, the iframe element features attributes such as height and width that are adjustable. The src attribute is utilized to designate the source of the video file.
Although iframes offer versatility, it's essential to factor in security concerns when incorporating code from external websites.
When utilizing a pre-configured content management system (CMS) such as WordPress or Drupal established by someone else, it may not be straightforward to directly copy and paste arbitrary embed codes from external sites. Typically, these CMS platforms have specific methods for allowing URLs or shortcodes only from trusted sources. For embedding items like YouTube videos, it's advisable to seek guidance from someone proficient in effectively utilizing the CMS.
Additionally, when constructing a website, it's crucial to consider security implications associated with the iframe element. If multiple individuals will be contributing content to the system, indiscriminately permitting all iframes without considering security measures is unwise. However, if you are the sole contributor of videos to the website, there isn't much cause for concern.

# HTML Content Identification
The internet spans the globe, encompassing diverse languages spoken by people worldwide. HTML offers mechanisms to specify the language of your content. By configuring these settings accurately, search engines can discern the language of websites. Spell checkers will apply suitable dictionaries, and when a browser reads content aloud, it will pronounce words correctly. It's crucial for computers to identify the language of the content they process.
The lang attribute serves to designate the language of a webpage. If the entire page is in one language, the process is straightforward. Simply set the language on the main element encapsulating everything else, typically the HTML element. This may only need to be done once, such as in a template file that applies universally across the site, but it's crucial not to overlook this step!
For instance, using "en-US" in the lang attribute indicates U.S. English, while "en-GB" denotes English in Great Britain. This distinction is significant for functionalities like spell checkers. Consider whether you prefer "color" spelled with or without a "u". In the U.K., it includes a "u". Therefore, specifying the preferred dictionary and pronunciation is essential. Rather than opting for a generic "lang=en" for English, it's advisable to be more precise.
The lang attribute offers various options beyond indicating language or regional variants; it can also denote other characteristics such as the writing system utilized. If your webpage features multiple languages, specify the language for each segment of content using the lang attribute on relevant elements. For example, if the majority of the page is in Mexican Spanish but includes block quotes in Nahuatl, apply lang="es-mx" on the outer HTML element and lang="nah" on the block quote elements.
Additionally, it's vital to specify the content's direction. While most languages read from left to right horizontally, some follow a right-to-left flow. Utilize the dir attribute to indicate the direction, which can be applied to any element. If all content on your page shares the same directionality, define it once on the outer HTML element.
To wrap things up, do not forget to set the charset for your project. What is that? Well, each language uses its own set of characters or alphabet. In the past, computer character sets were limited and mainly focused on the Latin alphabet. You may have heard of ASCII, which was created in the 1960s and consisted of only 128 characters from English typewriters. Nowadays, Unicode, particularly UTF-8, is widely used. It is like a massive specification that encodes content to support a vast range of characters, scripts, and even emojis. Unicode started with around 7,000 characters in 1991 and has now expanded to over 137,000, aiming to encompass all languages, scripts, and communication forms like Braille and musical notation.
Inform the browser about the character set being used. Otherwise, things can get pretty strange if the computer expects one thing and receives another. 
To specify the charset in HTML, simply include a meta charset tag that equals UTF-8. Place this meta element within the head element on every page of the website, which will be explained further in the chapter eight: HTML Integrations.
Initially, the web made a lot of assumptions about the languages and scripts people would use, and it only supported a few. Over the years, extensive efforts have been made to ensure everyone's inclusion. By defining the lang, dir, and charset for a project, you contribute to a more inclusive future for the web.

# HTML Generic elements, Div and Span
Several HTML elements have been discussed for various purposes, but what about situations when a specific element is needed that doesn't exist? Sometimes, there's a necessity to group elements or highlight a phrase without a predefined semantic meaning. Other times, targeting a specific part of the DOM with CSS or Javascript is required, even if it lacks inherent semantic significance. In such cases, two reliable elements are at our disposal: div and span. If you've worked as a developer writing HTML, chances are you've encountered these elements before.
Before 2010, prior to HTML5's introduction with its helpful semantic elements, divs were heavily relied upon for a multitude of purposes. Divs were utilized for creating sections, sidebars, and various other structural elements. Even today, people tend to excessively use divs and spans in HTML, often without further consideration. This course aims to underscore the importance of semantic HTML.
Technically, one could use divs and spans for everything. Some developers even place titles within divs and make spans simulate buttons. While HTML won't produce an error, and browsers will still attempt to parse the page, it's not considered best practice. This approach can negatively impact user experience. We strongly encourage avoiding excessive use of divs and spans for minor elements and instead opting for the appropriate HTML element that serves the purpose.
However, there are instances when a generic element is necessary. Div is a block-level element, whereas span is an inline element. They essentially have no inherent function until CSS or Javascript is applied to them.
Consider a simple article enclosed within an article element, comprising a headline and four paragraphs. When working on the CSS layout, there's a need to group these paragraphs together to apply a background color exclusively to them, leaving everything else unaffected. To achieve this, introduce a div with a class called "boxes". By targeting this box class with CSS, the desired changes can be achieved.
Now, imagine a specific phrase within the text requires targeted treatment, such as being written in Spanish and needing its language attribute updated accordingly. In this scenario, use the inline element span to delineate the desired phrase. Both div and span can utilize various global attributes like class, id, lang, and aria roles.
Div and span serve as useful fallback options when no other suitable element exists. Remember to use them judiciously.

# Unit 8: HTML Intergration
# HTML Intergration
The comprehensive coverage of HTML, including its elements, attributes, roles, and tools utilized to structure content on websites or web applications, has been addressed. HTML not only plays a pivotal role in defining these elements but also serves as a fundamental component of the web itself.
When accessing a website, users typically open a web browser or web view and input a URL. This can be done by manually typing it into the address bar, clicking on a search result or link, or through an app. Regardless of the method, a URL is involved. In response, the web server sends back the specific HTML file associated with that address.
In the earlier stages of the web, everything necessary to display a webpage was contained within a single HTML file, alongside images. However, with the advancement of technology, the process has become more intricate. Text is often stored in databases, and multiple static files are dynamically combined in real-time, tailored for each user. Visual styling is stored in CSS files, JavaScript in separate JavaScript files, and additional files are used for images, video, audio, and advertisements.
While modern web pages typically consist of a combination of different files, the underlying process remains consistent. Users visit a URL, triggering a request for an HTML file, which the server then returns. The browser interprets the HTML file and executes its instructions accordingly. This initial HTML file serves as the central hub for subsequent actions once the site loads.
Upon receiving the file, the browser immediately begins parsing it and following the instructions sequentially. Additionally, the file may contain references to other necessary files, prompting the browser to request them as well. Once all required files are obtained, the browser proceeds to execute their instructions, resulting in the rapid generation of the webpage.
Now, let's explore the structure of the entire HTML file. While the build system or CMS may not present a single file containing all the code, there are typically templates or theme files that dictate the content.
Within the HTML file, several critical components are necessary for every webpage. Firstly, it should commence with a doctype statement, signifying the HTML file's era. By including this, it signals adherence to modern web standards. Subsequently, the entire content is enclosed within an HTML element, delineating that all content within it is HTML. The HTML element is opened at the top and closed at the bottom.
Furthermore, certain specifics about the webpage, such as the language and content flow direction, are declared at the outset. These specifications ensure clarity for browsers and users alike.
The HTML file is further organized into two primary sections: the head and the body, marked by the head and body elements, respectively. The head contains metadata essential for the browser but not displayed on the page, while the body encompasses the visible content, composed of various elements discussed in this course. The body serves as the primary area for webpage content and interactions.
In summary, the doctype declaration, HTML head, and body elements constitute the foundational elements of every webpage.

# Document Header
Within the head section of a webpage lies crucial information that the browser requires to understand the website. Recall the importance of specifying the character set? This is where it becomes relevant.
The character set is not intended for user visibility but rather for the browser's interpretation. To convey this, the meta element is utilized. It's essential to place meta elements exclusively within the head section as they furnish metadata about the page. For instance, to define the character set, employ the character set attribute and set it to UTF-8. Before exploring other functionalities that meta tags offer, let's begin with an element that's mandatory on every webpage: the title element. It's worth noting that the title element doesn't display visible content.
The webpage title appears on the browser tab or bookmark when saved. It's also the name displayed under top sites upon opening a new browser. Essentially, whenever the browser references this page, it uses the title defined in the title element. Now that the essentials of every HTML page are addressed, let's delve into what else can be managed within the head section.
The meta element serves various purposes. One common application is to notify the browser that the layout has been optimized for small screens, making it a responsive website. Without this meta tag, the browser assumes the page follows an older layout designed for desktops, necessitating scaling down for mobile devices.
Furthermore, it's beneficial to incorporate a site description, visible in search engine results. Ever wondered why specific information about a website appears in a Google search? This is where that data is extracted from. Additionally, the meta tag assigns a name to the webpage when saved to the home screen and specifies a tile image and background color. When a link is shared on platforms like Slack, Asana, or Twitter, it transforms into an appealing card, facilitated by meta tags. Numerous techniques utilize the meta tag to enhance and refine the user experience of a website.
The link element is a vital component extensively used within the head section. It connects various assets to be loaded, such as CSS files, fonts, and favicons. To inform the browser about the asset type, the rel attribute is utilized. Furthermore, the href attribute specifies the URL for the asset. For instance, a link to a stylesheet would appear like this, indicating the rel attribute as "stylesheet." The same format applies to a link to a favicon. Additionally, a link to preload a font file can be included. It's important to consider the order in which the browser loads files, prioritizing items that need to load first at the top.
The script tag is another frequently used element within an HTML document's head. It directs the browser to load a JavaScript file. While it's typically positioned at the end of the document, some also place it within the head section.
In essence, the HTML head serves as a central hub for connecting and configuring various components, ensuring all assets are loaded and sharing page information with other sites and platforms. It acts as the headquarters for ensuring the webpage starts off effectively.

# Content structuring
We just covered what could happen in the document head. Now, let's talk about the typical structure inside the body. There are six important elements to understand:
1. Main: The main element is used once per webpage and tells the browser where the main content is located.
2. Header: The header and footer elements mark the header and footer areas on the page. Do not confuse header with head though. Head is where the file's metadata lives and is not displayed to users. Header is used for site headers, article headers, and headers within the content. A header is usually found at the top of most web pages and may include a logo, site name, and navigation.
3. Footer: The footer signifies that there are extra things to convey, regardless of its position on the page.
4. Article: An article often starts with a title, subtitle, author's name, and publication date, which can also be considered a header. Many web pages end with a footer at the bottom, containing links, copyright information, and additional details about the company. However, footers can also appear elsewhere. Some articles begin with metadata like hashtags or share buttons, which are suitable for a footer element. The article element wraps around any type of content unit, whether it is a long written article, a short snippet, a teaser card, a tweet, or even an app element. It represents a standalone unit of content.
5. Section: The section element is used to mark sections of content. For example, in a long essay with subheadings, each segment can be wrapped in a section element. It is also useful for dividing different topic zones on a website. Each section typically starts with its own headline.
6. Aside: Lastly, the aside element is for content that is off to the side, like sidebar information or additional details that accompany an article but are not part of its main flow. Advertisements can also be marked as an aside. Although the position on the page does not matter, the semantic meaning of these elements is crucial. The visual layout often conveys meaning, and these HTML elements help transfer that meaning from the design to the content.
