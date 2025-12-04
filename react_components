# React Components: The Core Concept

## English Version

React and its ecosystem provide dozens of useful and important features and concepts which of course are all going to be covered in depth throughout this course. But if you were forced to identify only one core concept which you will need for all react apps,

it would be the concept of working with components because components are potentially reusable building blocks which you as a react developer can create and which you then combine to build the overall user interface.

So React apps are in the end built by combining components. And whilst a couple of additional features and concepts would be required to create truly interactive user interfaces. Components are the one concept

every React app no matter its complexity will use. And indeed the idea of thinking of user interfaces as combinations of components is not unique or exclusive to React. If you visit any website of your choice,

you'll quickly be able to identify a couple of key building blocks that make up the overall site or app. For example, in this demo website, we're going to work on throughout this section, you could identify the header area, the key concept items and the interactive tabs section as components.

you could also identify more or less components because as you will also learn in this section and this course it will come down to the developers who are working on an app to define how big or small a component should be. But the idea behind those components

really just is that they wrap HTML and possibly also CSS code as well as any related javascript logic that might be needed and together those languages and code pieces then define and control a part of the UI

This allows you the developer to split up complex user interfaces into smaller more manageable parts which at least potentially may also be reused in different places of the UI for example, this core concept component is used four

times just configured with different data, but using the same HTML markup and styling and javascript logic under the hood. And that's one of the main reasons why this components approach is so powerful and popular without components,

you would quickly end up with rather large and complex HTML files that may become difficult to navigate and work with. In addition, a change in your code might need to be applied in different parts of your application. Hence increasing the likelihood of errors.

When using this components approach, you're instead reusing code and you only need to make such a change in one place. Another big advantage of this component's idea is that related code can be stored together because without components, you would typically have your markup in the HTML file

and your javascript code in one of your javascript files. If you needed to make a change to the javascript code, you would therefore have to switch back and forth between those files all the time. And since you are likely working in different files, and it's quite possible that you're not seeing

all the related code together all the time. It's also quite likely that you might accidentally break your code because you maybe changed something in your javascript code that then would have also required a change in the HTML code. On the other hand, when working with components related code is typically kept closely together,

hence simplifying the development process. And the last major advantage of working with components is that you follow a design and development principle, which is almost always a good idea. You have a separation of concerns different components, do different things and handle different parts of the UI

for example, in the demo project of this section, we have components that are responsible for outputting information and we have other components that are responsible for switching between tabs and handling user input.

And that's of course, just a basic app, the more complex your projects become the more useful this pattern becomes as it also simplifies the process of working on the same project with multiple developers where every developer works on their own feature area, for example, and that's why this idea of working with components is

embraced by React and why as a react developer, you will create and use hundreds and thousands of such components also in this course. And just as a side note, it's not just react. This concept is so popular and useful

that you'll also find it in other popular Frontend frameworks like Angular view or Svelte. And you'll also find it outside the world of web development, for example, in mobile development frameworks like Flutter. So let's therefore now take a look at a first react component in code and then of course,

also create a first component.

## 中文版本

React及其生态系统提供了数十种有用且重要的特性和概念，这些当然都将在本课程中深入讲解。但如果你被迫只确定一个对所有React应用都必需的核心概念，

那就是使用组件的概念，因为组件是潜在的可重用构建块，作为React开发者，你可以创建这些组件，然后将它们组合起来构建整体用户界面。

所以React应用最终是通过组合组件来构建的。虽然创建真正交互式的用户界面还需要一些额外的特性和概念，但组件是唯一一个

每个React应用无论其复杂程度如何都会使用的概念。实际上，将用户界面视为组件组合的想法并不是React独有或专属的。如果你访问任何你选择的网站，

你很快就能识别出构成整个网站或应用的几个关键构建块。例如，在我们将在本节中使用的这个演示网站中，你可以将头部区域、关键概念项目和交互式标签部分识别为组件。

你也可以识别出更多或更少的组件，因为正如你将在本节和本课程中学到的，最终由开发应用的开发者来定义组件应该有多大或多小。但这些组件背后的理念

实际上就是它们封装了HTML和可能还有CSS代码以及可能需要的任何相关JavaScript逻辑，这些语言和代码片段一起定义和控制UI的一部分。

这使你作为开发者能够将复杂的用户界面分解成更小、更易于管理的部分，这些部分至少潜在地也可以在UI的不同位置重复使用。例如，这个核心概念组件被使用了四

次，只是配置了不同的数据，但在底层使用相同的HTML标记、样式和JavaScript逻辑。这就是为什么这种组件方法如此强大和流行的主要原因之一。如果没有组件，

你很快就会得到相当大且复杂的HTML文件，这可能会变得难以导航和使用。此外，代码中的一个更改可能需要在应用的不同部分应用。因此增加了出错的可能性。

当使用这种组件方法时，你反而是在重用代码，只需要在一个地方进行更改。这种组件理念的另一个重要优势是相关代码可以存储在一起，因为没有组件的话，你通常会在HTML文件中放置标记，

而在JavaScript文件中放置JavaScript代码。如果你需要对JavaScript代码进行更改，你就必须不断地在这些文件之间来回切换。而且由于你可能在不同的文件中工作，很可能你看不到

所有相关代码一起展示。这也很可能导致你不小心破坏了代码，因为你可能在JavaScript代码中更改了某些内容，而这些更改本应同时在HTML代码中进行相应修改。另一方面，当使用组件时，相关代码通常被紧密地放在一起，

因此简化了开发过程。使用组件的最后一个主要优势是你遵循了一种设计和开发原则，这几乎总是一个好主意。你实现了关注点分离，不同的组件做不同的事情，处理UI的不同部分。

例如，在本节的演示项目中，我们有负责输出信息的组件，也有负责在标签之间切换和处理用户输入的其他组件。

当然，这只是一个基本的应用，你的项目越复杂，这种模式就越有用，因为它也简化了多个开发者在同一项目上工作的过程，每个开发者都可以在自己的功能区域工作，这就是为什么这种使用组件的理念

被React所采纳，也是为什么作为React开发者，你将在本课程中创建和使用数百甚至数千个这样的组件。顺便说一下，这不仅仅是React。这个概念非常流行和有用，

你也会在其他流行的前端框架中找到它，如Angular、Vue或Svelte。你也会在Web开发世界之外找到它，例如在移动开发框架Flutter中。所以让我们现在来看一下代码中的第一个React组件，然后当然，

也创建一个第一个组件。
