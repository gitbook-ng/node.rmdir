# rmdirr

Remove all files in the given path recursively.



## Description

Or just use `require( 'child_process' ).exec` and call `rm -r`

    var exec = require( 'child_process' ).exec,
        path = '/path/to/the/dir';

    exec( 'rm -r ' + path, function ( err, stdout, stderr ){
      // your callback goes here
    });


## Requires

    node >= 0.4.x



## Installation

    npm install rmdirr



## Usage

> Require the module before using

    var rmdir = require( 'rmdirr' );

### rmdirr( path, callback );

#### Arguments

> path

    type: String
    desc: The path to be clear.

> callback

    type: Function
    desc: The callback to be called after all files are removed.

#### Example

    var rmdir = require( 'rmdirr' ),
        path  = '/path/to/the/dir';

    rmdir( path, function (){
      console.log( 'all files removed' );
    });



## License

(The MIT License)

Copyright (c) 2011 dreamerslab &lt;ben@dreamerslab.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
