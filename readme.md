
Intro on what the tutorial will do and the tech used ex:

Techonologies used:
- Vue
- Nuxt
- Webpack
- Babel
- Sass
- Pug
- Vuex
- Axios
- Buefy
- Bulma

# 1. Installation from scratch
First we need to create a folder where our project would be located and initialize a package.json.
```shell
$ mkdir nuxt-practice
$ cd nuxt-practice/
$ npm init
```
After the initialization of package.json, let's install the Nuxt.js by typing
```
$ npm install --save nuxt
```
Then let's add a script for Nuxt.js by opening the package.json from your favorite text editor and adding the line
``` "dev": "nuxt" ``` to the scripts. 

Your folder and package.json should look like this.
![image of package.json and folder structure](https://raw.githubusercontent.com/trleonarddalmacio/images/master/nuxt-tutorial/https://raw.githubusercontent.com/trleonarddalmacio/images/master/nuxt-tutorial/1.%20Intro%201.png)

To verify that it's running correctly let's create a folder named **pages**, and create an **index.vue** file inside the created folder. 

**NOTE:** The pages folder will serve as the routing path in the parameter field. 

For example,
You have a site called **googlee<span></span>.com**
The file in the **/pages/users/index.vue** will be automatically routed and rendered to **googlee<span></span>.com/users**.

More of this would be discussed later.

Coming back, inside the index.vue file lets add a template with Hello World.
```html
<template>
	<div>
		<h1>Hello WORLD!</h1>
	</div>
</template>
```
Then run
```
$ npm run dev
```
Now your file should be running at **http://localhost:3000/**
![alt-text](https://raw.githubusercontent.com/trleonarddalmacio/images/master/nuxt-tutorial/1.%20Intro%202.png)


# 2. Directory Structure
There are 8 folder and 2 files that are important for Nuxt.js. Included in those are the **pages** folder and the **package.json**, but in this tutorial, we would not be using all of them. Still, I would be creating all of them.

Let's create the other 7 folders (**assets**, **component**, **layouts**, **middleware**, **plugins**, **static**, ) and the file **nuxt.config.js**

My current folder structure look like this:

![alt-text](https://raw.githubusercontent.com/trleonarddalmacio/images/master/nuxt-tutorial/2.%20Directory.png)

If your unsure of what is the purpose of each folder, you can refer to the [official Nuxt.js documentation](https://nuxtjs.org/guide/directory-structure). 

# 3. Routing