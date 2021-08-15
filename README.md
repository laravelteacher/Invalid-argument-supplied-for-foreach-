# Invalid-argument-supplied-for-foreach-


                                              Invalid argument supplied for foreach()
											  
Link Video: https://youtu.be/jYP-Rj1K1wU

It often happens to me to handle data that can be either an array or a null variable and to feed some foreach with these data.

When you feed a foreach with data that are not an array, you get a warning:

Personally I find this to be the most clean - not sure if it's the most efficient, mind!

if (is_array($datas) || is_object($data))
        {
		
		}
		

or

you can use 

foreach ((array) $items as $item) {
 // ...
 }

if (is_iterable($values))
{
    
} 


or 

use

foreach ($arr ?: [] as $elem) {
    // Do something
}

thanks
