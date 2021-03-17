### Read: Class 02 (_class 01 will magically appear here at some point and this disclaimer will go away_)
Handling events via DOM manipulation and even with JQuery is extremely cumbersome. It's _functional_, sure, but if nothing else, the code it produces can take significant effort to unwind and analyze if you're not already well-versed in what it does. Consider a basic example from [Learn JQuery](https://learn.jquery.com/events/inside-event-handling-function/): 

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

There's nothing particularly mysterious going on here, but that's a lot of action just to stop a link from firing. We find similar functionality at [ReactJS](https://reactjs.org/docs/handling-events.html):
```
function ActionLink() {
  function handleClick(e) {
    e.preventDefault();
    console.log('The link was clicked.');
  }
  ```
  
  The event handler isn't exactly the same, but it's much more readable. Considering how dynamic virtually everything on the internet is these days, it's important that building things that take advantage of that dymanism be easy to implement, and maybe more importantly, relatively simple to figure out after the fact. 
