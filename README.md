# :basecampy: Typescript-101
typescript 101 is the course that I'm learning so I decided to share any experiences I face 

## Content 
 - [introdaction](#introdaction)
 - [install typescript & compile TS with js ](#install)
 - [create a configuration and watch files ](#createConfig)

 ## :arrow_forward: <a id="introdaction"></a>introdaction 
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

## :arrow_forward: <a id="install"></a> install typescript & compile TS with js 
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
now look to the folder you will see a new js file created has the same name as Ts file like this below :
![● index ts - typescript-101 - Visual Studio Code 6_6_2023 2_51_30 PM](https://github.com/Mohamed-avr/typescritp-101/assets/58856307/ff8efe56-1209-42eb-9543-149e0b613bc9)


to compile a TS  code into JS code means creating another JS file 



  ## :arrow_forward: <a id="createConfig"></a> Create a configuration and watch files 
   - ### :shipit:   Only one Typescript file?
  we will not translate TS code into JS code every time we update TS code by typing for  
  that we will configure a file for TS that every change in the TS code file will also appear directly in JS file.  

  ``` 
  Tsc -w index.ts
  ```

this is if you have only one file called "index.ts" example  


 -  ### :shipit:  Many Typescript files ?
  we will create a dist folder :open_file_folder: ( distribution source ) based on our Typescript files and every change in each file will appear in JS files that gonna create in a dist folder :open_file_folder: 
   * First create TS files
   * Then move them to a new folder "src" folder , like this example :
     
   ![home ts - typescript-101 - Visual Studio Code 7_1_2023 6_00_25 PM (2)](https://github.com/Mohamed-avr/typescritp-101/assets/58856307/f3bc176e-f94f-48ae-aa99-8c64136324f5) 
   
   * Now we will initial typescript language using this command :
    ``` 
    Tsc --init
    ```
   now we have "tsconfig.json" .
  * After that we will config "src" folder :open_file_folder: that we create to "dist" folder  :open_file_folder:
    this is by jumping to "tsconfig.json" and do these changes :
     
    ``` 
  "rootDir" : "./src", 
  "target" : "es2016", 
  "outDir" : "./dist",
    ```
    note :exclamation: >> You can do many things you can hide comments you can make it more strict with this JSON file ... but now this is enough  


  * now type this command to make the changes :
    ```
    tsc
    ```
    but this will create only the dist folders with JS files and will not watch the TS files, let's make it happen!
    





  
  

