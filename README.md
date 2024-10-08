## _Commands_

- **if you wanna see the list of commands you can use with ts files, you can hit this command ➡ `tsc -h`.**
- **the command of run ts file ➡ `tsc fileName`.**
- **the command of run ts file in watch mode ➡ `tsc -w fileName`.**
- **to create tsConfig file ➡ `tsc --init`.**
- **if you wanna compiled the whole project, not specific file ➡ `tsc`.**
- **if you wanna compiled the whole project but in watch mode, not specific file ➡ `tsc -w`.**

---

## _Type Annotations Or Signature_

- **Indicate the data type of the variable.**
- **Indicate the data type of the Functions input/output.**
- **Ojects, etc.**

- **Why we use it ? `to force the type checking`.**
- **Is it mandatory ? `No it's not mandatory`.**
- **What happen if we did'nt use it ? `compiler will guess the type depend on the value of the variable`.**

---

## _Statically Types vs Dynamically Types_

### _Statically Types_

- **Languages like [Rust, C, C++].**
- **variables types are static, once you declare it you can't change it.**
- **Type of A variable is known at compile time "Do type checkin at compile time".**
- **Have better performance at run-time due to not nedding to check types dynamically.**
- **Error detected earlier.**

### _Dynamically Types_

- **Languages like [Php , Python, Javascript].**
- **variables types are dynamic, you can always change it.**
- **Type checking at Execution time.**
- **Error can be detected after Execution time.**

---

## _Data Types_

### _Enums_

- **Enums ➡ Enumerations.**
- **Allow us to declare `a set of named constants`.**
- **Used for logical grouping collection of constants `Collection of related values`.**
- **Enum can refer to other enum.**
- **Enum can refer to same enum.**
- **Enum can have calculations.**
- **Enum can have functions result as its value.**
- **It organize your code.**
- **By default enums are number-based, first element is 0.**
- **There's a numeric enums.**
- **There's a string-based enums.**
- **There's heterogeneous enums [string + number] .**
- **You can declare an enum by ➡ `enum level {easy = 10, medium = 15 , hard = 20 }`, you can add value to each key or just use the default values like this ➡ `enum level { easy, medium, hard }`.**

### _Tuple_

- **Is another sort of `array` type.**
- **most used in `ReactJs`.**
- **We know exactly how many elements it contains.**
- **We know which types it contains at specific positions.**
- **`For example ✔` ➡ `let article : [number, string, boolean] = [11, "title", true]`.**
- **Also I can add `readonly`, ➡ `let article : readonly [number, string, boolean] = [11, "title", true]` , Therefore He can't add anything to it just read.**

### _Void_

- **⚠ We use it with function will return nothing ⚠**
- **Even if i wrote `console.log()` and it already printed a message, This is not a return value so it's void value.**
- **If i wrote just `retutn;` it's void value.**
- **Function in `JS` that not return a value will show undefined - And undefined In not void.**

### _Never_

- **Return type never returns.**
- **The function doesn't have a normal completion, the type of this function should be ➡ `never type`.**
- **It throws an `Error` Or Never finishes running at all "infinite loop", All these cases are ➡ `never type`.**

### _Union_

- **The `|` symbol is used to create the union ➡ `OR`.**

### _Intersection_

- **Is a type that combines several types into one.**
- **The `&` symbol us used to create an Intersection.**

- **`If a union is an "OR", then an Intersection is an and`**

---

## _Data Alias_

- **I can give a shortcut to the types and use it ➡ `type st = string` and use `st` instead of `string`.**
- **this method in case if I write the data type names many times and I wanna minimize letters as much as I can.**
- **Also I can create an object and assign many types on it like ➡ `type userInfoTypes = {name: string, age: number, worked: boolean}` and use `userInfoTypes` as datatype set for passing it into the function.**
- **Depend on the last method, After createing an object has userInfoTypes, I can add additional type like ➡ `type last = userInfoTypes & {married : boolean}`.**

---

## _Interface_

- **Serve like types.**
- **Interface describes the shape of an object.**
- **It defines the syntax to follow.**

- **Use with [ object, function ].**
- **Use readonly and optional operator.**

---

## _OOP_

### _Polymorphism & Method Override_

#### _Polymorphism_

- **Classes have the same methods but different implementations.**
- **.**

#### _Method Override_

- **.**

### _Abstract Classes & Members_

- **You can define an abstract class by write keyword `abstract` before the class name like this ➡ `abstract className { }`.**
- **We can't create an instance of an abstract class, `All what you can do is inherit from it`.**
- **We also have `abstract methods`, which means you must implement these methods in all subclasses of the abstract class, And you can define `abstract method` by write the keyword `abstract` before the method name.**
- **You can't write any code in an `abstract method` within an `abstract class`, you can only define the method.**

### _Class Implements Interface_

- **How to implement specific interface while we creating the class ? `This means that all elements in the interface must be implemented in the class, and you're free to add additional properties that don't exist in the interface`.**

### _Static Members_

- **Static members are the `properties & methods` that belong only to class itself, not to the `objects` that we created from the `class`.**
- **Don't use "name, length, call"**

### _Get And Set Accessors_

- **`Get And Set Accessors` are `functions` start with `[ set | get ]` help me get data from `private property` Or set value to `private property` ➡ `get funcName(): string { returm this.username}` Or `set funcName(value: string) { this.username = value}`.**

### _Data Access Modifiers & Parameters Properties_

#### _Public_

- **All members of a class is typescript are public.**
- **All public members can accessed anywhere without any restrictions.**

#### _Private_

- **Members are visible only to that class and are not accessible outside the class.**

#### _Protected_

- **Same like `private` but can be accessed within the same class and its subClasses.**

---

## _Generics_

- **Help write a reusable code.**
- **Allowto pass type as a parameter to another type.**
- **You will be able to deal with multiple types without using `any` type.**

### _We can create_

- **Generic classes.**
- **Generic functions.**
- **Generic methods.**
- **Generic interfaces.**

## _Shortcuts names_

- **src ➡ Source folder - where we have our ts project.**
- **dist ➡ Distrution folder - where we have a js copy from src.**

---
