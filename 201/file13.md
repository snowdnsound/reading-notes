# Local Storage

The main problem with HTTP as the main transport layer of the Web is that it is stateless. This means that when you use an application and then close it, its state will be reset the next time you open it. If you close an application on your desktop and re-open it, its most recent state is restored.

The classic way to do this is by using a cookie. A cookie is a text file hosted on the user’s computer and connected to the domain that your website runs on. You can store information in them, read them out and delete them. Cookies have a few limitations though:

* They add to the load of every document accessed on the domain.
* They allow up to only 4 KB of data storage.
* Because cookies have been used to spy on people’s surfing behavior, security-conscious people and companies turn them off or request to be asked every time whether a cookie should be set.

To work around the issue of local storage, the WHATWG and W3C came up with a few local storage specs, which were originally a part of HTML5 but then put aside because HTML5 was already big enough. 

Using local storage in modern browsers is ridiculously easy. All you have to do is modify the localStorage object in JavaScript. You can do that directly or (and this is probably cleaner) use the setItem() and getItem() method:

localStorage.setItem('favoriteflavor','vanilla');  

If you read out the favoriteflavor key, you will get back “vanilla”:

var taste = localStorage.getItem('favoriteflavor');
// -> "vanilla"  

To remove the item, you can use — can you guess? — the removeItem() method:

localStorage.removeItem('favoriteflavor');
var taste = localStorage.getItem('favoriteflavor');
// -> null  

That’s it! You can also use sessionStorage instead of localStorage if you want the data to be maintained only until the browser window closes. One annoying shortcoming of local storage is that you can only store strings in the different keys. This means that when you have an object, it will not be stored the right way. You can work around this by using the native JSON.stringify() and JSON.parse() methods:

var car = {};
car.wheels = 4;
car.doors = 2;
car.sound = 'vroom';
car.name = 'Lightning McQueen';
console.log( car );
localStorage.setItem( 'car', JSON.stringify(car) );
console.log( JSON.parse( localStorage.getItem( 'car' ) ) );

## Things I Want to Learn More About

* Web Applications
* Stateless vs other states?
* At rest
* Evercookie


## Handy Links

* [Local Storage and How to Use it on Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)
* [The Past, Present & Future of Local Storage for Web Applicaions](http://diveinto.html5doctor.com/storage.html)
* [Local storage specs](https://html.spec.whatwg.org/multipage/webstorage.html)
* [Evercookie](https://samy.pl/evercookie/)
* [Autosave User Input into Forms](https://www.smashingmagazine.com/2011/12/sisyphus-js-client-side-drafts-and-more/)

## Questions From the Reading

### Local Storage and How To Use It On Websites

Why would a developer use local storage for a web application?

* This is helpful when needing to store infomration locally such as the state of an application for a later time as HTML is stateless. 

What information should not be stored in local storage?

* Personally Identifiable Information (PPI), authentication tokens, user location data or API keys. 

Local storage can store what type of data? How would you convert it to that type before storing?

* It stores strings, you would use the JSON.stringify() and JSON.parse() methods to convert it. 