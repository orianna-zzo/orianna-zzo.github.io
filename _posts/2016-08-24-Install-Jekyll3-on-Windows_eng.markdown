---
layout: post
title:  "Install Jekyll3 on Windows"
date:   2016-08-24 01:16:28 +0800
categories: CS
tags: gitpage, CSS, jekyll
---

I planned to build my own website long time ago. Finally, I'm ready to take action. Github page seems to be a great choice. It's time to learn how to build it. There are more tutorials on Linux than on Windows for beginers. Let's try and learn.



#### Reference


## Preparation

# 1. Install Ruby

 * Dowanload Ruby2.3.1(x64)from [here](http://rubyinstaller.org/downloads/)

__Attention__:

 - No spaces in any folder name of path
 
 - Choose "Add Ruby executables to you PATH"
 
![1. install ruby](/images/2016-8-24/1.rubyinstall.png)

 
 * Then check Ruby with cmd

```
ruby -v
```
![2. check ruby](/images/2016-8-24/2.rubycheck.png)



# 2. Install Ruby Devkit

 * Download Devkit from the [same website](http://rubyinstaller.org/downloads/). 
The devkit is a toolkit for developers to build and use extensions for Ruby on Windows much easier. [Here](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit#building-the-devkit)
is the wiki for devkit, including the installation instructions.
There are three versions:

 __Ruby1.8.7 to 1.9.3__: DevKit tdm-32-4.5.2-20111229-1559-sfx.exe 
 
 __Ruby 2.0.0 & above (32bits version only)__: DevKit mingw64-32-4.7.2-20130224-1151-sfx.exe
 
 __Ruby 2.0.0 & above (x64 only)__: DevKit mingw64-64-4.7.2-20130224-1432-sfx.exe

I've downloaded DevKit-mingw64-64-4.7.2-20130224-1432-sfx.exe. I failed to install the devkit in Program Files. I had to install it in C:\DevKit

![3. devkit fail](/images/2016-8-24/3.devkitfail.png)

 * Go to the devkit directory and initialize config.yml 
 
 
 ```ruby dk.rb init```
 
 comfig.yml file will be auto-generated. You can check the file with
 
 ```notepad config.yml```
 
 '-C:\Ruby23-x64' is at the end of the file
 
 ![4. initial devkit config](/images/2016-8-24/4.initdevkitconfig.png)
 
 
 * _[optional]_ Review the list of Rubies 
 ```ruby dk.rb review```
 

#