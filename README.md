# Install webpack-dev-server and run project via that

This simple project explain how to add webpack-dev-server.

1. Add webpack-dev-server plugin into npm
   >npm install webpack-dev-server  --save-dev   
   
   //--Save -dev helps you to add plugins to package.json file

2. Package.json looks like
	{
	  "name": "first_project_webpack",
	  "version": "1.0.0",
	  "description": "sample project webpack",
	  "main": "index.js",
	  "scripts": {
		"test": "echo \"Error: no test specified\" && exit 1",
		"build": "webpack-dev-server --entry ./src/js/index.js --output-filename ./dist/bundle.js",
		"build:prod": "webpack src/js/index.js dist/bundle.js -p"
	  },
	  "author": "vijayabal",
	  "license": "ISC",
	  "devDependencies": {
		"webpack": "^3.6.0",
		"webpack-dev-server": "^2.9.1"
	  }
	}	
  
