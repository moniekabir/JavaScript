Functions
Now that we have our sentence stored in a variable, let's change a word stored in it! We can do this by performing a function. Functions are a type of value that, well, serve a 
specific function (AKA purpose or action) for us. Calling them "actions" sounded weird I guess so they went with the word "function" instead.

JavaScript has a function called `replace` that does exactly what we want! Functions take in any number of values in their parentheses (zero, one or many) and return either 
nothing (undefined) or the changed string. The replace function is available to use on any strings and takes in two values: the characters to take out and the characters 
to swap in. It gets confusing to describe these things so here is a visual example:

```
"Hello World".replace('World', 'JavaScript');
```

Notice how the value of dogSentence is the same even after we run replace on it? This is because the replace function, (and most JavaScript functions for that matter) takes the 
value we give it and returns a new value, without modifying the value we passed in. Since we didn't store the result (there is no = on the left side of the replace function) it 
just printed out the return value in our console.
