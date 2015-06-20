# Mastering CSS: BEM and ITCSS

Some days ago, Moove-it gave us the chance to meet Harry Roberts, an experienced
Front End developer. Harry provided courses to companies such as Google, Etsy,
and the BBC. The focus was to improve our Front End skills through a two-day
workshop, but the experience gave us more than a bunch of technical skills and
knowledge.

Writing CSS is very simple. Learning the language is not a big deal. It takes
no more than 2 minutes to write 3 lines of CSS to style an element of the DOM.
But, let’s think beyond. What if the application grows bigger than what we
expected at the beginning of the project? Is our code maintainable? What things
should we consider in order to write more maintainable and scalable CSS code?

Let’s look at just two technical elements we learned throughout the workshop.

### BEM. Block, Element, Modifier

When building a typical website, the process is based on the assumption that
the design and the technical specification for a website do not change over the
course of its development. The designer and the developer will work with little
or no interaction between them. Typically, we assume that the design is ready
before working on the development.

This approach has the following iteration assumptions:

*   First, the designer prepares a series of mock-ups visualizing the design of
    the website.

*   Then, based on the mock-ups, a static page is created.
*   Last, the developer brings the site to life with the integration with the
    BackEnd and adding JS logic.


This approach works well, if the assumption that we mentioned above is true.
However, that is rarely the case, as normally the website begins to evolve and
take on a life of its own. The design of the pages gradually changes, new pages
or sections are added.

One of the most important features of using BEM, is that it ensures that
everyone participating in the development of a website is working with the same
codebase and using the same terminology. The design of the website can be
changed at any moment, as site requirements change, without getting into any
troubles or conflicts.

#### BEM Principles

Thinking about programming methodologies, one of the most common examples is
the Objetc Oriented Programming (OOP). We’re very familiar with OOP, and in some
ways, BEM is similar to OOP. BEM is a way of describing reality in code, with a
range of patterns, and a way of thinking about program entities regardless of
the programming languages being used.

#### BEM Components

*   *Block*: A block is an independent entity, a “building block” of an
    application. A block can be either simple or compound (containing other blocks
    ). For example, a block can be a Search Box.

*   *Element*: An element is a part of a block that performs a certain function
    . Elements are context-dependent: they only make sense in the context of the
    block that they belong to. In our example, elements are the input of the Search
    Box, or the Submit button.

*   *Modifier*: If we want to add a particular attribute to an element, we
    should use modifiers. For example, to add two Search Boxes, but one with a
    bigger button, we can add the modifier –big to the Submit button.
   <figure>

![][1]</figure>
In this case, we will have something like this:

|  | <block:search>

And the css, should be something like this:

|  | .b-search{

As you can see, this approach gives us the chance to modify the block, remove
it, or add new components, without unexpected changes across the application.
The code will be maintainable, easy to learn, and simply awesome.

### ITCSS. A sane, scalable, managed CSS architecture from CSS Wizardry

The title of the [official page][2] is very descriptive. The workshop made us
think a lot about our one apps and highlighted the importance of having our own
CSS architecture. We usually build large and complex applications, that change
over the time. Having a defined architecture is something we can’t avoid, and
will give us the ability to offer better code in less time.

Managing CSS at scale is hard, and sometimes we make it a lot harder than it
should be. The Inverted Triangle CSS is a simple, effective, and as-yet
unpublished methodology to help manage, maintain, and scale CSS projects of all
sizes. ITCSS, is not a library, it’s a school-of-thought, a meta framework if
you will. It helps manage the problems that writing CSS at scale has, and helps
keep sanity . It’s also based on this statement: “each piece of CSS needs a
knowledge of what came before it, and what might come after it”. CSS is giant
dependency tree, and we need a way to manage this dependency at a very low level.

ITCSS was one of the most valuable topics that we learned in the workshop, and
something that we already started to use in our web applications.

### Miscellaneous…

Last, but not least, let’s talk about Harry. We met not only a css expert,
but also a great person. We can say a lot of things about the workshop, the
ITCSS architecture, BEM and all this great technical stuff, but that’s not all.
The workshop provided the opportunity to met a person who worked with valuable
companies across the globe, and we were able to learn a lot from his experience.

We also went out to drink beer and talk about culture, sports, technologies,
etc, with a person we met the day before. It was a great experience, which gave
us a great amount of technical knowledge, and opportunity to make a new friend.

![][3]</figure>

 [1]: img/P04PTRZ.png
 [2]: http://itcss.io/ "ITCSS"
 [3]: img/Mj5Mv41.jpg
