#css
 -->introduction to css(cascading style sheet)

 
 1.Styling
 - today we learnt that how to style web page
 - there are 3 ways of styling:
    1.External.
    2.Internal.
    3.Inline.
In web page if we want link something use "link" tag.

2.fonts:
- your default font can be different based on how you set it.
- if you want change the font :
  - go to google.
  - search google fonts.
  - choose your font.
  - get the font
  - get embedded code.
  - copy code from import.
  - paste it in style sheet without style tag.
  - edit font family and font weight
  - save and run.
3. colours:
 - if you want to change the colours:
    -In CSS we use the color property to set the color of the text.
       eg.
       p
       {
        color: red; /*named color*/
       }
    - In CSS we use the background-color property to set the background-color of the text.
     eg. 
     p{
        background-color: lightblue;
     }   
4. Selectors:
   - In CSS selectors are patterns used to target and select the HTML elements you want to style.
🔹 Basic Types of CSS Selectors
1.Universal Selector (*)
Selects all elements.
2.Class Selector (.classname)
Selects all elements with a specific class.
3.ID Selector (#id)
Selects a single element with a specific ID.
-id vs Classes.
 id -> less Used -> Dont Use Same id Twice on One Page.
 class -> most Used -> Classes Can be used multiple times.
5. Utility Classes:
   -Utility classes in CSS are single-purpose classes that apply one specific style or property to an element. They are designed to be reusable, composable, and non-semantic, often used to build up styles by combining multiple small classes rather than writing custom CSS for each component.
6. Types of CSS Units: 
      - There are two types of CSS unit:
    1) Absolute Units 
     -Fixed
    2) Relative Units
     -Not Fixed
7.  Flex:
    In CSS, flex refers to Flexbox, a powerful layout model that makes it easier to design flexible and responsive layout structures.
    🔹 What is Flexbox?
    Flexbox (Flexible Box Layout) is used to align and distribute space among items in a container, even when their size is unknown or dynamic.
    Flexbox is one-dimensional layout System.
    - There are 4 types of direction in Flex:
     Value               Description                          
    1.row                Default. Items are placed **horizontally** from left to right.               
    2.row-reverse        Items are placed **horizontally**, but in **reverse** order (right to left). 
    3.column             Items are placed **vertically** from top to bottom.                          
    4.column-reverse     Items are placed **vertically**, but in **reverse** order (bottom to top).   
    

row → ➡️ A B C

row-reverse → ⬅️ C B A

column → ⬇️
A
B
C

column-reverse → ⬆️
C
B
A

display: flex;
   justify-content: flex-start;
   justify-content: flex-end;
   justify-content: center;
   justify-content: space-between;
   justify-content: space-around;
   justify-content: space-evenly;


8. 🔹 CSS Box Model 
Every HTML element is considered a box, and the CSS box model defines how the size of that box is determined. It consists of the following parts (from inside out):

 1.Content.

 2.Padding.

 3.Border.

 4.Margin.

9. 🔹 Inheritance:
Inheritance in CSS refers to the way some CSS property values are automatically passed down from a parent element to its child elements in the document tree.

properties that inherits by default:

1.color.
2.font-style.
3.font-family.
4.font-size.
5.font-weight.
6.font-variant.
7.letter-spacing.
8.white-space
9.text-align.
10.visibility.


10. 🔹 position :
The position property in CSS defines how an element is positioned in the document flow. It affects where the element appears on the page and how it interacts with other elements.

     🔹 Position Values in CSS
   Value      	    Description
   static	      The element follows the normal document flow. No offset applied.
   relative	      Positioned relative to its normal position. You can use top, left, etc.
   absolute       Positioned relative to the nearest positioned ancestor (non-static).
   fixed	         Positioned relative to the viewport (stays in place when scrolling).
   sticky	      Hybrid of relative and fixed. It scrolls with the page until it reaches a certain position, then sticks.



11. 🔹 Viewport:
The viewport is the "visible area of a web page" within the browser window. It represents the portion of the page the user can see without scrolling.

🔹 Why the Viewport Matters in CSS
  1.It determines how content is sized and positioned relative to the user’s screen.
  2.Responsive design often depends on viewport size.
  3.CSS units like vw, vh, and media queries rely on the viewport dimensions.

Concept/Unit	   Description                                      	Example
1.vw	           1% of the viewport's width         	               width: 50vw; means 50% of viewport width
2.vh	           1% of the viewport's height	                        height: 100vh; means full viewport height
3.vmin	        1% of the smaller dimension (width or height)       Useful for responsive squares
4.vmax	        1% of the larger dimension (width or height)	               --


