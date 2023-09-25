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