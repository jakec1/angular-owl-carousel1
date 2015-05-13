# angular-owl-carousel1

Angular directive wrapping owl carousel v1

*For use with Owl Carousel 1*

## Usage

Javascript:
```javascript

	// Define app module
	angular
		.module('myApp', ['angular-owl-carousel']);

	// Create controller
	angular
		.module('myApp')
		.controller('MyController', MyController);

	function MyController() {
		this.items = ['item1', 'item2'];
	}
```

HTML:
```html
	<div ng-controller="MyController">
		<div
			items="1"
			navigation="true"
			owl-carousel="items">
			<div class="item">{{ item }}</div>
		</div>
	</div>
```

Feel free to use owl carousel params described on [official site](http://owlgraphic.com/owlcarousel/#customizing). Just add them as on the code example above.

*Note:* I created this directive for owl carousel v1 because v2 is in beta now and has some problems with destroying that I could not fight.
