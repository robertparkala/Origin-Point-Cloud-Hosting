# Blue-Origin-Cloud-Hosting

Responsive Web Design Projects - Building a Cloud Hosting website. Use HTML and CSS to complete this project.

The goal is to create a fully responsive website for a cloud hosting service, modelled after Heroku.com. Since this project is also a part of the 100daysofcode challenge all of the additional notes for it will reside in the 100 days of code repository which I have forked. File to look for > log.md. 

PROJECT LOG

#Day 1: October 28, 2020

**Today's Progress**: Started a new project called Blue Origin Cloud Hosting, added HTML structure and css styling to navbar, showcase section and submit form.

**Thoughts:** It's the first day of this challenge but I've been learning HTML and CSS for exactly a month now. I'm seeing progress in relations to understanding classes better when going through my HTML structure and am thinking in more complex terms when it comes to CSS. For example I feel more confident now with flexbox, grid and also relative and absolute positioning.

A modern website with CSS, Flexbox, Grid, Animation, Span, Column, Rows

Creating an index.html and styles.css. and a boilerplate HTML content.

We used cdnjs.com font Awesome and copied this into our head element

Also, installed a atom-live server package because then it’ll automatically update my HTML preview on the web browser.

BASE CSS INPUTS

For example we set the body font-family to what we imported, color and also a more spaced out line height. We make sure that the lists are not bulleted and the anchor tag links don’t have an underline and text decoration is set to none and color.
For headings h1 and h2 we change the font weight to 300 for it to be a bit lighter also space out the line height and set a new margin of 10px to top and bottom and 0 to left and right.

MAKING A FLEXBOX CONTAINER CLASS

I don’t want to add a flex display to the container itself so I’m adding a utility class called flex. Remember how to bootcamp showed you how to do this as well.

NAVBAR LINKS

Setting the navbar links as in class navbar ul to display flex

SHOWCASE AREA

We’re using the container class again to maintain the specifications from our CSS and now adding grid so we can have similar functions as we did with flex.

SHOWCASE AREA USING GRID
As we can see, that by using the grid utility class in the container we are making it possible for us to style the container using the display attribute GRID. Now, by setting that to just GRID nothing happens, but we also need to specify the grid-template-columns and their width. In the screenshot we can see that each of the DIVS in the container is now changed into a grid item similar to a flexbox item and the first DIV is the size of 300px and the next one is fitted into a 200px container.

SHOWCASE AREA CARD WITH FORM

We pushed the form down with the relative position and then with the specification top and also gave it a height of 350px which gave us the scroll bar which we don’t want. What’s happening is we’re overflowing that element and we need to adjust it.

SHOWCASE INPUTS

Since we want to style the inputs that we created for the form but NOT the button itself we’ll create the style specification above and style the types TEXT and EMAIL thus targeting the values NAME, COMPANY NAME and EMAIL.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 2: October 29, 2020

**Today's Progress**: Today's main draw were flexbox and grid. Created the stats section, CLI section and bottom Cloud and Read more section.

**Thoughts:** CREATING THE STATS AREA WITH GRID

Moving on to HTML now and creating the STATS area. Let’s break it down. First we created the section and containers because we don’t want the content to stretch out all the way and end where the rest of the stuff ends. We’ll have h3 and some utility classes for text, margin classes. my-1 is the margin class for Y axis. Those are utility classes so we don’t need to add so much CSS like margins and paddings on the element itself. Three areas for the stats, Deployment, Published and Projects.

Also, we’re adding 3 grid columns so we need a grid-3 class. my-4 is a larger margin class

i tag is for ICONS. Text-secondary is for our text color. Fa meaning Font Awesome and 3x meaning 3x times larger font.

We used the grid class remember, and what that’s doing is taking the firs two grids out of the three and splitting them into two. Now, we need to change that to three in the grid class to get them to align nicely.
We don’t want to use the original GRID class but we’ll use the one we intended for the icons.

CREATING A NEW CSS FILE TO SPLIT THING UP

Now we have the utilities in a new css file and also we added a link to our HTML to link the two css files. SO COOL!
Utility styles are for styles that are to be repeated throughout the page and basics styles reside in the style.css file.

ADDING MARGIN AND PADDING CLASSES

We added my-1-5 margin classes and set the margin for my-1 to 1rem for the H3 and my-4 to 3rem for the grid.

MODIFIYING THE STATS ICONS AREA

To set the STATS heading in the center and give it a max-width we will move it from a single line text to a max-width of 500px in the center of the page.

Changing the font-size to 35px. NOW, what I didn’t know is that you can move withing classes, for example, we are targeting the H3, that is in the grid class and is also in the stats class. WOW!

CREATING THE LOWER CLI WITH GRID

This is some clever work here. Pay attention that we are first using the CONTAINER class for everything because we already modified it and we can reuse the class. Now, also, we’re using the GRID class since we already have that on hand as well. WOW WOW WOW!

