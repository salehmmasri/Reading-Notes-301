# SMACSS and Responsive Web Design
*Reading Shay Howe’s intro to RWD All About Floats*

*Bookmark/Skim Don’t Overthink It Grids CSS Floats Explained By Riding An Escalator - If you took Code 201, review this article. If you did not take Code 201, this is Essential reading.*

**SMACSS Official Documentation**

## Responsive Web Design
*Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.*

- Ethan Marcotte book

- Responsive vs. Adaptive vs. Mobile

- Responsive generally means to react quickly and positively to any change.
    - websites continually and fluidly change based on different factors, such as :
        - viewport.
        - width.
- adaptive means to be easily modified for a new purpose or situation.
    - built to a group of preset factors.
    - Mobile means to build a separate   website commonly on a new domain solely for mobile users.
*Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. This solution has the benefits of being all three, responsive, adaptive, and mobile.*
## Responsive web design is broken down into three main components:
- Flexible Layouts

    - the practice of building the layout of a website with a flexible grid
    - capable of dynamically resizing to any width.
        - Flexible grids are built using relative length units(percentages % or em). These relative lengths are then used to declare common grid property values such as width, margin, or padding.
- media queries

- an extension to media types commonly found when targeting and including styles.
    - @media all and (min-width: 800px) and (max-width: 1024px) {...}
- mobile first
- Viewport

- flexible media

- Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.
- using the max-width property.
- Flexible Embedded Media

    - the embedded element needs to be absolutely positioned within a parent element.
    - The parent element needs to have a width of 100% so that it may scale based on the width of the viewport.
    - the parent element also needs to have a height of 0 to trigger the hasLayout mechanism within Internet Explorer.    