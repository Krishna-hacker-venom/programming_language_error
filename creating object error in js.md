 you’re trying to mix a statement (console.log) inside an object literal, which isn’t valid JavaScript syntax. Objects can only contain key-value pairs (properties) or methods (functions).

 // creating a js object
const user = {
    name : "krishna",
    age : 22,
    isdev : false,
    console.log("hello world!!"); // here this is wrong
}

correct vrsion of code : 
// Object
const user = {
  name: 'Alice',
  age: 25,
  greet() {
    console.log(`Hi, I'm ${this.name}`);
  }
};
