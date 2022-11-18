## React Js Tutorial
#### Welcome to this React Js Tutorial
- First, you need to learn and have a better understanding of the prerequisites of HTML, CSS & JAVASCRIPT

- Html is the NOUN of a webpage
- Javascript is the VERB of the webpage because it performs the actions.
- JS uses JIT compiler (just in time compiler)

E.g - function fun(){
          console.log("hello");}

      setInterval(fun, 1000);
// returns hello after every 1sec(1000ms)

     clearInterval(1)
// stops the run

- linking (<script type="text/javascript" src="demo.js</script>)

- alert("Hello user")

- virtual DOM - part of your webpage gets updated or refreshed whenever you send a request or response
- library - (comes with preloaded code)

- (create react app) - creates single page react applications
we get the; -- webpack(minify, bundle, compile)
            -- compiler(jsx - js)
            -- node package manager
            -- development server
          
##### Run the following:-
C:\Users\MARX>npm install create-react-app -g
          
****Running          
npm WARN deprecated tar@2.2.2: This version of tar is no longer supported, and will not receive security updates. Please upgrade asap.

changed 67 packages, and audited 68 packages in 20s

5 packages are looking for funding
  run `npm fund` for details

2 high severity vulnerabilities

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.

##### Changing the root directory
          
C:\Users\MARX>cd Desktop

C:\Users\MARX\Desktop>

##### Creating our folder
C:\Users\MARX\Desktop>md React_tutorial

##### Chaning the root directory to our folder
C:\Users\MARX\Desktop>cd React_tutorial

##### Creating our React app inside this directory
C:\Users\MARX\Desktop\React_tutorial>create-react-app demo_project

##### Javascript essentials to know
          
*****Let Keyword
          
console.log("Global scope");
for (var g_scope = 1; g_scope<5; g_scope++)
{
  console.log(g_scope);//Global scope
}
console.log(g_scope);
          
// Returns the g_scope value 5 times because it can be accessed globally

// Introducing the let keyword
          
console.log("Block scope");
for (let b_scope = 1; b_scope<5; b_scope++)
{
  console.log(b_scope);
}
console.log(b_scope);//Error (Block scope)

*****constant keyword
          
//const value cannot be changed
//you can change the properties of object but not reference


*****function declaration - loads at compile time
          
function execute(){ 
   console.log("Hello");
}
// returns > execute()
           >Hello
           <undefined

*****function expression - loads at runtime
          
var execute = functon name(){
    console.log("Bye");
}
//returns >execute()
          >Bye


*****export keyword
          
Helps us to use one javascript file in another javascript file.

//with default:
          
const academy ={
    name:"GL";
}
export default academy;

//without default:
          
export const subject = "React";

export const status=()=>{
   console.log('Completed');
}

*****import keyword
          
To include the exported file we use import

//with default
          
import academy from './file_name.js';

//without default
          
import {subject} from './file_name.js';
import {status} from '.file_name.js';

*****class(methods & properties)
          
class c_name{
 constructor()
}

*****object(instance of a class)
          
const x = new
c_name();

*****Inheritance (inheriting methods & properties)
          
- super()

*****spread operator
          
- used with arrays or objects
- used to retrieve all values or properties from one array into another
- represented by three dots(...)

const arr = [1,2,3];
const new_arr=[...arr,4];

new_arr 
> [1,2,3,4]
arr
> [1,2,3]

*****Rest operator
          
first;
functon sum(a,b){
  return a+b;
}
console.log(sum(1,2)
//returns value 3
if we > console.log(1,2,3)
//still returns 3 and assumes the rest
hence inconveniences us when we want to add other numbers

//So we'll use the rest operator(...)
          
function sum(..args) //give it a name args
     let total = 0;
     for(let i in args){
         total += args [i];
     }
     return total;
}
console.log(sum(1,2,3,4)
          
//when we console it now returns 10 and thus we can add other numbers.

*****destructuring
          
- A way with which we can extract few elements from the array or few properties from the object.
var values = [10,20,30];
[first,,last] = values;

> first - returns 10
>last - returns 30
//hence we have destructured te array


****Basics of react app
1. node_modules -all packages used by npm
2. public - stores anything that we will render
3. src
4. gitignore- files we want to ignore when exporting
5. package-json - dependencies and files we need 

- Lastly open the demo_project we created and deleted all files in the src directory apart from the index.js and app.js files
- You can then copy the simple code in the app.js and index.js files which is simply a div created with a heading parameter inside.
- Then the root id in the index.html file rendered in the index.js file since it is a global attribute.
 
