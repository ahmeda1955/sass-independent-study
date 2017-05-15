# Entry 6: Actual work with **_SASS_**

I think this has by far been the most challenging week in my SASS journey. I am trying to get to work 
and start working on my website! However, I am having some issues set it up.
I was too worried trying to gain lots of knowledge about SASS functions that I don't remember investing time into 
actually looking at how to set it up in the website/app you're doing other than 
running "gem install SASS".

However, after doing some digging and searching around I found out what I should do 
and how SASS actually works with CSS. So, you don't just write "sass" and that's how 
your website gets customized. You have to Make Sass watch your SCSS files and make it "compile" the CSS

You do that by typing in 
```sass
sass --watch scss:css
```

## What is the “--watch” command ?

Actually, the “--watch” command is not a “command”. It’s called a flag.
The “--watch” flag tells Sass to “pay attention” to the folders /scss and /css, so when you make changes to
the .scss file (demo-styles.scss) Sass will detect the change and compile the SCSS file into the final CSS file you’re going
to use on your website or app.
All tutorials I’ve read make you watch specific files, like this:

```sass
sass --watch styles.scss:styles.css
```
…which is Ok. I just think that watching folders is easier 
and makes more sense because you’re watching ALL FILES in both directories rather than specific ones, 
and saves you having to type too much in the CMD as well.


### What I learned this week is actually, arguabely one of the most important  things I've 
encountered throughout my independent-study journey. Now, I know how SASS LITERALLY works.
So, you write in SASS, then SASS, _magically_ converts the SASS into regular CSS for your website or app
 to understand.
 
 
 ## Takeaways:
 
 1) Google is your bestfriend. Use google whenever you're stuck. The answer
 will always be there, I promise; progress takes patience and perseverance. 
 
 2) Read other coders blogs.



