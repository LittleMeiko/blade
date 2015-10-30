
[![](https://dn-biezhi.qbox.me/LOGO_BIG.png)](http://bladejava.com)

[![Build Status](https://img.shields.io/travis/biezhi/blade.svg?style=flat-square)](https://travis-ci.org/biezhi/blade)
[![maven-central](https://img.shields.io/maven-central/v/com.bladejava/blade-core.svg?style=flat-square)](http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22com.bladejava%22)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![@biezhi on weibo](https://img.shields.io/badge/weibo-%40biezhi-red.svg?style=flat-square)](http://weibo.com/u/5238733773)

[中文](https://github.com/biezhi/blade/blob/master/README_CN.md)

## What Is Blade?

`blade` is a lightweight MVC framework. It is based on the principles of simplicity and elegance. 
If you like it, can be [Star and Fork](https://github.com/biezhi/blade), thanks!

## Features

* [x] Lightweight. The code is simple and structure is clear
* [x] Modular (you can choose which components to use)
* [x] Support plug-in extension mechanism
* [x] Restful style routing interface
* [x] Multiple configuration files support (currently properties, json and coding)
* [x] Eembed jetty server and template engine support
* [x] Support jdk1.6 or higher version

## Overview

* Simplicity. The design is simple, easy to understand and doesn't introduce many layers between you and the standard library. It is a goal of the project that users should be able to understand the whole framework in a single day.
* Elegance. `blade` Support the REST style routing interface, provide DSL grammar to write, no invasive interceptors.

## Getting started

To get started, first [include the Blade library](http://bladejava.com/docs/intro/getting_start) and then create a class with a main method like this:

```java
public class App {
	
	public static void main(String[] args) {
		Blade blade = Blade.me();
		blade.get("/", (request, response) -> {
			response.html("<h1>Hello blade!</h1>");
		});
		blade.listen(9001).start();
	}
}
```

Run it and point your browser to http://localhost:9001. There you go, you've just created your first Blade app!

OK, all this may seem simple, refer to the guidelines for use more ready-made examples for your reference:

+ [HELLO](https://github.com/bladejava/hello)
+ [API DOCS](http://bladejava.com/apidocs/)
+ [USE GUIDE](https://github.com/biezhi/blade/wiki)
+ [EXAMPLES](https://github.com/bladejava)

## Plan

1. Improve the document
2. Add the routing configuration way
3. To develop personalized social applications
4. Maintain and optimize the code
	
## Update

[update log](https://github.com/biezhi/blade/blob/master/UPDATE_LOG.md)

## Contact

- Blog:[https://biezhi.me](https://biezhi.me)
- Mail: biezhi.me#gmail.com
- QQ Group: [1013565](http://shang.qq.com/wpa/qunwpa?idkey=932642920a5c0ef5f1ae902723c4f168c58ea63f3cef1139e30d68145d3b5b2f)

## licenses

```
Copyright 2015 biezhi

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