ADDING ANOTHER SECTION FOR READ MORE

Now this is interesting again. We’re creating another section and a class cloud so instead of adding the blue background color right on cloud, we’re adding another bg-primary class so we could use our variable with the primary color. Now, we’re going to center the text and we have a heading h2. Specific size class for headings, like lg = large.
Paragraphs are going to a bit bigger using the class lead.
Now, adding in the button with the anchor tag and also the styling is going to come from the same btn class we used before but we’re going to use the btn-dark and style that.
Also, we currently had the one DIV and we’re going to be adding in a second DIV as the image so we can take advantage of the two grid spaces we have witch are laid out with 1fr

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 3: October 30, 2020

**Today's Progress**: Today I finished the supported languages and footer sections. Added social media links and media queries for both tabled and mobile.

**Thoughts:**

ADDING SUPPORTED LANGUAGES SECTION

Created a languages section and h2 with the medium class, with text center and we’ll do my-2 for margins. Feels like we’re using Bootstrap but it’s actually thorough and custom CSS. We’re going to use flex for this because we want to align them into a row and each one will be wrapped in a card and h4 and an image underneath. Images/logos.
CSS that we’re adding .languages .card with text align and margins for top/left side bottom and right side. And adding onto the flex we’re adding flex-wrap and set that to wrap.

Increased h4 size and margin bottom. Also, set the hover attribute to the card elementso that the images would move up a little bit and that’s the transform property on the Y axis and up means a negative value on the axis.
For the smoother effect we’ll add a transition onto the transform property with the ease in.

FOOTER SECTION

Creating the footer bar starts with a footer tag with a class of bg dark and padding py-5
Container is going to be grid 3 and we’ll have a div with the site name in the h1 and a paragraph with the Copyright, &copy gives us the copyright symbol. That was the firs grid item
We’ll do a NAV tag with the ul and links to Home, Features and Docs and a Privacy policy but I didn’t want to create links that go nowhere.
Final DIV as the grid item will be the Social. With font awesome the social media icons will be FAB abbreviation.
Also, we added in to make the social media link anchor tags white and spaced out our social media icons with margin from left and right.

ADDING MEDIA QUERIES TO MAKE THE PAGE RESPONSIVE

Adding two separate media queries in our style.css. First one for tablets and under and the second one for mobile. For Tablets, anything under 768x will be styled here. For mobile we want to capture anything under 500px. For the menu that’s going to be fine on tablets even if there’s more items but for mobile we’ll change things up.

In mobile Navbar height set to 110px, to put the menu items under the logo. Navbar we have a class flex, so it’s a row by default so we’ll set it to column with flex direction which will put the logo and the UL on top of each other. For the navbar UL we’ll add padding and a transparent background.

Style all the grids first and I want to stack everything, so tablets and under. Instead of two and three columns I want everything in one column. Grid classes first! Setting the grid template columns to 1fr so it would take up the entire column and in the CLI area we have two rows so we’ll set the grid template rows to 1fr as well for it to take up only 1.

Initially the showcase is 400 px and we’ll set the showcase height to auto so it would take up the entire space.  So to form wouldn’t be on the text. Showcase-text we’ll align to the center and we’ll push it down with the margin top for 40px.
I want to move the showcase form to the middle and we’ll use the justify-self: center; to do that. We’ve used justify content a bunch so that’s going to be on a flexbox or a grid container.
Justify-self we use on an actual grid or flex item to justify just that item. Margin to auto. Now the form’s in the middle.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 4: October 31, 2020 Happy Halloween, boo!

**Today's Progress**: Today got an early start and I thought that I’d first spend an hour or more on Stack Overflow answering some of my first questions ever. As far as coding today, I created the Features page, which is the second of the three pages that are going to be on it. Added the navbar, features heading, img and footer.

**Thoughts:**

CREATING THE FEATURES PAGE

Created a new file features.html and copied all of the content from index.html and we’re keeping the nav bar, footer. Removed everything UP from Footer and until Showcase included.

This page is not going to be as complex because we already have all the helper classes ready and most of the elements.

Now, we’ve added the Head section  and a subsequent DIV, that also is styled with the container an now a grid attribute. We’re using the same bg-primary and py-3 classes to style our background and padding. Also, using the XL class for H1 and LEAD for our paragraph.
We entered an image as our second grid item.
Then we added the Features CSS for the picture and made it smaller and pushed it to the end of the container grid with justify-self: flex-end;

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 5: October 31, 2020 Happy Halloween, boo!

**Today's Progress**: Finished the Features page with subhead and subhead grid.

**Thoughts:**

CREATING THE SUBHEAD AND SUBHEAD GRID

Created the features sub head section and a new container grid. Added heading H1 with a class of medium and paragraph with some dummy text. Added a new image server 2.

