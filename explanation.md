  - [x]  *learn* **getter** and ***setter*** methods

```js
let person = {

    firstName:"Farhod",
    lastName:"dadajonov",
    fullName(){
        return person.firstName + ' ' + person.lastName;
    }
}
console.log(person.fullName());
```
here we use the getter property to avoid writing code 
in the form of a function 




```js
let person = {
    firstName:"Farhod",
    lastName:"dadajonov",
    get fullName(){
        return this.firstName + ' ' + this.lastName;
    }
}
console.log(person.fullName);
```
where the results are the same using only the keywords (get, this)
and (fullNmane) is used as a property
this called is getter form

____Now we learn the setter
What is setter?
The setter is to enter information about this 
property in a single row

```js
let person = {
    firstName:"Farhod",
    lastName:"dadajonov",
    get fullName(){
        return this.firstName + ' ' + this.lastName;
    },
    set fullName(value){
        let fullNameArray = value.split(' ');
        this.firstName = fullNameArray[0];
        this.lastName = fullNameArray[1];
    }
}
person.fullName  = 'Soliyev To\'lqinxon';
console.log(person.fullName);
```
the result of our code will now be a tag to the 
newly entered value 
that is 'Soliyev To'lqinxon'
The keywords (set, this) and the and split () method were 
used to generate the setter property

where the split () method is used,
this method returns a string and divides it into values according to the written characters and equals the index.
