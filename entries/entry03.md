# Entry 3: Import and Mixins in **_SASS_**

## Import:

#### Partials:
Importing is a big PRO and definetely a key feature of SASS. However, before we get into what exactly it importing is and how we can use them, 
I have to mention that you won't be able to use the feautre without being familiar 
with another aspect of Sass: Partials. A partial is simply a Sass file named with a leading underscore. You might name it something like _partial.scss . The underscore lets Sass know that the file is only a partial file and that it should not be generated into a CSS file. Sass partials are mainly to be used with the SASS @import directive. 
___

_Naturally_ to be able to keep your code in separate files, you need to be able to combine them all back together. With Sass, however, you can use the @import directive to include the content of one file in another.
Sass extends the CSS @import rule so that it works with .scss and .sass files. It imports the file referenced and any variables or mixins that are defined in the imported file can be used in the main file.

```sass

@import "typography.scss";

```


The statement above would find either typography.scss or typography.sass in the same directory as the file importing the typography styles.

By default Sass will include the content of the file being imported in place of the @import statement, but there are times when Sass will compile to a CSS @import rule. In other words you’ll end up with an @import in the .css file instead of the code in the referenced file. Sass will compile to an @import if:

The file’s extension is .css
The filename begins with http://
The filename is a url()
The @import has any media queries

## Mixins
Another one of the most powerful features of the CSS preprocessor Sass is the mixin. Think of it like that,

when taking the styles for a button and, instead of needing to remember what
all of the properties are, having a selector include the styles for the button instead. 
The button styles
are maintained in a single place, making them easy to update and keep consistent.

It's literally the heaven of any coder: **_Efficiency_**.

An example of how to use a mixin would look like that:
```Sass
a:link { color: white; }
a:visited { color: blue; }
a:hover { color: green; }
a:active { color: red; }
```
Writing this code over and over again can get annoying very quickly, even if it didn't get annoying, 
still, efficiency is literally what good coding is about, 
especially when you have a large site with a lot of links. 
With a mixin creating link can be done with Sass like this.
```Sass
@mixin linx ($link, $visit, $hover, $active) {
  a {
    color: $link;
    &:visited {
      color: $visit;
    }
    &:hover {
      color: $hover;   
    }
    &:active {
      color: $active;
    }
  }
}
```
## How to include a mixin
To make use of a mixin you have to include it in your Sass files. To call the link mixin from above we would add this line.

```Sass
@include linx(white, blue, green, red);
```
The @include directive allows you to use mixins within your Sass files.

## How to create a Mixin
To create a mixin you use the @mixin directive. For example:
```Sass
@mixin sample {
  font-size: 12px;
}
```
You define this directive by using @mixin followed by the name of the mixin. You can also optionally include arguments in your mixin, such as with the linx mixin from above.
I will not get into arguments this much now, I will try to cover most 
of it in my next entry because, I feel like that topic is too big to be mentioned as a minor
detail.

## Side note:
I have already started thinking about my big project. The project that will heko assess the learning
I have been doing. I will make a tutorial, similar to the one I made about setting up GitHub;
I will start the website from Scratch and start coding the HTML portion of it in week 4.



## Takeaways:
1) If you really commit to yourself to your project, regardless of how you feel about it
(even though everyone should be feeling 100% good about his project anyways) you will feel yourself getting pulled into it more and more everyday; You will want to 
do more research so that you can be an expert in your topic. So, point is: **COMMIT YOURSELF TO THE STUDY!**

2) Try to have fun with the project.













