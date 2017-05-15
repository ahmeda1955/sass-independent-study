# Entry 7: Actual work with **_SASS_** Part Two

This entry is really special to me. I have successfully incorporated SASS in my code and got it 
to work. All it took was for me to approach the idea from a different perspective, I was just 
making life harder for myself!

## How I installed **_SASS_** in my project: 

After running 

```Sass
gem install sass
```

I would quickly try to rush things and type,

``` Sass
sass --watch input.scss:output.css
```
Not knowing what that meant, or what it did. Then I would tinker a lot trying to copy 
and paste commands hoping they'd work. However, I found out what I was slacking/missing out 

After taking a closer look at, 

```Sass
sass --watch input.scss:output.css
```

I realized that two files are part of that command, "input.scss" and "output.css". So, 
I went ahead and created those using the touch command. Then I ran the new command I found out about, 
```Sass
sass input.scss output.css
```

Upon doing that, I realized that a file with the name " output.css.map" was created, and it contained the following code.
<img src="../images/Screenshot (10)"/>


I thought to myself, "That's a good sign, it looks legit".


Then, I realized that this is finally how SASS could easily work:

After making two files, one input, and output; All you have to do is type your 
Sassy code in the input file, then SASS does all the work and transfers the worked up
code to the "Output" as a regular css file your HTML could understand.

Of course, you link your code to your Sass using 
```Html
<link rel="stylesheet" href="output.css">
```
Last thing: <br>
You could use the 

```Sass
sass --watch input.scss:output.css
```
After you get your input and output files set up. 
What that does is tell Sass  to watch the file and update the CSS every time the Sass file changes.
Yes, that would happen regardless, when you type into input save, and refresh. However, that command saves you from all the hassle and
makes life easier by allowing you to see real-time changes to your output.css file as you type 
into your index.scss file. It's actually pretty cool to see too!

That's a screenshot of my output.css file to give you an idea of how thingws are.

<img src="../images/Screenshot (11)"/>

Sass did all that for me. I never typed anything into output.css. I type intpo 
the input file and after running the --watch command I saw all my work get converted and transferred 
to the output file.

## Takeaways
1) Sometimes, you might be trying "Too hard" to figure something out. Too hard that you'd probably 
fail to realize that you could probably get the results you'd 
been looking for by trying another way, all you have to do is relax and think
and not try to push things through, especially when you're working with code.
Work Smart, not Hard.



