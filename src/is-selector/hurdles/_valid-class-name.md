//Task: Write a scss function to test a string using only scss syntax and follow the instructions in the comment.

// $class-part-until: (" ", ".", "#", ":", ">", "+", "~", "*" );
// $class-part-attr: ("[", "]");
// $class-part-function: ("(", ")");
// $letters: 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ';
// $numbers: '0123456789';
// $special: '-_';
// $all-allowed-chars: $letters + $numbers + $special

// Example function

// 1. get the $string
// 2. check if first char in $string is a "." -> null
// 3. check if second char in $string is a digit -> warning, null
// [ must be followed by ], and ( must be followed by )
// 4. find location of first list item $class-part-attr in $string
//     a. if not found -> go on
//         - if found -> search for second list item $class-part-attr in $string
//     b. if location of first list item is bigger then location of second list item -> warning, null
//         - if location of first list item is smaller then location of second list item -> go on
// 5. find location of first list item $class-part-function in $string
//     a. if not found -> go on
//         - if found -> search for second list item $class-part-attr in $string
//     b. if location of first list item is bigger then location of second list item -> warning, null
//         - if location of first list item is smaller then location of second list item -> go on
// 6. find location of $class-part-until in string and cut it before this location
//     - ignore first char in $string, because it is a "." and check if this part contains only $all-allowed-chars
//     - if yes -> return $string
//     - if no -> return warning, null
// 7. return $string

// You can use my functions in addition to the standard SCSS functions, like str-slice or str-index if needed.
//
// @function str-split($string, $separator) {
//   $split-arr: ();
//   $index: str-index($string, $separator);
//   @while $index != null {
//     $item: str-slice($string, 1, $index - 1);
//     $split-arr: append($split-arr, $item);
//     $string: str-slice($string, $index + str-length($separator));
//     $index: str-index($string, $separator);
//   }
//   $split-arr: append($split-arr, $string);
//   @return $split-arr;
// }
//
// @function str-trim($string) {
//   @while str-slice($string, 1, 1) == ' ' {
//     $string: str-slice($string, 2);
//   }
//   @while str-slice($string, -1) == ' ' {
//     $string: str-slice($string, 1, -2);
//   }
//   @return $string;
// }




