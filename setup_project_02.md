# React Project Setup and JSX Introduction

## English Version

Now that we know what the general idea behind components is and why working with components is so popular. It's time to switch to a React project and get started with components and with writing code there. And therefore attached to this lecture, you find a code sandbox link to a react project I prepared for you,

which is the starting project for the demo project we're going to work on throughout this section. Now, if you don't want to use this browser based environment and if you instead prefer to follow along locally,

you can also use this alternative zip file which you also find attached which once you downloaded and extracted it will of course give you that same starting project. Now, just a project which you can use and run locally on your system. If you go for this local option instead of using code sandbox,

you should open this extracted folder with any code editor of your choice, for example, visual studio code. And then there in that project, you first of all have to run NPM, install in your system terminal, navigate it into that project folder.

This command will download and install any third party packages needed by this project. For example, the React libraries and the build process tools that watch and transform the React code to code that works in the browser. Because as mentioned in the first course section by default,

the code you write in React projects would not run in the browser. Now after successfully running NPM install, which is something you only need to do once you can run NPM, run DEV to start the development server. This development server will allow you to visit a preview

website where you can see your react app in action. You should keep this development server process up and running for as long as you are working on this project. Because behind the scenes, this process will watch your code and reload that preview website.

Whenever you make changes to the code, you find that preview website by visiting this address that's output after running NPM, run DEV as mentioned, it's the same starting project and therefore the same demo website as you find it in that code sandbox environment there. If you are using code sandbox, you don't need to run NPM install or NPM, run DEV

because code sandbox will do that for you. Now, in your local project, you can quit this running development server with control C whenever you're done for the day. And if you then want to start coding again, you can simply restart it by running NPM,

run DEV again again. This is all not required if you're using the code sandbox environment.

So now with that starting project up and running, you'll find a couple of files and folders in that project folder. For example, you'll find an index HTML file in that folder. But if you open that file, you'll see that it's pretty empty though. It only contains some basic markup,

but it definitely does not contain the HTML code that's responsible for displaying the content we're seeing on the screen, the image, the title and so on. And the reason for that of course is that React is rendering this content on the screen that React is responsible for bringing something onto the screen.

And we can see in that index HTML file that it does indeed load a javascript file. It includes this index Js file. Now let's ignore that strange extension dot JSX for now and instead take a look at that file

as we can see here, we find it in this SRC this source folder. And if we open it, we do indeed find some javascript code in that file, but we still don't see anything that seems to be related to that image or title we're seeing on the website instead besides other things which we will explore later.

This file imports something from the app jsx file and this file finally does contain the markup for the content we're seeing on the screen though this file actually contains code that might be a bit confusing if you take a closer look

because it seems to contain HTML code inside of a javascript function. So inside of javascript code, and it also got this strange extension dot JSX. Well, this file as well as the index JSX file has this extension because

it is a javascript file that uses nonstandard javascript syntax to be precise. It uses a javascript syntax extension called jsx, which conveniently simply stands for javascript syntax extension. And this extension allows developers to describe and create HTML elements

by writing HTML markup code inside of javascript files. And since React will be about describing and creating user interfaces and parts of user interfaces.

This is a very useful feature. But whilst it is a nice feature and therefore used in basically all React projects and also many Non React projects, it is a feature that's not supported by browsers. So the code you see in the index Js X and APP.JS X files would not work in browsers.

Instead, the code you write as a react developer is transformed behind the scenes by the development server. In this case here before it reaches the browser, it's transformed to code that does work in the browser.

But as a developer, thanks to this jsx extension, you have this more convenient way of describing the user interface. But what's really important about this app JSX file is that what we can see here is a React component.

It is such a component I mentioned in previous lectures. And as you can see in React a component is really just a javascript function. Though in order to be recognized and used as a component by React, it's a function that must follow two important rules.

The function name must start with an uppercase character and the function must return a renderable value typically the to be rendered HTML markup. So this JSX code you see here and that's really all this is how components are created in React.

You create a regular javascript function, give it a suitable name that starts with an uppercase character and return some jsx code. And with that, let's now finally create our first custom component.

## 中文版本

现在我们已经了解了组件背后的一般理念以及为什么使用组件如此流行。是时候切换到React项目，开始使用组件并在那里编写代码了。因此，在本课程中，你会找到一个代码沙盒链接，链接到我为你准备的React项目，

这是我们将在整个章节中使用的演示项目的起始项目。现在，如果你不想使用这个基于浏览器的环境，而是更喜欢在本地跟随学习，

