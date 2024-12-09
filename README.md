# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

What are the main differences between Flexbox and Grid layouts? Describe scenarios where each layout system would be more suitable.

### Response 1

## Prompt 2

What is the difference between `justify-content` and `align-items` in Flexbox? How does each property control the positioning of flex items within the container?

### Response 2

## Prompt 3
Describe the difference between `grid-template-areas` and `grid-template-columns`/`grid-template-rows`. When might you prefer one approach over the other?

`grid-template-areas`:
Can be used as a way to organize your webpage layout, with clear and easy to understand labels such as ("Header", "sidebar", and "footer") You can easily move sections around just by changing names without worrying about the exact sizes of rows and columns. Organizes your page into sections with clear labels that are easy to rearrange.

`grid-template-columns`/`grid-template-rows`:
Gives you exact control over the sizes of the grid, so everything fits just right. If you need a specific number of rows or columns this how you would be able to make more precise and add actual number of measurements.


## Prompt 4

Explain the `min-width` and `max-width` keywords in media queries. How do they help create responsive breakpoints for different screen sizes?

`Min-width` is mostly used when you are creating a website and want to make sure that it looks good while on a larger.

```
 For large desktops (min-width: 1024px) 
@media (min-width: 1024px) {
  body {
    font-size: 18px;
  }
}
```
When using `max-width` you are making sure that your website is compatible with smaller screens like phones or tablet. 

 For smaller screens, like phones  with a max width of 600 px.
``` 
@media (max-width: 600px) {
  body {
    font-size: 12px;
  }
}
```
By combining both you are able to create websites that adapts to any screen size. 


## Prompt 5

Imagine you are teaching a brief lesson on **mobile first design**. Your lesson should include the following information:

* An explanation of mobile first design and a few of the benefits of this approach 
* A CSS code example demonstrating how to use media queries to adjust the layout of a container from mobile to desktop with either Flexbox or Grid (choose one).
* An explanation of the code example.

**Mobile first design**: 
* With mobile first designs the designs start simple for small screens and adjusts for larger screens later on. 

*  **Flex Box** that I used below in my example is a tool used in css in order to make your layouts look good in an easier way

```
// default style for mobile
.container {
display: flex;
gap: 10px
}
// change layout for wider screen 768px (tablets/ desktops)
@media (min-width: 768) {
    .container {
     flex-direction: row;
    justify-content:space-between;
    }
}

```


