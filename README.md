# deprecated-dojo

Let's build a complete list of dojo deprecated api, to support [anti-babel](https://github.com/gratex/anti-babel), git-qa and other code quality and refactoring tools.

## Problem

dojo is not very consistent in marking the codes as deprecated, 
this may help you (helped us)

Examples of inconsistencies:

dojo/_base/lang methods 
- not marked in source code
- not marked in api docs (detail.json)
- marked in reference guide

Another problem is that some methods you will never find in documentation:

Example, dojo functional and unzip

	< ../dojo-website/src/documentation/api/1.10/details.json grep unzip

## Install and try
	
	# get tools
	npm install

	# not using submodule, gh-pages problem
	# get/update dojo data (api and reference guide)
	# git submodule init
	# git submodule update

	# do
	git clone -b master --single-branch https://github.com/dojo/dojo-website.git

	# or if clone somewhere on disk adjust paths

	# methods deprecated in API docs (detail.json)
	./bin/deprecated-api dojo-website/src/documentation/api/1.10/details.json

	# modules with some deprecated apis
	./bin/deprecated-reference-guide

Samples:

	./bin/deprecated-api dojo-website/src/documentation/api/1.10/details.json | wc -l
	    1163
	 ./bin/deprecated-api dojo-website/src/documentation/api/1.9/details.json | wc -l
	    1128
	./bin/deprecated-api dojo-website/src/documentation/api/1.8/details.json | wc -l
	     972	



