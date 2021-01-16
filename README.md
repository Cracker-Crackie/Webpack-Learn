
# INTERVIEW QUESTION - WEBPACK

 ## Introduction
 Basic of Webpack [Bundle your Code]
 

**webpack** is an open-source JavaScript module bundler. It is made primarily for JavaScript, but it can transform front-end assets such as HTML, CSS, and images if the corresponding loaders are included. webpack takes modules with dependencies and generates static assets representing those modules.
 
**webpack**  is a  _static module bundler_  for modern JavaScript applications. When webpack processes your application, it internally builds a  [dependency graph](https://webpack.js.org/concepts/dependency-graph/)  which maps every module your project needs and generates one or more  _bundles_.


To get started you only need to understand its  **Core Concepts**:

-   [Entry](https://webpack.js.org/concepts/#entry) An **entry point** indicates which module webpack should use to begin building out its internal dependency graph.

-   [Output](https://webpack.js.org/concepts/#output) The **output** property tells webpack where to emit the _bundles_ it creates and how to name these files. It defaults to `./dist/main.js` for the main output file and to the `./dist` folder for any other generated file.

-   [Loaders](https://webpack.js.org/concepts/#loaders) Out of the box, webpack only understands JavaScript and JSON files. **Loaders** allow webpack to process other types of files and convert them into valid modules that can be consumed by your application and added to the dependency graph.

-   [Plugins](https://webpack.js.org/concepts/#plugins) While loaders are used to transform certain types of modules, plugins can be leveraged to perform a wider range of tasks like bundle optimization, asset management and injection of environment variables.

-   [Mode](https://webpack.js.org/concepts/#mode) By setting the `mode` parameter to either `development`, `production` or `none`, you can enable webpack's built-in optimizations that correspond to each environment. The default value is `production`.

-   [Browser Compatibility](https://webpack.js.org/concepts/#browser-compatibility) webpack supports all browsers that are  ES5-compliant  (IE8 and below are not supported). webpack needs  `Promise`  for  `import()`  and  `require.ensure()` If you want to support older browsers, you will need to  load a polyfill  before using these expressions.

## Why webpack

To understand why you should use webpack, let's recap how we used JavaScript on the web before bundlers were a thing.

There are two ways to run JavaScript in a browser. First, include a script for each functionality; this solution is hard to scale because loading too many scripts can cause a network bottleneck. The second option is to use a big  `.js`  file containing all your project code, but this leads to problems in scope, size, readability and maintainability.

> **IIFE's - Immediately invoked function expressions
> Birth of JavaScript Modules happened thanks to Node.js
> npm + Node.js + modules -- mass distribution
> ESM - ECMAScript Modules
> Automatic Dependency Collection**



- What is webpack, difference between webpack 4, 5. What is Zero config?
- What is the main difference between webpack and other build tools like gulp or grunt & which to use ?
- What is Gulp?
- What is Grunt?
- What is a bundle in webpack?
- Types of webpack env?
- What is an entry point concept in Webpack?
- What is a dependency graph?
- Which modules design patterns webpack supports out of the box?
- What is webpack's config file?
-  What is multiple entry points in a webpack configuration file & how to define multiple Entry point?
- Can we have multiple configurations for different env?
- What is a loader in webpack?
- Different types of loader & Where should loaders be defined?
- Explain Loader Rule ?
- What is synchronous & an asynchronous Loader & example?
- Is it possible to use multiple loaders in the rules single object?
- Name some commonly used Loader & example?
- What is a plugin in webpack?
- loader v/s plugin?
- What is CompressionPlugin?
- Name some plugins & example ?  
- What is custom way of writing a plugin?
- Features of Loader & Plugin
- What is module Resolution & types of path?
- What is Manifest ?
-  What is webpack runtime?
- What is HMR (Hot Module Replacement) ?
- What is Babel ? How to configure Babel?
- Commonly used Plugin's:
``AutomaticPrefetchPlugin,
CommonsChunkPlugin,
CopyWebpackPlugin,
CssMinimizerWebpackPlugin,
DefinePlugin,
EnvironmentPlugin,
EslintWebpackPlugin,
HashedModuleIdsPlugin,
HotModuleReplacementPlugin,
HtmlWebpackPlugin,
ImageMinimizerWebpackPlugin,
MinChunkSizePlugin,
MiniCssExtractPlugin,
NoEmitOnErrorsPlugin,
PrefetchPlugin,
ProvidePlugin,
SourceMapDevToolPlugin,
SplitChunksPlugin,
HtmlWebpackPlugin,
TerserWebpackPlugin``

- What is webpack-dev-server? How to configure Webpack_server?
- On which platform is webpack-dev-server developed?
- What is source maps? How to enable in webpack bundles?
- How to automatically build and update bundles in the browser after a change in source code?
- Explain caching and how to achieve it using webpack?
- What analysis tools do you use for webpack bundle's inspection?
- What is webpack code splitting & which pulgin to use?
- Is it possible to use other languages (except javascript) for the webpack config file?
- What is the difference between tree shaking and dead code elimination.
- Explain me the difference between NPM vs. Bower vs. Browserify vs. Gulp vs. Grunt vs. Webpack?
- What is Parallel-Webpack?
- Types of Hashing in webpack?
- What if we change ‘./greeting.js’ to ‘greeting.js’ ? What will happen?
- What is the difference between source code and distribution code when working with Webpack 5?

> Source code --> actual code

> Distribution code -> compiled code

- What are optimization option in Webpack?
 **optimization.minimize** - to minimize bundle file & by default uglify-js
 **optimization.minimizer** - to provide which minimizer technique to use
**optimization.splitChunks** - The SplitChunksPlugin allows us to extract common dependencies into an existing entry chunk or an entirely new chunk. Always enabled.
**optimization.runtimeChunkFinds** - modules which are shared between chunk and splits them into separate chunks to reduce duplication or separate vendor modules from application **modules.optimization.noEmitOnErrors** - Enabled in production mode. Elsewise disabled. Don’t write output assets when compilation errors. unable to use working part of the application. And no broken bundles.

- How does SplitChunksPlugin prevent duplication?
- What does the webpack-bundle-optimize-helper tool offer? 
- What are differences between SystemJS and Webpack?
- How to create multiple output paths in Webpack config?
- AMD vs CommonJS ?

Study Url's: 

•https://github.com/kukuu/webpack
•https://developpaper.com/collection-of-webpack-interview-questions/
•https://blog.jakoblind.no/how-webpack-decides-what-to-bundle/
•https://docs.w3cub.com/webpack/plugins/mini-css-extract-plugin/
•https://medium.com/@craigmiller160/how-to-fully-optimize-webpack-4-tree-shaking-405e1c76038
•https://webpack.js.org/loaders/
•https://github.com/systemjs/systemjs
•https://medium.com/@imranhsayed/webpack-loaders-and-plugins-e13f79fe6b32
•https://alligator.io/tooling/webpack-gulp-grunt-browserify/
•https://fedev.tech/topic/webpack
•https://stackoverflow.com/questions/37452402/webpack-loaders-vs-plugins-whats-the-difference/38281240#38281240
•https://medium.com/@Rich_Harris/tree-shaking-versus-dead-code-elimination-d3765df85c80