Modified CSS to push the subhead image to the container end and modified the width to be a bit bigger than the features server logo.

We’re making a grid of cards but we’re also adding the FLEX because we want to align these items using flex.
Adding an icon with Font Awesome and then we’ll add a paragraph and add lorem30 dummy text. Now we need 6 of those divs and just modify the icons with font awesome.

We’re adding special styles so that the grids would not be sitting next to each other. So specifically, in the features main we’re targeting the icons and adding a margin to the right to push then away from the text a little bit.

For the grid itself we’re going to do some spanning but before we’re going to set the grid-3 onto the div container class to give it 3 columns and add a bit of padding to the features main in CSS.

Now, we want the firs grid element to take up (span) one row and span three columns. Also the second element to span one row and take up 2 columns. We can do that by addressing the first child in the grid and subsequently with the nth-child(2) we can address the second child. WOW, totally now stuff here!

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 6: October 31, 2020 Happy Halloween, boo!

**Today's Progress**: Finished the Blue Origin Cloud Hosting Website, which is now responsive across platforms.

**Thoughts:**

CREATING THE DOCUMENTATION PAGE

We copied the features page as a boiler for the docs.html and also changed the section class from features-head to docs-head.

DOCUMENTATION MAIN

The docs main is going to be a similar container grid class DIV that has second DIV with the card class in it. We’re adding a heading H3 and a navbar with an unordered list with list items and also a second heading with an H3 and a similar list.

INTRODUCTION

We create another DIV with the class card an since it’s housed in a div container grid then it’ll format into 2 columns of 1fr. Inside the card we have a heading h2 and a paragraph with an alert alert-success DIV that houses a font awesome icon. 

LINKS AND LISTS 

We added a heading in the card and a paragraph. Under the paragraph we created a link with an <a> tag. And set it up as a button Install CLI. Now, under the button we added the Requirements heading h3 and formulated those requirements into a unordered list. 
Under the list we added another H3 and a Paragraph with a <pre><code> tag that allows us to add in the terminal code lines. Make sure to read more about this!

We’ll add a margin to the docs main heading and we will also modify the docs-main .grid to take up 1fr for the first grid item and 2fr for the second grid item. 

ALERT SUCCESS AND ERROR

Now, we’re styling the Alert class and it’s similar to the Bootstrap alerts where you can see SUCCESS, DANGER etc. 

We’re setting the alert class color to light color with the custom properties (variables)

STYLING THE CODE IN <PRE> TAGS

We’re making the pre tags look like they would be off of a real documentation page.

STYLING THE PRIMARY COLOR OF LI ITEM

We’re setting a text primary class to the Introduction LI item. Using the bg. background colors and btn colors and copying down but changing the background color to just color to make the Introduction blue. 

MAKING THE INNER PAGES RESPONSIVE 

We added the features main grid and the docs main grid to the 768x. Now the Features grid starts to stack up. Now we want to center  our images on both the features head, subhead and on the docs head. Now we’re working on the Features grid span and we’re targeting the grid’s first child and the nh-child(2)
and setting the grid-columns to 1 so they would stack underneath each other.

ANIMATIONS

We’re creating animations in our style.css under Footer with @keyframes and adding slide-in’s to certain elements for right, left, top and bottom. We’re actually manipulating translate X and translate Y.

We want it to start off screen and it will start negative 100% on the left with this keyframe.

And end up in it’s normal position 0 at 100%

Same thing for the slide in from the Right. Now it will start at positive 100% to the right and will return to its original position 0 at 100%
We’re doing the same with Top and Bottom but remember that now we’re manipulating the Y axis and returning the element back to its position in the X axis. Super cool stuff here! 

Slide in from the Left is going to go in the Showcase Text (which we need to create) and Slide in From Right will go on the showcase form. We specified the animation action from our keyframes, then the duration and what kind of movement. Now we want the STATS to come out the bottom.

DEPLOYING TO NETLIFY

Deploying to Netlify and creating a Git Repository there.

ADDING THE FORM FUNCTION FROM NETLIFY

So that our form would actually work on our home page. Adding this to our index.html

ADDING THE SPAM FILTER

Recaptcha or Honeypot. Recaptcha would mes up our layout bot we’re adding the honeypot so if you’re a bot you’ll fill it out and if you’re a human you wont. 

Also we’re adding in the paragraph wit the hidden like so. This is going to hide the honeypot based on the hidden class. Also, we’re going to add CSS to style.css and hide the visibility and since it will still take up space, we’ll set the height to 0.

NOW WE’RE SET TO DEPLOY

Opening up our VSCode terminal with command + tilde (which is right under the escape button) and adding 
git init. GitHub's got our repository. Now, we’re going to Netlify again and creating a new repository. Following the steps that are laid ouf by Netlify. Deployed at https://blue-origin-cloud-hosting.netlify.app/

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)
