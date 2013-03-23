# PythonMarkdownCompiler
Batch compiling markdown files to html using python-markdown2. 
## Usage
There are 2 versions available. 
## md-render
Intended for simple processing. Also includes a basic batch processor. 

* `md-render FILENAME [OUTPUT]` Highlights FILENAME. OUTPUT can be an output file. Defaults to stdout. 
* `md-render INFOLDER OUTFOLDER` Basic batch processing. Deprecated in favor of md-render2. 
## md-render2
Intended for batch processing bigger directories. 

* `md-render2 INFOLDER OUTFOLDER` Highlight all *.txt, *.md and files without extension in INFOLDER and save them as FILENAME_WITHOUT_EXTENSION.html in OUTFOLDER. Also adds a navigation  of the form /index => /myfolder/index => /myfolder/myfile. 
HTML Titles will be added as being the first heading in the rendered files. 
## Dependencies

* [python-markdown2](https://github.com/trentm/python-markdown2)
	* Install: `pip install markdown2`, `pypm install markdown2` or `easy_install markdown2`
	* License: [MIT License](https://github.com/trentm/python-markdown2/blob/master/LICENSE.txt)

* [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/)
	* Install: `pip install beautifulsoup4`, `easy_install beautifulsoup4` or the package `beautifulsoup4` in some recent verions of debian / ubuntu
	* License: MIT license

##License
		    DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
		            Version 2, December 2004

	 Copyright (C) 2013 Tom Wiesing <tkw01536@gmail.com>

	 Everyone is permitted to copy and distribute verbatim or modified
	 copies of this license document, and changing it is allowed as long
	 as the name is changed.

		    DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
	   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

	  0. You just DO WHAT THE FUCK YOU WANT TO.
