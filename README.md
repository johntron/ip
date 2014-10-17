ip
==

Tools for working with IP addresses (v4 and v6).


Usage
==
```javascript
var IP = require('ip'),
	min = new IP('192.168.0.0'),
	max = new IP('192.168.255.255'), // Inclusive
	entered = '192.168.0.0';

entered = new IP(entered);

if (entered.less(min) || entered.equal(min)) {
	console.log('Entered IP must be greater than 192.168.0.0');
} else if (entered.greater(max)) {
	console.log('Entered IP must be less than 192.168.255.255 (inclusive)');
}
```
