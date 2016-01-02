# Umbrella JS

Covers your javascript needs for those rainy days. A <2kb performant jquery-like library born from the question: [You might not need jquery](http://youmightnotneedjquery.com/), then what do you need?

You probably need awesome CSS (like [Picnic CSS](http://picnicss.com/)) and a lightweight, modern and performant javascript library.



## Getting started

Just download `umbrella.min.js`, include it in your html witih `<script src="umbrella.min.js"></script>` and you're good to go. After that, start using it:

```js
u(".menu a:first-child").addClass('active');
// or (more vanilla but slightly error-prone):
u(".menu a:first-child").first().classList.add('active');
```


## [Documentation (link)](documentation.md)


## Performance


Umbrella JS selector is faster than jQuery in some situations (Firefox) and similar in others (Chrome). This is possible by leveraging native methods where possible, but if you find any way to make it faster I'll welcome it greatly.

Old tests (no CDN yet and hot-linking has been disabled): 
  
- classes: http://jsperf.com/umbrella-vs-jquery-class/2
- tags: http://jsperf.com/umbrella-vs-jquery-tag/2
- ids: http://jsperf.com/umbrella-vs-jquery-id/2
- complex: http://jsperf.com/umbrella-vs-jquery-complex/2

## Compatibility

You can have a light library that works on the mobile browsers or a heavy one that works on old Internet Explorer versions, but you cannot have both. This is aimed for modern, responsive websites. The code is tested against Firefox and Chrome frequently and against IE10 ocasionally and on major releases.

This is where there might be more compatibility issues:
- http://caniuse.com/#feat=queryselector
- http://caniuse.com/#search=classList (compatible with notes 2 & 3)


## Alternatives

- [jQuery](https://jquery.com/)

- [Zepto](http://zeptojs.com/) 


## Contributing

You are encouraged to contribute to Umbrella JS. To write a new plugin, just copy one of the existing ones (specially recommend "addclass") and modify the files.


## Author and License

Created and maintained by [Francisco Presencia](https://github.com/FranciscoP) under the MIT license.