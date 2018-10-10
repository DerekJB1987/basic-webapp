# basic-webapp

> A Vue.js project

## Build Setup

``` bash
# First you need to check your vue version by typing in vue --version. 
If there is no installed version of Vue then you must type into the terminal 
`npm install -g vue-cli`

After this step then you must bootstrap the project by typing `vue init webpack test-project` into
the terminal. You can give the project a name and then select enter on the next two prompts. 
Select Read-only on the vue build prompt and then select no on all remaining prompts 
to successfully create your project skeleton.

Now you will have to install the Node modules so cd into the project folder name so type in 
`cd test-project` or whatever name you gave it into your terminal to change directories. 
After you have done this, type `npm install` and follow that with `npm run dev` to 
deploy the site for testing. 

## Deploy Site
# To deploy the site, you must first alter the configuration so Webpack builds the code in a `docs/` 
directory instead of the `dist/` directory which is the default. To do this you must open the
`config/index.js` file and change
```index: path.resolve(__dirname, '../dist/index.html'),
    assetsRoot: path.resolve(__dirname, '../dist'),
    assetsPublicPath: '/',``` to 
    ```index: path.resolve(__dirname, '../docs/index.html'),
    assetsRoot: path.resolve(__dirname, '../docs'),
    assetsPublicPath: '',```

# Now you can type in `npm run build` in your terminal to process the code, and build the site.

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
