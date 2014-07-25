Bower Cheat Sheet
=======================

##Installation
* node.js: [download](http://nodejs.org/download/)
* Requires Git
  * Mac: installed
  * Windows: mysysgit [download](http://msysgit.github.io/)
* ```npm install bower -g```


##Installing Packages
####Basic Installation Steps
1. Go to the project folder (using a Terminal program: e.g. ```cd ~/Documents/my_project/```
2. Install the package <br>
   ```bower install <package-name>``` <br>
   For example: ```bower install jquery``` 

####More Installation Options
```bower install <package-name>#<version>``` <br>
Install particular version of package. For example: ```bower install jquery#1.11```

```bower install <package1-name> <package2-name> <package3-name> <package4-name>``` <br>
Install multiple packages at once

####Specifying Where Bower Installs Packages
Normally, bower install packages in your project's root directory in a folder named ```bowser_components```. If you want to change where the packages are installed -- for example, in a ```js``` or ```js/libs``` folder, you need to create a file named ```.bowerrc``` in the project directory. That file should have a simple JSON string formatted like this:

```javascript
{
     "directory" : "js/lib"
}``` 

The path to the directory is relative to the project directory (and where the ```.bowerrc``` file is located.)

Bower can only install into one location, so if you want separate installations within one project -- for example ```js/libs``` (for production libraries) and ```test/libs``` (for testing libraries) -- you need to 
