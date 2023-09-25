# Type_Script_Intro

## What and Why 

 - TypeScript extends JavaScript and uses static typing in place of dynamic type 
 - with TypeScript you can declare a type before hand for your function to advoid errors in large projects.

	an example of this is 

	function add ( a: number, b: number) {
				return a + b ;
				}
				const result = add ( '2', '5');

	in JavaScript this will return 25 due to concatenation of the strings, in TypeScript the function can not run, due to the number type being set within the funtion.
##  Install and Using TS

 - to install TS locally type npm install typescript into the terminal
 - npx tsc is the comand for the TS compiler and you can point to which file you want to compile 
 - with npx init -y you can make a empty JSon Package 
  ## Primitives

These are the basic JS type, number, string, boolean. In TS the need to be lowercase to start to not point to an object. 

ex: let userName: string;
userName = 'Kyle'; 
## More complex types
writing a string in TS requires you to set :[] as the type, and with an object you will need to set as :{}.

ex: let person: {
		name: string;
		age: number;
		};

this lets you set an obeject an only accepts these types within it.
also you can do the same and add an array within the type.
## Type inference
TS will infer the type you are using without you needing to tell it 
ex: let course = 'this course'
here TS will set the type to a string 
## Union Types
you are allowed in TS you set more than one type using a pipe ( | ) 
ex: let course: string | number;
ex: let userName: string | string[];
## Type Aliases 
you may assigin an type aliases to make your own types which when complied when go away, but can reduce the amount of code within your TS files. This is done using the type keyword.
## Functions & Types
you may set types to the param of a function as well as the return.
### Generics 
let you make a flexable type using <T> after your function name which allows you to tell TS the type is not any. And set mulitple thing to the same type to utaliz inference.
## Classes 
you are able to set class types all within a constructor while also setting the classes to public/ private for use outside of the method.
## Interfaces
allow you to create a groundwork for classes that then let you implement that into a object and forces you follow the same groundwork of the class.