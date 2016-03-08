# The origins of style

Q: When was style first applied to an HTML document?

Right at the beginning.

Q: How?

Browsers. Tim Berners-Lee and the team at CERN wanted a way to interpret an HTML document that made sense to the user. i.e. HTML by nature contains instructions on how to be rendered.

So, HTML is a very basic example of Declarative programming.

# Procedural/Imperative vs. Functional/Declarative UIs

Q: Can someone give me an example of other methods of creating graphical user interfaces? Think about other programming languages. How do they create their own UIs?

Procedural or Imperative programming. Think C/C++. How do you create a UI in that language? Well, you render it, yourself. Each and every aspect of the UI would need to be defined.

Q: Why was a declarative approach to building UIs chosen over say a imperative / procedural one for the Web?

See:

 - http://programmers.stackexchange.com/questions/173354/what-is-declarative-ui
 - http://blog.thinkful.com/post/71644244908/thoughts-on-declarative-and-imperative-languages

# The rise of attributes

The declarative approach to building web-based user interfaces resulted in a plethora of style-controlling elements and attributes that controlled the presentation of HTML documents.

Q: Name as many presentational elements as you can

center
b
i
s
strike
u
small
big
font
blink
marquee
tt
basefont

Q: Name as many presentational attributes as you can

align
border
bgcolor
link
vlink
alink
text
background
cellspacing
cellpadding
valign
width
height

Why are presentational elements and attributes bad?
Are they all that bad?

# The internal workings of style in early browsers

OK, let me set the scene. It's the early 90s. There's no such thing as CSS yet.
You're using Mosaic on your 286 and you're connected to the internet via a 9600 baud serial modem.

You type in your favourite search engine URL: www.altavista.com and hit enter.

- When does a browser start rendering the stream of HTML?
- Why does it do it that way?
- What are the exclusions for this rule?
- When does a browser re-render something?

The highly-abbreviated rules:

1. Start parsing the document as it is being received
2. As an element is 'completed', start rendering the element according to its specifications and attributes.
	2.1 If the element is contained in a <table>, wait for the entire table to finish, and then render.
	2.2 If an image is downloading and it's corresponding <img> element doesn't have width and height attributes, then wait till you can determine the image dimensions. Once the dimensions are known, re-render the image, its container and subsequent elements.
3. Continue till document end.

# Then came CSS

- What is CSS?
- Why was CSS created?
- Why is separating style from content a good thing?
- Why is it a bad thing?
- But, React?!

# So, how is style applied to a document?

- elements and attributes
- `<link rel="stylesheet" href="…">`
- `<style>` blocks
- inline style attributes
- JavaScript .style methods

What order are these processed in?

Author presentational HTML elements and attributes (excl. inline style)
User Agent CSS
Author CSS
User custom CSS
Inline styles


# To sum up

What are the various influencers for styling an HTML element?

What is really going on when it comes to styling an HTML document?


