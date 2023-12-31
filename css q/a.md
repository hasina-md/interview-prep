1. ### Positioning Elements:

- Can you describe the difference between position: relative, absolute, fixed, and sticky in CSS?
---
1. **P**osition:static :-
- Elements with position: static; are positioned according to the normal flow of the document.
-  The top, right, bottom, and left properties have no effect.
 
 2. **P**osition:relative :-

- Elements with position: relative; are positioned relative to their normal position in the document flow.
-  Using top, right, bottom, or left will move the element from its normal position.

3. **P**osition:absolute :-
-  Elements with position: absolute; are removed from the normal flow of the document and positioned relative to the nearest positioned ancestor.

4. **P**osition: fixed :-
   - Elements with position: fixed; are removed from the normal flow and positioned relative to the browser window.

  - They stay fixed at their specified position even when the user scrolls the page.

5. **p**osition: sticky; :-

- Elements with position: sticky; are positioned based on the user's scroll position.

- They behave like relative positioning until the element crosses a specified point during scrolling, at which point it becomes fixed.

# CSS Layout Techniques
###  How does flexbox work? Provide an example scenario where you would use it.

```
The main idea behind Flexbox is to give the container the ability to alter its items' width/height (and order) to best fill available space, hence optimizing user interface (UI) adaptability to varying screen sizes.

        *(or)*

 Its main features include the ability to create responsive and dynamic layouts, handle content overflow, and control alignment and ordering of elements.

```

- Flexbox works in a one-dimensional layout, either in a row or a column.

```
  <!DOCTYPE>
  <html>
  <head>
  <title>Example Scenario</title>
  <style>
   .container {
    dispaly: flex;
   }
   .color {
    background: orangered;
    flex-grow: 1;
   }
   .one {
    background: yellowgreen;
   }
   .two {
    background: blue;
   }
   .container > div {
    padding: .5em;
    font-size: 5vw;
    color: white;
   }
  </style>
  </head>
  </html>
  <div class="container">
  <div class="color">Box1</div>
  <div class="one">Box2</div>
  <div class="two">Box3</div>
  </div>
```