# Entry 4: Inheritance and Operators in **_SASS_**

## Operators

Even though I mentioned inheritance first in my title, I want to start off by talking about Operators since I feel like it is easier to explain.
Basically, SASS can do MATH. Woah, I feel like that sounded like a rap, map, lap, cap. Let me stop,
anyways, back to operators. In Sass, Arithmetic operators are used to perform the standard arithmetic operations. 
The operators that Sass supports are + , - , % , * ,  and /. 

An example of how the + operator works: 
```Sass
h2 {
    
    font-size: 5px + 2; // 7px
}
```

They're used to do their obvious function .. Math.
However, an important catch I feel like is worth mentioning is the fact that 
operators only work for numbers with compatible units.
So, if we would've done the same operation we did above but tried to differentiate the units; we would get
something like this:

```Sass
    font-size: 5px + 2em; // error incompatible units

```
    
    
 Basicaly, that's how all the operatots work, generally. The + add, - subtracts, all that good old basic math we are used to, however, this time it's cooler than just adding, multiplying, dividing, or subtracting apples, now we're CODERS!
 
 ## Inhertance 
 Now, what is inheritance? The only way you use inheritance is by the @extend feature, that, in fact, is, what inheritance is. The @extend feautre. Okay, what exactly is the _@extend_ feature?
 
 
 @extend is a feature of Sass that allows classes to share a set of properties with one another. Selectors that @extend a class in Sass will have their selector included right up next to the class it is extending, resulting in a comma separated list.

Its syntax looks like that:
```Sass
@extend .class-name;

```

Examples of Usage: <br>
```Sass
.foo {
  color: black;
  border: 1px solid black;
}

.bar {
  @extend .foo;
  background-color: red;
}
```
```Sass
This is compiled to:

.foo, .bar {
  color: black;
  border: 1px solid black;
}

.bar {
  background-color: red;
}
```
In the example above,.foo and .barare defined which have the following features:

.bar inherits from .foo, containing all properties of parent class .foo.
.bar extends .foo by adding the property background-color.


By the way, this is the last entry in which I will be going over basic principles of Sass. In fact,
I am actually done with those. I have already started planning my BIG FINAL PROJECT. I know you want to know what it is,
I'll tell you, it isn't a secret. As you might've guessed, I'm making a website in which I will use HTML to code and incorporate SASS in it to test my understanding of it. I am so looking forward for that website. I will keep ya'll updated .. TILL NEXT ENTRY.





## Takeaways:
1- Start planning your big project, I promise, it'll be a big relief and it'll actually feel good to start working on something that big.
It'll make you feel the worth of all the research you've been doing. Really, that is the hight=light of this entry ( starting the website) and therefore, I have no
 other actual takeaways but this. **Start your project, dudeeeee!**



