So why would you ever use arrays if you can just put your data in objects? Because objects don't remember the order of the keys that you set. You might enter in an object 
like this:

```
{ date: "10/20/2012", diary: "slept a bit today", name: "Charles" }
But the computer could give it back to you like this:

{ diary: "slept a bit today", name: "Charles", date: "10/20/2012" }
Or like this!

{ name: "Charles", diary: "slept a bit today", date: "10/20/2012" }

```

So you can't ever trust the order of keys in objects. If you wanna get REALLY fancy you can make an array filled with objects, or an object filled with arrays!

var moodLog = [
  {
    date: "10/20/2012",
    mood: "catnipped"
  }, 
  {
    date: "10/21/2012",
    mood: "nonplussed"
  },
  {
    date: "10/22/2012",
    mood: "purring"
  }
]

// ordered from least to most favorite
var favorites = {
  treats: ["bird sighting", "belly rub", "catnip"],
  napSpots: ["couch", "planter box", "human face"]
}
When you combine different things like this you are making data structures, just like legos!
