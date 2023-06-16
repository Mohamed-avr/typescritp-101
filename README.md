# typescript-101
typescript 101 is the course that I'm learning so I decided to share any experiences I face 

## Content 
 - [introdaction](#introdaction)
 - [install typescript & compile TS with js ](#install)
 - [create a configuration and watch files ](#empty)

## <a id="introdaction"></a>introdaction 
  ### What is typesciprt ? 
  1. typescript is a strongly typed programming language that builds on javascript 
  2. typescript developed by Microsoft 
  3. typescript is javascript with types 
  4. typescript adds features to javascript without changing it 


### Why do we need typescript?
* detect errors without running the code this is called "static type checking" 
   - that means you can find the error while typing before going to another thing 
* analyze the code as you type 
* save some unit tests as the error shows while writing 
* every JS file is a valid TS file  
   - that means you can write javascript code inside a typescript file or code 
* will help you when you write react,vue, angular, next.. apps 
* gives you the missing features in JS like "interfaces, generics, decorators" 

### How typescript works 
 - typescript compiler compiles TS code into JavaScript code "This Called Transpitaltion"
 - what about the new features in typescript that are not in js when the code of TS is compiled into js code. 
    - there is something called a workaround is simulating the features of TS that do not exist in JS 

### What you need to know 
- javascript concepts (basic):
  - variables 
  - arrays 
  - objects 
  - functions 
  - conditions 

## <a id="install"></a> install typescript & compile TS with js 
what we will learn is how to install typescript and how to compile TS with JS 
so first you need to check if you have Node.js by this code below using terminal, Bash, or Powershell.

```
node -v 

ex:v19.8.1
```
if you don't have the node.js on your computer go to install it from this [website](https://nodejs.org/en)
then install TS on your computer following this code : 
```
npm i -g typescript
```
after this check if TS installed by cmd or bash 
```
tsc -v 
ex: Version 
```
now create a folder and open it in any editor to make the procces easier after this we will go to compile TS file with the Js file 
first, create a typescript file inside that folder like this one here : 

![index ts - typescript-101 - Visual Studio Code 6_6_2023 1_31_11 PM](https://github.com/Mohamed-avr/typescritp-101/assets/58856307/fbb60349-2e55-4766-8bdb-7a0893c1aaf1)


I created the file of TS and I name it index.ts you can give it the name you want also you see the folder name is typescript-101

now if let's try to code and  then we will compile it to js code
this below is typescript code we will compile it now 

``` 
const generateIDs= 1245;
console.log(Math.random() * generateIDs );
``` 
now in the same editor open the terminal and write this commend : 

``` 
tsc index.ts
```
now look to the folder you will see a new js file created has the same name with Ts file like this below :
![● index ts - typescript-101 - Visual Studio Code 6_6_2023 2_51_30 PM](https://github.com/Mohamed-avr/typescritp-101/assets/58856307/ff8efe56-1209-42eb-9543-149e0b613bc9)

to combile a TS  code to JS code this means to create another JS file 



