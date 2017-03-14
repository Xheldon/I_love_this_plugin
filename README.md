# I love this plugin

### 我用过的一些好用/常用的插件

### 通用:

1. [ora](https://github.com/sindresorhus/ora)
	>用来在控制台显示一个类似于loandig循环转圈的效果
	>
		const ora = require('ora');
		const spinner = ora('Loading unicorns').start();
		setTimeout(() => {
	    	spinner.color = 'yellow';
    		spinner.text = 'Loading rainbows';
		}, 1000);
	
2. [glob](https://github.com/isaacs/node-glob)
	>允许使用在shell中使用的patterns如`*` `?` `[...]`等进行文件匹配
	>
		var glob = require("glob")
		// options is optional
		glob("**/*.js", options, function (er, files) {
		  // files is an array of filenames.
		  // If the `nonull` option is set, and nothing
		  // was found, then files is ["**/*.js"]
		  // er is an error object or null.
		})
1. [colors](https://github.com/marak/colors.js/)
	>用来在控制台输出不同颜色不同背景的字体，其分String原型入侵模式和非入侵模式调用。
	
	>原型入侵式：
	>	
		console.log('i like cake and pies'.underline.red)
	>原型非入侵式：	
	>
		console.log(colors.red.underline('i like cake and pies'))
		
		
2. [dev-cert-authority](https://github.com/latentflip/dev-cert-authority)
	>用来在本地开发过程中使用https调试，尤其是当接口或者数据请求地址为https时尤其有用。

### Webpack(只列出非官方插件)

1. [progress-bar-webpack-plugin](https://github.com/clessg/progress-bar-webpack-plugin)
	>一个进度条插件，用来显示webpack打包任务进度，其中的options与`node-progress`插件一致,配合`colors`插件使用效果更佳
	>
		new ProgressBarPlugin({
		  format: '  build [:bar] ' + chalk.green.bold(':percent') + ' (:elapsed seconds)',
		  clear: false
		})

2. [webpack-merge](https://github.com/survivejs/webpack-merge)
	>一个合并配置插件，类似于jQuery的$.extend()
3. [clean-webpack-plugin](https://github.com/johnagan/clean-webpack-plugin)
	>一个用来打包之前清空目录的插件，需要清空的目录可以以数组的形式传参。

