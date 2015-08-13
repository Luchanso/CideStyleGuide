
```haxe
function example() {

    //bad. no braces, single line code.
    if(true) return;

    //good
    if(true) {
        return;
    }

} //example
```

### Classes
* public variables always first
* after public variables, group properties together
* private variables next
* methods - constructor/init first, then destroy/cleanup
* methods - public facing api higher up
* methods - internal api next
* methods - private/internal/utility functions last

### Class format guidelines

* two lines gap
  * between imports and package
  * between imports and class declaration
  * between class declaration and member declaration
  * between member declaration and functions
  * between last function and close brace
* one line gap at the end of the file

```haxe
package example;


import things;
import more;


class Example {


    public var one : Int;
    public var two : Bool;

    public var property (get,set) : String;

    var three : String;


    public function new() {

    } //new

    public function destroy() {

    } //destroy

    function internal() {

    } //internal


} //Example
```
