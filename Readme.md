# Reading Notes

## Code 301 - Intermediate Software Development
I've taken 301 before, but I'm super excited to learn some React and remember how JavaScript works (_and doesn't_).

Some things I'm hoping to get out of 301:
- Some solid React knowledge
- Improved JS skills in general
- ~~sleep :zzz:~~

***This is the end of my description.***
Wow, that was aggressive. Remind me **not** to do that again.

### Read: Class 02 (_class 01 will magically appear here at some point and this disclaimer will go away_)
Handling events via DOM manipulation and even with JQuery is extremely cumbersome. It's _functional_, sure, but if nothing else, the code it produces can take significant effort to unwind and analyze if you're not already well-versed in what it does. Consider a basic example from [Learn JQuery(https://learn.jquery.com/events/inside-event-handling-function/)]: 

```
// Preventing a link from being followed
$( "a" ).click(function( event ) {
    var elem = $( this );
    if ( elem.attr( "href" ).match( "evil" ) ) {
        event.preventDefault();
        elem.addClass( "evil" );
    }
});
```

There's nothing particularly mysterious going on here, but that's a lot of action just to stop a link from firing. We find similar functionality at (reactjs.org):
```
function ActionLink() {
  function handleClick(e) {
    e.preventDefault();
    console.log('The link was clicked.');
  }
  ```
  
  The event handler isn't exactly the same, but it's much more readable. Considering how dynamic virtually everything on the internet is these days, it's important that building things that take advantage of that dymanism be easy to implement, and maybe more importantly, relatively simple to figure out after the fact. 
