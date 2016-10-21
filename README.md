# NotesToMyself

20-Oct-2016

# PHP notes.

### String operations
. is a concatenation operator.

strtoupper --> function to change to Uppercase.

strtolower

ucwords --> capitalize of html.

#### length
strlen("hi");

output: 2

#### replace 
$msg = 'Have a nice day!'
str_replace('nice','great',$msg); 

output-> Have a great day!

#### repeat
str_repeat($msg,3);

output: Have a great day!Have a great day!Have a great day!

#### substring
substr($msg,5,16); // params: string,startingIndex,endIndex(If endIndex omitted prints entire string from the start44ing index)

output: a great day!

#### If string is present in other string.
strstr($msg,"nice");

output: nice day! (prints everything after the match.)

#### String position
strpos($msg, "nice");

output: 7

#### If character present in string.
strchr($msg, 'i');

output: ice day! (prints everything after the match.)

### Numbers


As in C, it supports pre-increment/decrement and post-increment/decrement.

#### Abs
abs(-99);

output: 99

#### power
pow(2,10); //base,power

output: 1024

####  Generating random number
rand();
rand(12,29); // lower limit,upper limit

output: Generates random number

#### mod
fmod(27,5); // dividend,divisor

output: 2

#### Square root
sqrt(225);

output: 15

#### Round
$num = 15.6589;
round($num,2); // number,how many decimal places

output: 15.66

#### Ceiling
ceil($num);

output: 16

#### Floor
floor($num);

output: 15

#### To test if its a integer.
is_int($num); // Return 1 if yes, nothing if no.

output:  (nothing)

#### To test if its a float.
is_float($num); 

output:  1

#### To test if its a number.
is_numeric($num);

output: 1

### Arrays

#### Syntax 
$arr = array(.....); // Items can be of any type
$arr = array(12,34.56," savita "," Misa Misa ",["dangs",24, 7], " bar "," Yagami ");
$arr[2];

output: savita

echo $arr[6] . $arr[4][0] . $arr[3] . $arr[4][1] . $arr[5] . $arr[4][2];

output: Yagami dangs Misa Misa 24 bar 7 

#### print_r function
print_r($arr);

output Array ( [0] => 12 [1] => 34.56 [2] => savita [3] => Misa Misa [4] => Array ( [0] => dangs [1] => 24 [2] => 7 ) [5] => bar [6] => Yagami ) 

### Associative arrays

$arr = array("name"=>"John", "sex"=>"unknown");
echo $arr1[sex] . "<br>";

output: unknown

$arr2 = array(array("name"=>" Lindsy ","age"=>24), array("name"=>" Logan ","hobbie"=> " dangs "));
echo $arr2[1]["name"] . $arr2[1]["hobbie"] . $arr2[0]["name"] . "<br>";

output: Logan dangs Lindsy 
