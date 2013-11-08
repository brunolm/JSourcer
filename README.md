JSourcer
========

Bundle and minify Javascript files in a folder navigating through references.


Syntax
------------

    <Debug|Release> SourcePath-1 OutputPath-1 [SourcePath-N OutputPath-N]
    
Debug just bundle files.
Release bundle and minify.


Example
-------

Folder structure example
- Input
  - 000-test.js
  - 001-test.js
  - 002-test.js
- Output

Call

    JSourcer Debug "Example\Input\\" "Example\Output\all.js"
    
Result
- Output
  - all.js
  
To add references, put at the top of the file

    /// <reference path="path.js" />
