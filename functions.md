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

# The "standard library"
You might be wondering what other functions are available in JavaScript. The answer: A TON. There are lots built in, standard libraries that you can learn about at MDN (A site run
by Mozilla that has lotsa nifty information about web technologies). For example here is the MDN page on JavaScript's Math object.

# Making new functions
You aren't limited to using other peoples functions — you can also write them yourself. It's pretty easy! Let's make a function called makeMoreExciting that adds a bunch of exclamation points to the end of a string.

```
function makeMoreExciting(string) {
  return string + '!!!!'
}
```
In my head I read it out loud like this: "there's a function called 'make more exciting' that takes in a string and returns a new copy of that string that has a bunch of exclamation points at the end".

Why is sentence empty? Because functions return undefined by default! You can choose to return a value by returning something. Functions should take in a value and, if they change the value or create a new value that is supposed to be used later, return a value (fun fact: a fancy term for this style is functional programming). Here is another function that doesn't return anything but instead uses a different method to show us the output:

```
function yellIt(string) {
  string = string.toUpperCase()
  string = makeMoreExciting(string)
  console.log(string)
}
```

So is there something wrong with the above yellIt function? It depends! Here are the two major types of functions:

functions that modify or create values and return them
functions take in values and perform some action that cannot be returned
console.log is an example of the second type of function: it prints things out to your console — an action that you can see with your eyes but that cannot be represented as a JavaScript value. My own rule of thumb is to try to keep the two types of functions separate from each other, so here's how I would rewrite the yellIt function:

function yellIt(string) {
  string = string.toUpperCase()
  return makeMoreExciting(string)
}

console.log(yellIt("i fear no human"))
This way yellIt becomes more generic, meaning it only does one or two simple little things and doesn't know anything about printing itself to a console — that part can always be programmed later, outside the function definition.