你也可以使用这个你也能找到的替代zip文件，一旦你下载并解压它，它当然会给你相同的起始项目。这只是一个你可以在你的系统上使用和运行的项目。如果你选择这个本地选项而不是使用代码沙盒，

你应该用任何你选择的代码编辑器打开这个解压后的文件夹，例如Visual Studio Code。然后在那个项目中，你首先需要在你的系统终端中运行NPM install，导航到那个项目文件夹。

这个命令将下载并安装这个项目所需的任何第三方包。例如，React库和构建过程工具，它们监视并转换React代码为在浏览器中工作的代码。因为正如在第一个课程部分中提到的，默认情况下，

你在React项目中编写的代码不会在浏览器中运行。现在，成功运行NPM install后，这是你只需要做一次的事情，你可以运行NPM run dev来启动开发服务器。这个开发服务器将允许你访问一个预览

网站，在那里你可以看到你的React应用程序在运行。你应该保持这个开发服务器进程运行，只要你在这个项目上工作。因为在幕后，这个进程将监视你的代码并重新加载那个预览网站。

每当你对代码进行更改时，你可以通过访问运行NPM run dev后输出的这个地址找到那个预览网站，如前所述，它是相同的起始项目，因此是你在代码沙盒环境中找到的相同的演示网站。如果你使用的是代码沙盒，你不需要运行NPM install或NPM run dev，

因为代码沙盒会为你做这些。现在，在你的本地项目中，你可以在一天结束时随时使用Control C退出这个运行中的开发服务器。如果你想再次开始编码，你可以简单地通过运行NPM run dev来重新启动它，

再次运行。如果你使用的是代码沙盒环境，这一切都不是必需的。

现在，随着起始项目的运行，你会在该项目文件夹中找到一些文件和文件夹。例如，你会在该文件夹中找到一个index.html文件。但如果你打开该文件，你会看到它相当空，只包含一些基本的标记，

但它绝对不包含负责显示我们在屏幕上看到的内容的HTML代码，如图像、标题等。这当然是因为React正在屏幕上渲染这些内容，React负责将内容呈现到屏幕上。

我们可以在index.html文件中看到，它确实加载了一个JavaScript文件。它包含了这个index.js文件。现在让我们暂时忽略那个奇怪的扩展名.jsx，而是看一下那个文件，

正如我们在这里看到的，我们在这个SRC（源）文件夹中找到它。如果我们打开它，我们确实在该文件中找到了一些JavaScript代码，但我们仍然看不到任何似乎与我们在网站上看到的图像或标题相关的内容，而是其他我们稍后将探索的东西。

这个文件从app.jsx文件导入了一些东西，而这个文件最终确实包含了我们在屏幕上看到的内容的标记，尽管这个文件实际上包含的代码如果你仔细看可能会有点令人困惑，

因为它似乎在JavaScript函数内部包含HTML代码。所以在JavaScript代码内部，它还有这个奇怪的扩展名.jsx。好吧，这个文件以及index.jsx文件之所以有这个扩展名，是因为

它是一个使用非标准JavaScript语法的JavaScript文件，准确地说。它使用了一个名为JSX的JavaScript语法扩展，这个名字方便地简单代表JavaScript语法扩展。这个扩展允许开发者通过

在JavaScript文件内部编写HTML标记代码来描述和创建HTML元素。由于React将关注描述和创建用户界面及用户界面的部分，

这是一个非常有用的功能。但虽然它是一个很好的功能，因此在基本上所有React项目和许多非React项目中使用，但它是一个浏览器不支持的功能。所以你在index.jsx和app.jsx文件中看到的代码在浏览器中不会工作。

相反，你作为React开发者编写的代码在幕后由开发服务器转换。在这种情况下，在它到达浏览器之前，它被转换为在浏览器中工作的代码。

但作为开发者，多亏了这个jsx扩展，你有这种更方便的方式来描述用户界面。但关于这个app.jsx文件真正重要的是，我们在这里看到的是一个React组件。

它就是我在之前讲座中提到的那种组件。正如你在React中看到的，组件实际上只是一个JavaScript函数。不过，为了被React识别和使用为组件，这个函数必须遵循两个重要规则。

函数名必须以大写字符开头，并且函数必须返回一个可渲染的值，通常是要渲染的HTML标记。所以你在这里看到的这个JSX代码，这就是React中创建组件的全部内容。

你创建一个常规的JavaScript函数，给它一个以大写字符开头的合适名称，并返回一些JSX代码。有了这些，现在让我们最终创建我们的第一个自定义组件。
