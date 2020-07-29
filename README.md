# Learning html Elements
Today we further learned about the various HTML elements, Entities and Semantics,Mentioning IDs and Classes for the HTML Element, shortcut and Emmet representation for creating HTML Elements.

## The `meta` tag

One important html element is the `meta` tag. Located in the `head` section of the html file and therefore invisible to the site visitor, it is visible to the browser and contains information that can sometimes be crucial for a site's potential popularity. It also optimizes the site dimensions to fit the screen of the device on which it is viewed. Following are some examples of `meta` tags:

`meta charset="UTF-8"` - it determines the character set of the website, in this case Unicode Transformation Format with 8 bytes
`meta name="author" content="John Doe"` -it specifies the name of the website's author

## html Typography

It determines the way in which content is to be displayed/written

## html block vs. inline elements

The block elements are always displayed in a new line and take up the full width of the page, while the inline ones do not start in a new line and occupy only as much width as necessary.

## The `div` tag

The `div` tag is a block-level, non-semantic element which serves as a division within the html document that can be easily styled by using CSS and JavaScript. It is virtually a universal tag that can be used in any context and include any content.

## class vs. id

While the class attribute can be employed in describing and styling many similar elements, the id one is ONLY to be used for individual elements. `class` is noted as a dot, `.` in CSS, while `id` is represented by a hash tag, `#`

## Emmet Abbreviations

The Emmet Abbreviations make the life of the Web Designer/Developer just so much easier, as they substantially simplify the code writing process when used in the Visual Studio Code. Here are some examples:
`ul#main-nav>li*5` - generates an unorganized list with the `id` main-nav and five list items
`ul#main-nav>li*3>a ` - generates an unorganized list with the `id` main-nav, three list items and a link in every one of them
`#footer>p{Copyright &copy;2020}` - generates a footer element with the copyright info inside it
`#contact.card>h3{Contact Me}+ul>li{Address:...}+li{Phone:...}+li{E-mail:...}` - how about writing all your contact data in ONE single line? And seeing the title and the entire list come out of it!

## Entities

Because in html some characters are reserved, they need to expressed through entities in order to be properly displayed in the browser. For example, the ">" sign is used in closing tags and if the intention is to actually show it as a greater than sign, let's say 5>3, it needs to be done through an entity. Here are some examples:
`&lt;` or `&#60;` is "less than", <
`&gt;` or `&#62` is "greater than", >
`&copy;` is "copyright"
`&reg;` is "registered"
Currency signs are reserved characters as well, therefore they need to also be expressed through entities:
`&cent;` is "cent"
`&dollar;` is "dollar"
`&yen;` is "yen"
`&pound;` is "pound"
`&euro;` is "euro"
What about card suits, are they also reserved characters? Well, yes:
`&spades;` is "spades"
`&clubs;` is "clubs"
`&diam;` is "diamonds"
`&hearts;` is "hearts"

## Self-closing tags

This kind of tags do not require an end tag, marked by the sign `/`, good examples include the aforementioned `meta` tag and the one for "image", `img`

## Creation of a website with the CSS style already provided, insert the proper html

At the end we had to create such a website and Safwan explained to us the importance of such elements as `section` and `article`. Glauber and Daniel also showed us an efficient way to insert articles within a section by using Emmet abbreviations:
`section>article*2>(h3{Title}+p>lorem100)` or
`section>article*2>(h3{Title$}+p>lorem100)`