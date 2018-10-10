# basic-webapp

> A Vue.js project

## Build Setup

## Set up the development environment
```First you need to check your vue version by typing in vue --version. 
If there is no installed version of Vue then you must type into the terminal 
`code` npm install -g vue-cli `code`

After this step then you must bootstrap the project by typing `code` vue init webpack test-project `code` into
the terminal. You can give the project a name and then select enter on the next two prompts. 
Select Read-only on the vue build prompt and then select no on all remaining prompts 
to successfully create your project skeleton.```

## Build the code for deployment and how to run the development server
Now you will have to install the Node modules so cd into the project folder name so type in 
 `code`cd test-project `code` or whatever name you gave it into your terminal to change directories. 
After you have done this, type `npm install` and follow that with `code` npm run dev `code` to 
deploy the site for testing. 

## Deploy Site
To deploy the site, you must first alter the configuration so Webpack builds the code in a `code` docs/ `code` 
directory instead of the  `code` dist/ `code` directory which is the default. To do this you must open the
 `code` config/index.js `code` file and change
`code`index: path.resolve(__dirname, '../dist/index.html'),
    assetsRoot: path.resolve(__dirname, '../dist'),
    assetsPublicPath: '/',``` to 
    ```index: path.resolve(__dirname, '../docs/index.html'),
    assetsRoot: path.resolve(__dirname, '../docs'),
    assetsPublicPath: '',`code`

# Now you can type in `code` npm run build `code` in your terminal to process the code, and build the site.

For a detailed explanation on how things work, check out the [guide]
(http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
