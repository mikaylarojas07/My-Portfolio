Assignment 1 README file
Mikayla Rojas #101023576

CITATIONS
Phone number input validation adapted from: https://www.w3schools.com/tags/att_input_type_tel.asp, published by Refsnes Data
Media Query integer strategy to avoid gaps adapted from: https://stevefenton.co.uk/blog/2023/05/unintentional-media-query-gaps/, written by Steve Fenton
Profile image code adapted from: https://www.w3schools.com/html/html_images.asp-->, published by Refsnes Data


GUI/INTERFACE
My webpage uses three separate CSS files, each of them linked with a media query so that only one stylesheet applies at a time. 
The stylesheet that is applied to the corresponding html file is based on the user's screen width. 
- style.css for laptop.desktop (screens between 960px and up)
- tablet.css for tablets (screens between 481px and 959px)
- mobile.css for mobile devices, ex, smartphones (screens 480px and smaller)

I chose these dimensions for each view port because they match the typical range of real device widths. 
Another reason is because I am familiar using these dimensions through lecture practice. 

At each break point, elements like navigation links, cards, images, and videos resize using percentage-based widths (fluid design), rather than fixed pixel values. 
This is so that the layout can scale up and down with each viewport range so page content does not get cut off. 
For example, .card elements shrink from their default desktop width to 70% screen width on tablets and 90% width on mobile, and the navigation links change from links on the desktop to buttons on tablet/desktop to remain easy to tap on a screen.
When switching from tablet to mobile, I designed my site so that the button size for the navigation links increases, giving the user larger buttons to click on when on a smaller screen. 

I also removed the hover features for tablet and mobile screens, because a feature that changes the opacity of an element when hovered over does not make sense on a touchscreen device. 
Because I removed the .card:hover effect for tablet and mobile, I also changed the default opacity for the project card elements to 1 instead of 0.7, to increase the contrast for better viewing on smaller screens.

One challenge I faced when defining these dimensions came to my attention during testing/resizing. 
I noticed that when on the edge of a breakpoint (eg, at 959px or 480px), none of my CSS styling was applying at all, and it was as if I had no stylesheet linked. 
After doing some research into these gaps, I then realized that pixels are not always integer values, which was contributing the the gap in styling when resizing along the edges of the breakpoints. 
Since my breakpoints were initially set using whole numbers (eg, max-width: 959px, min-width: 960px), a fractional width like 959.5 would fail to match either condition, leaving a small gap because none of the stylesheets woul apply. 
To fix this, I adjusted my max-width values to include a decimal (eg, 959.9px instead of 959px), successfully closing that gap, ensuring that no width falls outside all three media query ranges (desktop, tablet, mobile).


COLOUR GRADIENTS
My website's "Home" page contains both a linear gradient and an angle linear gradient. 
The linear gradient can be seen in the page header, as a horizontal top-to-bottom gradient that gradually shifts from  #D7BDE2 to #A3C6A8. 
The angled linear gradient can be seen in the page footer, as a diagonal linear gradient on a 45 degree angle that gradually shifts from #F7CAC9 to #D7BDE2


COLOUR SCHEME
I used a custom colour scheme from Adobe with the following colours: #FFF5E3 #A3C6A8 #D7BDE2 #F4A261 #F7CAC9. 
I chose this colour scheme because it is cohesive and the colours complement one another. I used Adobe's "Explore Colour Palettes" feature and searched for a colour scheme that I thought would bring my page to life.
The neutral shades allow the more striking colours to pop, and the boldness makes my page look unique and aesthetically pleasing. 

