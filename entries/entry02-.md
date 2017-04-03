# Entry 2: Nesting and Partials in **_SASS_**

## Nesting:

Nesting is a big thing in SASS. Basically, based on my understanding, Sass takes the user's pre written css selectors and turns them into html navigation. You can use the li, ul and a selectors
to organize your css. Nesting allows you to write selectors that mimic the structure of your HTML. This allows you to use shortcuts to create your CSS. For example:

```
div {
    p {
        color: black;
    }
}
```
## How do you use Nesting?


Nesting styles is simple enough. You just enclose a selector (or selectors) inside the curly braces of another selector.


```css

.parent {
    .child {
    }
}
```

#### Partials
Partuaks snippets of code that Sass does not translate into regular css, unlike what sass normally does to css. A partial is simply a Sass file named with a leading underscore. You might name it something like _partial.scss . The underscore lets Sass know that the file is only a partial file and that it should not be generated into a CSS file.



# Takeaways

1) Try to not leave entries to tge last minute. Procrastination is never good!
When you do things in a rush you won't gain and have as much knowledge and understanding, the same way 
you would have if you  weren't rushing.

2) Make sure you put some of the code examples in blogs to actual WORK. JSBIN the life out of code!

3) Again, please do not procrastinate.