# ntc.php

PHP port of `ntc js` (Name that Color JavaScript, created by Chirag Mehta)
http://chir.ag/projects/ntc/

The original script (`ntc.js`) is released under the: Creative Commons License:
Attribution 2.5 http://creativecommons.org/licenses/by/2.5/

For more detail information about `ntc js`, see author's comments of [`ntc.js`](https://github.com/atmarksharp/ntc.php/blob/master/original/ntc.js).

## Sample Usage

```php
<?php

require 'ntc.php';

$n_match  = NTC::name("#6195ED");
$n_rgb        = $n_match[0]; // This is the RGB value of the closest matching color
$n_name       = $n_match[1]; // This is the text string for the name of the match
$n_exactmatch = $n_match[2]; // True if exact color match, False if close-match

var_dump($n_match);

// array(3) {
//   [0]=>
//   string(7) "#6495ED"
//   [1]=>
//   string(15) "Cornflower Blue"
//   [2]=>
//   bool(false)
// }
```

## License

CC By 2.5
http://creativecommons.org/licenses/by/2.5/

Original version was created by Chirag Mehta, And ported to PHP by atmarksharp.

<a rel="license" href="http://creativecommons.org/licenses/by/2.5/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/2.5/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/2.5/">Creative Commons Attribution 2.5 Generic License</a>.
