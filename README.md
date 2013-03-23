# Python Markdown Compiler
Batch compiling markdown files to html using python-markdown2. Tested with Python 2.7. 
## Usage
There are 2 versions available. 
### md-render
Deprecated in favor of md-render2. 

* `md-render FILENAME [OUTPUT]` Highlights FILENAME. OUTPUT can be an output file. Defaults to stdout. 
* `md-render INFOLDER OUTFOLDER` Basic batch processing. 

### md-render2
Intended for batch processing bigger directories. 

```
usage: md-render2.py [-h] [--no-nav] [--render [EXTENSION [EXTENSION ...]]]
                     [--copy [EXTENSION [EXTENSION ...]] | --no-copy
                     [EXTENSION [EXTENSION ...]]]
                     INFOLDER OUTFOLDER

Python Markdown Compiler

optional arguments:
  -h, --help            show this help message and exit
  --no-nav              Do not render the navigation menu.

Location:
  Where to find the source, where to put the rendered files.

  INFOLDER              Input folder.
  OUTFOLDER             Output folder. Will be created if it does not exist.

File Selection:
  Which files to render, which to copy.

  --render [EXTENSION [EXTENSION ...]]
                        Extensions to render. * is a wildcat and means
                        everything. (Default: ["", "txt", "md"])
  --copy [EXTENSION [EXTENSION ...]]
                        Extensions to copy. * is a wildcat and means
                        everything. (Default: [])
  --no-copy [EXTENSION [EXTENSION ...]]
                        Extensions to exclude from copying. (Default: [""])
```

## Dependencies

* [python-markdown2](https://github.com/trentm/python-markdown2)
	* Install: `pip install markdown2`, `pypm install markdown2` or `easy_install markdown2`
	* License: [MIT License](https://github.com/trentm/python-markdown2/blob/master/LICENSE.txt)

* [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/)
	* Install: `pip install beautifulsoup4`, `easy_install beautifulsoup4` or the package `beautifulsoup4` in some recent verions of debian / ubuntu
	* License: MIT license

* `argparse`  module

## License
		    DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
		            Version 2, December 2004

	 Copyright (C) 2013 Tom Wiesing <tkw01536@gmail.com>

	 Everyone is permitted to copy and distribute verbatim or modified
	 copies of this license document, and changing it is allowed as long
	 as the name is changed.

		    DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
	   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

	  0. You just DO WHAT THE FUCK YOU WANT TO.
