# The Pitfalls of Writing Overly Specific CSS

As a third year CMD student with a background of IT Software Engineering and over five years of experience in web development, I wanted to provide my point of view in regards of the way CSS is taught at (my) school. For beginner developers, or students in this case, it is crucial to adopt best practices when it comes to coding to improve collaboration, maintainability and efficiency. With these best practices comes needing to have a solid understanding of how CSS works and it's many diverse selectors.

Throughout my CMD career I have noticed there is a high emphasis on writing highly specific CSS, without utilizing any classes or IDs. While I understand the reasoning behind this (creating a solid foundation for beginner developers), I also think there might be too much emphasis on this way of developing. I notice fellow students actively avoiding the use of classes or IDs, or when they do use classes they tend to either create classes for a single specific item or not giving them the correct name. And honestly, I can't blame them! I used to be like that as well; I used classes on every single item, not understanding the power of classes and why we use them. The issue I have is that our courses make it seem like using classes is a bad thing. I think we need to advocate and help students understand how to create more modular, dynamic and efficient coding practices.

## The Downsides of Specificity

One of the primary drawbacks of writing overly specific CSS is the lack of modularity it introduces. As mentioned before, I totally understand why beginners should learn how to write without use of classes. But this results in them not wanting to use classes at all throughout the rest of their career (at least during their school career) When each style rule targets a specific element or group of elements, it becomes challenging to reuse styles across different parts of a website or application. This redundancy can result in bloated stylesheets, increased development time, and decreased maintainability. I have had to work in several group projects for a web development project, and each time I am met with the dread of having to maintain the CSS. All because my teammates (not their fault by the way! This is not me pointing a finger at them, I am pointing the finger at our courses) do not understand the downsides of specificity and the power of writing modular code. 

Using too much specificty makes it incredibly hard to make even minor changes to the layout or structure of a site or application, which then results to a higher likelihood of creating errors or inconsistencies. There are several ways I have noticed students write their overly specific CSS selectors.

```css
/* Example 1: Overly specific selectors */
div.container ul#nav li.active a {
    color: red;
}

/* Example 2 */
div > ul > li > a {
    color: red
}

/* Example 3 */
header > div:first-of-type ul > li:nth-of-type(4) {
    background-color: blue;
}

```

```html
<!-- Example 4: Inline styles -->
<div style="color: blue;">Hello, World!</div>
```

```css
/* Example 1: Utilizing classes */
.container {
  /* Styles for container */
}

.nav {
  /* Styles for navigation */
}

.active {
  /* Styles for active elements */
}

/* Example 2: External CSS file */
/* styles.css */
.text-blue {
  color: blue;
}
```

### Collaboration Challenges

In collaborative environments, where multiple developers work on the same codebase (for example: school projects!), the specificity of CSS can significantly hinder teamwork and productivity. With specific CSS, the chances of naming conflicts increase, as each developer may create their own uniquely tailored selectors. Resolving conflicts and merging code becomes a time-consuming task that detracts from the overall efficiency of the team. In contrast, using classes and IDs allows for clear communication and collaboration, as they provide standardized hooks for styling and make it easier to understand and navigate the codebase.

### Maintainability and Scalability

As projects grow in size and complexity, maintaining and scaling the CSS becomes a critical concern. Writing specific CSS makes it challenging to make changes or add new features without affecting other parts of the codebase. In contrast, modular CSS promotes reusability, flexibility, and scalability. By separating styles into reusable classes, developers can easily update or extend the appearance and behavior of elements without risking unintended side effects. This modularity also facilitates the maintenance of consistent design patterns and user experiences across the entire project.

### Efficiency and Performance

Specific CSS can adversely impact performance by increasing the size of the stylesheet. The more specific the selectors, the longer it takes for the browser to parse and apply the styles! This can result in slower load times and a suboptimal user experience, particularly on mobile devices or in low-bandwidth situations. On the other hand, writing efficient CSS, utilizing class and ID selectors judiciously, allows the browser to render the styles quickly and efficiently, enhancing the overall performance of the website or application.

## BEM naming convention

The way I learned CSS several years ago was by a former collegue of mine. At work they stuck to the BEM (Block-Element-Modifier) naming convention. As I developed more, and attended CMD, I adopted a mix of BEM and using more specific CSS selectors where needed and relevant. I am not saying BEM is the best naming convention, this is just me sharing what works best for me and how I write more modular and scalable CSS in combination with what I have learned during my years at CMD.

BEM is a naming convention that provides a structured methodology for naming CSS classes. It consists of three components: blocks, elements, and modifiers. Blocks represent standalone components on a page, such as a header, sidebar, or button. Elements are the parts that make up a block, and modifiers define variations or states of a block or element. By organizing CSS classes in this hierarchical manner, BEM promotes modularity, reusability, and maintainability. With a shared understanding of the class naming structure, developers can work seamlessly on the same codebase, reducing conflicts and facilitating teamwork. When revisiting the codebase or collaborating with other developers, it becomes easier to understand the purpose and context of each class, reducing confusion and minimizing the learning curve

While BEM encourages the use of descriptive class names, it's essential to avoid falling into the trap of excessive class usage. Adding too many classes to elements can make the CSS codebase convoluted and difficult to manage. It may also lead to an overcomplication of styles and hinder code readability. Developers should remember that BEM is a tool, not a rule! It should be used accordingly, focusing on clarity and maintainability rather than rigid adherence.

To strike the right balance with BEM, you should try to prioritize modularity and minimalism. Each class name should have a clear purpose and should be used where necessary. When applying BEM, I try to consider the following guidelines:

1. **Identify reusable blocks:** Analyze your project's components and identify those that can be encapsulated into standalone blocks. Blocks should be self-contained and modular, allowing for easy reusability across different parts of the application
2. **Use elements within blocks:** Elements represent the smaller parts that make up a block. Use them sparingly and only when they provide value. Elements should be tightly coupled with their parent blocks and shouldn't be used outside their context.
3. **Leverage modifiers for variations:** Modifiers define variations or states of blocks or elements. They are particularly useful when you need to style specific instances differently. However, it's crucial to avoid creating unnecessary modifiers and instead focus on essential variations that truly affect the appearance or behavior of the component.

Here are some code examples that demonstrate the usage of the BEM naming convention and how I use it:

```html
<main>
    <!-- depending on context I would add a class to header element if necessary -->
    <header>
        <h1>Welcome</h1>
        <p>Lorem ipsum dolor sit amet...</p>

        <!-- reusable component(s) -->
        <div class="btn-container">
            <a class="btn" href="#" target="_blank">Login</a>
            <button class="btn btn--secondary">Read More</button>
        </div>
    </header>

    <!-- ... more HTML stuff -->
</main>
```

```css

header {
  /* header styles */
}

    /* Element */
    header h1 {
        /* styles for h1 elements within headers */
    }

    header p {
        /* styles for p elements within headers */
    }


.btn-container {
    /* block styles */
}

    .btn {
    /* Styles for the button element */
    }

    .btn--secondary {
    /* Additional styles for the button element when it has the "secondary" modifier */
    }

```

## Resources

- My own brain and experience
- [BEM Naming Convention](https://getbem.com/naming/)