12. 🔹 em and rem:
Both em and rem are relative length units used mostly for font sizes, spacing, and layout dimensions.

1.em
Relative to the font-size of the element's parent (or the element itself if used in font-size).
Can compound if nested, meaning multiple em values multiply through the DOM tree.

2.rem
Stands for “root em”.
1.Always relative to the root element's (<html>) font size.
2.Consistent.


13. 🔹Transitions: 
    Transition: A smooth transition from one property value to another.
    transition-property: Specifies which property to transition.
    transition-duration: Defines how long the transition takes.
    transition-timing-function: Defines the speed curve of the transition.
    transition-delay: Adds a delay before the transition starts.



14. 🔹Animations:
    Animation: More complex, keyframe-based animations.
    @keyframes: Defines the animation's keyframes (specific states at certain points).
    animation-name: Specifies the name of the animation.
    animation-duration: Defines how long the animation runs.
    animation-timing-function: Controls the timing of the animation.
    animation-delay: Delays the start of the animation.
    animation-iteration-count: Defines how many times the animation runs.

 15. 🔹 Pseudo-classes:
 Pseudo classes in CSS are essential for targeting elements based on their state, structure, position, or other dynamic characteristics. They enable you to apply styles without altering the HTML structure, offering greater flexibility in your web design.   

16.  1.Structural Pseudo-classes:
       These pseudo-classes target elements based on their position or relationship in the DOM tree.
      1) :first-child
       Theory: Matches the first child element of a parent element.
       Example: This is useful when styling only the first element in a parent container.

e.g
       p:first-child {
       color: blue;
       }

      

      2) :last-child
              Theory: Matches the last child element of a parent element.
              Example: To target the last element in a list for specific styling.

e.g 
        p:last-child {
        color: red;
        }


       3) :nth-child(n)
          Theory: Matches elements based on their position in a group of siblings. n can be a number, keyword (odd, even), or formula.
          Example: Targeting every second item in a list.

e.g
         li:nth-child(2n) {
         background-color: #f0f0f0;
         }

17. Margin: 
      In CSS, margin refers to the space outside the border of an element. 
      It is a part of the box model in CSS, which defines how elements are structured on the web page. 
      Margins create space between an element and its surrounding elements (such as text, other elements, or the edge of the container).
      The margin is used to separate elements and provide spacing to make the layout visually appealing and organized.
      
      
      Key Points about Margin:
      External Spacing: Margins create space outside an element's border. This is different from padding, which creates space inside the element, between its content and border.
      Invisible Area: Margins are transparent and do not have any color or background.
      Collapsing Margins: When two vertical margins meet (e.g., between two block elements), they may collapse into one. This is called margin collapsing.
      Independent Margins: Margins for each side of an element (top, right, bottom, left) can be set independently, allowing for fine control over spacing.


      margin-top: Defines the margin space on the top of the element.
      margin-right: Defines the margin space on the right of the element.
      margin-bottom: Defines the margin space on the bottom of the element.
      margin-left: Defines the margin space on the left of the element.


 18. margin collapsing:
         Margin Collapsing in CSS?
           Margin collapsing refers to a behavior in CSS where vertical margins of adjacent block-level elements collapse into a single margin. 
           The larger margin of the two is retained, and the smaller margin is ignored. This happens when elements are in the same block formatting context and are next to each other, either vertically or at the top or bottom of a parent element.
           This can lead to what might seem like unexpected behavior when elements with margins are stacked together.
               
           
      How Margin Collapsing Works:
       When two adjacent vertical margins meet, the following rules apply:
       Two adjacent block-level elements will have their vertical margins collapse into one margin.
       The larger of the two margins is kept, and the smaller one is discarded. If both margins are equal,the total margin between the two elements is just the value of that single margin.
       Collapsing doesn't happen with horizontal margins, only vertical margins (top and bottom).

  19. Padding :
      Padding in CSS is the space inside an element, between the content of the element and its border. 
       It is part of the CSS box model and allows you to control the space within the element, essentially creating a buffer between the element's content and the edge of the element's border.
       Padding is used to create breathing room around the content inside an element,ensuring that the content doesn't touch the border directly,making the design cleaner and more visually appealing.

      Key Points About Padding:
        1.Inside the Element: Padding is the space inside an element’s border. It does not affect the layout of other elements but affects how content is displayed within the element.
        2.Transparent: Like margins, padding is transparent and does not have any color or background. It simply creates spacing.
        3.Applies to All Elements: Padding can be applied to any block-level or inline element, although it's more commonly used with block-level elements like form elements.
        4.Separate from Margins: Padding affects the internal space of an element, while margin controls the external space.

