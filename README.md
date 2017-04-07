# api documentation for  [sql.js (v0.4.0)](http://github.com/kripken/sql.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-sql.js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sql.js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sql.js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sql.js)
#### SQLite library with support for opening and writing databases, prepared statements, and more. This SQLite library is in pure javascript (compiled with emscripten).

[![NPM](https://nodei.co/npm/sql.js.png?downloads=true)](https://www.npmjs.com/package/sql.js)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sql.js/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sql.js_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sql.js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sql.js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sql.js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/kripken/sql.js/issues",
        "email": "pere.jobs@gmail.com"
    },
    "contributors": [
        {
            "name": "Ophir LOJKINE",
            "email": "pere.jobs@gmail.com",
            "url": "https://github.com/lovasoa"
        },
        {
            "name": "@kripken"
        },
        {
            "name": "@hankinsoft"
        },
        {
            "name": "@firien"
        },
        {
            "name": "@dinedal"
        }
    ],
    "dependencies": {},
    "description": "SQLite library with support for opening and writing databases, prepared statements, and more. This SQLite library is in pure javascript (compiled with emscripten).",
    "devDependencies": {
        "test": ">=0.6",
        "workerjs": ">=0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "23be9635520eb0ff43a741e7e830397266e88445",
        "tarball": "https://registry.npmjs.org/sql.js/-/sql.js-0.4.0.tgz"
    },
    "gitHead": "8ae8ecb742d695570d97b64a3db28c2e662c866b",
    "homepage": "http://github.com/kripken/sql.js",
    "keywords": [
        "sql",
        "sqlite",
        "stand-alone",
        "relational",
        "database",
        "RDBMS",
        "data",
        "query",
        "statement",
        "emscripten",
        "asm",
        "asm.js"
    ],
    "license": "MIT",
    "main": "./js/sql.js",
    "maintainers": [
        {
            "name": "lovasoa",
            "email": "pere.jobs@gmail.com"
        }
    ],
    "name": "sql.js",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/kripken/sql.js.git"
    },
    "scripts": {
        "test": "node test/all.js"
    },
    "version": "0.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sql.js](#apidoc.module.sql.js)
1.  [function <span class="apidocSignatureSpan">sql.js.</span>Database (a)](#apidoc.element.sql.js.Database)
1.  [function <span class="apidocSignatureSpan">sql.js.</span>js.Database (a)](#apidoc.element.sql.js.js.Database)
1.  object <span class="apidocSignatureSpan">sql.js.</span>js.Database.prototype
1.  object <span class="apidocSignatureSpan">sql.js.</span>js.sql_debug
1.  object <span class="apidocSignatureSpan">sql.js.</span>js.sql_memory_growth
1.  object <span class="apidocSignatureSpan">sql.js.</span>js.worker_sql

#### [module sql.js.Database](#apidoc.module.sql.js.Database)
1.  [function <span class="apidocSignatureSpan">sql.js.</span>Database (a)](#apidoc.element.sql.js.Database.Database)

#### [module sql.js.Database.prototype](#apidoc.module.sql.js.Database.prototype)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>close ()](#apidoc.element.sql.js.Database.prototype.close)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>create_function (a, c)](#apidoc.element.sql.js.Database.prototype.create_function)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>each (a, c, d, e)](#apidoc.element.sql.js.Database.prototype.each)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>exec (a)](#apidoc.element.sql.js.Database.prototype.exec)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>export ()](#apidoc.element.sql.js.Database.prototype.export)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>getRowsModified ()](#apidoc.element.sql.js.Database.prototype.getRowsModified)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>handleError (a)](#apidoc.element.sql.js.Database.prototype.handleError)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>prepare (a, c)](#apidoc.element.sql.js.Database.prototype.prepare)
1.  [function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>run (a, c)](#apidoc.element.sql.js.Database.prototype.run)

#### [module sql.js.sql_debug](#apidoc.module.sql.js.sql_debug)
1.  [function <span class="apidocSignatureSpan">sql.js.sql_debug.</span>Database (data)](#apidoc.element.sql.js.sql_debug.Database)

#### [module sql.js.sql_memory_growth](#apidoc.module.sql.js.sql_memory_growth)
1.  [function <span class="apidocSignatureSpan">sql.js.sql_memory_growth.</span>Database (a)](#apidoc.element.sql.js.sql_memory_growth.Database)

#### [module sql.js.worker_sql](#apidoc.module.sql.js.worker_sql)
1.  [function <span class="apidocSignatureSpan">sql.js.worker_sql.</span>Database (a)](#apidoc.element.sql.js.worker_sql.Database)



# <a name="apidoc.module.sql.js"></a>[module sql.js](#apidoc.module.sql.js)

#### <a name="apidoc.element.sql.js.Database"></a>[function <span class="apidocSignatureSpan">sql.js.</span>Database (a)](#apidoc.element.sql.js.Database)
- description and source-code
```javascript
function a(a){this.filename="dbfile_"+(4294967295*Math.random()>>>0);null!=a&&Gc("/",this.filename,a,!0,!0);this.handleError(xe(
this.filename,Z));this.db=y(Z,"i32");be(this.db);this.ra={}}
```
- example usage
```shell
...
## Usage

'''javascript
var sql = require('sql.js');
// or sql = window.SQL if you are in a browser

// Create a database
var db = new sql.Database();
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
...
```

#### <a name="apidoc.element.sql.js.js.Database"></a>[function <span class="apidocSignatureSpan">sql.js.</span>js.Database (a)](#apidoc.element.sql.js.js.Database)
- description and source-code
```javascript
function a(a){this.filename="dbfile_"+(4294967295*Math.random()>>>0);null!=a&&Gc("/",this.filename,a,!0,!0);this.handleError(xe(
this.filename,Z));this.db=y(Z,"i32");be(this.db);this.ra={}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sql.js.Database"></a>[module sql.js.Database](#apidoc.module.sql.js.Database)

#### <a name="apidoc.element.sql.js.Database.Database"></a>[function <span class="apidocSignatureSpan">sql.js.</span>Database (a)](#apidoc.element.sql.js.Database.Database)
- description and source-code
```javascript
function a(a){this.filename="dbfile_"+(4294967295*Math.random()>>>0);null!=a&&Gc("/",this.filename,a,!0,!0);this.handleError(xe(
this.filename,Z));this.db=y(Z,"i32");be(this.db);this.ra={}}
```
- example usage
```shell
...
## Usage

'''javascript
var sql = require('sql.js');
// or sql = window.SQL if you are in a browser

// Create a database
var db = new sql.Database();
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
...
```



# <a name="apidoc.module.sql.js.Database.prototype"></a>[module sql.js.Database.prototype](#apidoc.module.sql.js.Database.prototype)

#### <a name="apidoc.element.sql.js.Database.prototype.close"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>close ()](#apidoc.element.sql.js.Database.prototype.close)
- description and source-code
```javascript
close = function (){var a,c,d;c=this.ra;for(a in c)d=c[a],d.free();this.handleError(le(this.db));qc("/"+this.filename);return this.db=null
}
```
- example usage
```shell
...
    console.log("FS.trackingDelegate['onOpenFile']('"+path+"', flags) threw an exception: " + e.message);
  }
  return stream;
},close:function (stream) {
  if (stream.getdents) stream.getdents = null; // free readdir state
  try {
    if (stream.stream_ops.close) {
      stream.stream_ops.close(stream);
    }
  } catch (e) {
    throw e;
  } finally {
    FS.closeStream(stream.fd);
  }
},llseek:function (stream, offset, whence) {
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.create_function"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>create_function (a, c)](#apidoc.element.sql.js.Database.prototype.create_function)
- description and source-code
```javascript
create_function = function (a, c){var d;d=l.La(function(a,
b,d){var m,t,r,x,v;t=[];for(m=r=0;0<=b?r<=b:r>=b;m=0<=b?++r:--r)x=y(d+4*m,"i32"),v=Ke(x),m=function(){switch(!1){case 1!==v:return
 Ie;case 2!==v:return He;case 3!==v:return Je;case 4!==v:return function(a){var b,c,d,e;e=Ge(a);b=Fe(a);a=new Uint8Array(e);for(
c=d=0;0<=e?d<e:d>e;c=0<=e?++d:--d)a[c]=u[b+c];return a};default:return function(){return null}}}(),m=m(x),t.push(m);if(b=c.apply
(null,t))switch(typeof b){case "number":return Be(a,b);case "string":return De(a,b,-1,-1)}else return Ce(a)});this.handleError(se
(this.db,
a,c.length,X.jb,0,d,0,0,0));return this}
```
- example usage
```shell
...
stmt.bind([0, 'hello']);
while (stmt.step()) console.log(stmt.get()); // Will print [0, 'hello']

// You can also use javascript functions inside your SQL code
// Create the js function you need
function add(a, b) {return a+b;}
// Specifies the SQL function's name, the number of it's arguments, and the js function to use
db.create_function("add_js", add);
// Run a query in which the function is used
db.run("INSERT INTO hello VALUES (add_js(7, 3), add_js('Hello ', 'world'));"); // Inserts 10 and 'Hello world'

// free the memory used by the statement
stmt.free();
// You can not use your statement anymore once it has been freed.
// But not freeing your statements causes memory leaks. You don't want that.
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.each"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>each (a, c, d, e)](#apidoc.element.sql.js.Database.prototype.each)
- description and source-code
```javascript
each = function (a, c, d, e){"function"===typeof c&&(e=d,d=c,c=void 0);for(a=this.prepare(a,c);a.step();)d(a.getAsObject());a.free();if("function
"===typeof e)return e()}
```
- example usage
```shell
...
to the query
@param callback [Function(Object)] A function that will be called on each row of result
@param done [Function] A function that will be called when all rows have been retrieved

@return [Database] The database object. Useful for method chaining

@example Read values from a table
    db.each("SELECT name,age FROM users WHERE age >= $majority",
                    {$majority:18},
                    function(row){console.log(row.name + " is a grown-up.")}
                );
 */

Database.prototype['each'] = function(sql, params, callback, done) {
  var stmt;
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.exec"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>exec (a)](#apidoc.element.sql.js.Database.prototype.exec)
- description and source-code
```javascript
exec = function (a){var c,d,e,g,h;if(!this.db)throw"Database closed";g=l.qa();d=l.R(a.length<<3);wa(a,d);a=l.R(4);for(e=
[];y(d,"i8")!==ae;)if(ya(Z,0,"i32"),ya(a,0,"i32"),this.handleError(ze(this.db,d,-1,Z,a)),c=y(Z,"i32"),d=y(a,"i32"),c!==ae){h=new
 ce(c,this);for(c=null;h.step();)null===c&&(c={columns:h.getColumnNames(),values:[]},e.push(c)),c.values.push(h.get());h.free()}
l.ga(g);return e}
```
- example usage
```shell
...

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
db.run(sqlstr); // Run the query without returning anything

var res = db.exec("SELECT * FROM hello");
/*
[
	{columns:['a','b'], values:[[0,'hello'],[1,'world']]}
]
*/

// Prepare an sql statement
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.export"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>export ()](#apidoc.element.sql.js.Database.prototype.export)
- description and source-code
```javascript
export = function (){var a,c,d,e;d=this.ra;for(a in d)e=d[a],e.free();this.handleError(le(this.db));e=this.filename;a=a={encoding:"binary
"};a.flags=a.flags||"r";a.encoding=a.encoding||"binary";if("utf8"!==a.encoding&&"binary"!==a.encoding)throw Error('Invalid encoding
 type "'+a.encoding+'"');d=wc(e,a.flags);e=rc(e).size;var g=new Uint8Array(e);
Ac(d,g,0,e,0);"utf8"===a.encoding?c=La(g,0):"binary"===a.encoding&&(c=g);yc(d);this.handleError(xe(this.filename,Z));this.db=y(Z
,"i32");return c}
```
- example usage
```shell
...

// free the memory used by the statement
stmt.free();
// You can not use your statement anymore once it has been freed.
// But not freeing your statements causes memory leaks. You don't want that.

// Export the database to an Uint8Array containing the SQLite database file
var binaryArray = db.export();
'''

## Demo
There is an online demo available here : http://kripken.github.io/sql.js/GUI

## Examples
The test files provide up to date example of the use of the api.
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.getRowsModified"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>getRowsModified ()](#apidoc.element.sql.js.Database.prototype.getRowsModified)
- description and source-code
```javascript
getRowsModified = function (){return je(this.db)}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sql.js.Database.prototype.handleError"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>handleError (a)](#apidoc.element.sql.js.Database.prototype.handleError)
- description and source-code
```javascript
handleError = function (a){if(a===X.ka)return null;a=ue(this.db);throw Error(a);}
```
- example usage
```shell
...
  this.pos = 1;
  switch (ret = sqlite3_step(this.stmt)) {
    case SQLite.ROW:
      return true;
    case SQLite.DONE:
      return false;
    default:
      return this.db.handleError(ret);
  }
};

Statement.prototype.getNumber = function(pos) {
  if (pos == null) {
    pos = this.pos++;
  }
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.prepare"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>prepare (a, c)](#apidoc.element.sql.js.Database.prototype.prepare)
- description and source-code
```javascript
prepare = function (a, c){var d,e;ya(Z,0,"i32");
this.handleError(ye(this.db,a,-1,Z,ae));d=y(Z,"i32");if(d===ae)throw"Nothing to prepare";e=new ce(d,this);null!=c&&e.bind(c);return
 this.ra[d]=e}
```
- example usage
```shell
...
/*
[
	{columns:['a','b'], values:[[0,'hello'],[1,'world']]}
]
*/

// Prepare an sql statement
var stmt = db.prepare("SELECT * FROM hello WHERE a=:aval AND b=:bval");

// Bind values to the parameters and fetch the results of the query
var result = stmt.getAsObject({':aval' : 1, ':bval' : 'world'});
console.log(result); // Will print {a:1, b:'world'}

// Bind other values
stmt.bind([0, 'hello']);
...
```

#### <a name="apidoc.element.sql.js.Database.prototype.run"></a>[function <span class="apidocSignatureSpan">sql.js.Database.prototype.</span>run (a, c)](#apidoc.element.sql.js.Database.prototype.run)
- description and source-code
```javascript
run = function (a, c){var d;if(!this.db)throw"Database closed";c?(d=this.prepare(a,c),d.step(),d.free()):this.handleError(ve(this.db,a,
0,0,Z));return this}
```
- example usage
```shell
...
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
db.run(sqlstr); // Run the query without returning anything

var res = db.exec("SELECT * FROM hello");
/*
[
	{columns:['a','b'], values:[[0,'hello'],[1,'world']]}
]
*/
...
```



# <a name="apidoc.module.sql.js.sql_debug"></a>[module sql.js.sql_debug](#apidoc.module.sql.js.sql_debug)

#### <a name="apidoc.element.sql.js.sql_debug.Database"></a>[function <span class="apidocSignatureSpan">sql.js.sql_debug.</span>Database (data)](#apidoc.element.sql.js.sql_debug.Database)
- description and source-code
```javascript
function Database(data) {
  this.filename = 'dbfile_' + (0xffffffff * Math.random() >>> 0);
  if (data != null) {
    FS.createDataFile('/', this.filename, data, true, true);
  }
  this.handleError(sqlite3_open(this.filename, apiTemp));
  this.db = getValue(apiTemp, 'i32');
  RegisterExtensionFunctions(this.db);
  this.statements = {};
}
```
- example usage
```shell
...
## Usage

'''javascript
var sql = require('sql.js');
// or sql = window.SQL if you are in a browser

// Create a database
var db = new sql.Database();
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
...
```



# <a name="apidoc.module.sql.js.sql_memory_growth"></a>[module sql.js.sql_memory_growth](#apidoc.module.sql.js.sql_memory_growth)

#### <a name="apidoc.element.sql.js.sql_memory_growth.Database"></a>[function <span class="apidocSignatureSpan">sql.js.sql_memory_growth.</span>Database (a)](#apidoc.element.sql.js.sql_memory_growth.Database)
- description and source-code
```javascript
function a(a){this.filename="dbfile_"+(4294967295*Math.random()>>>0);null!=a&&Kc("/",this.filename,a,!0,!0);this.handleError(Be(
this.filename,Z));this.db=Ha(Z,"i32");fe(this.db);this.ra={}}
```
- example usage
```shell
...
## Usage

'''javascript
var sql = require('sql.js');
// or sql = window.SQL if you are in a browser

// Create a database
var db = new sql.Database();
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
...
```



# <a name="apidoc.module.sql.js.worker_sql"></a>[module sql.js.worker_sql](#apidoc.module.sql.js.worker_sql)

#### <a name="apidoc.element.sql.js.worker_sql.Database"></a>[function <span class="apidocSignatureSpan">sql.js.worker_sql.</span>Database (a)](#apidoc.element.sql.js.worker_sql.Database)
- description and source-code
```javascript
function a(a){this.filename="dbfile_"+(4294967295*Math.random()>>>0);null!=a&&Gc("/",this.filename,a,!0,!0);this.handleError(xe(
this.filename,Z));this.db=y(Z,"i32");be(this.db);this.ra={}}
```
- example usage
```shell
...
## Usage

'''javascript
var sql = require('sql.js');
// or sql = window.SQL if you are in a browser

// Create a database
var db = new sql.Database();
// NOTE: You can also use new sql.Database(data) where
// data is an Uint8Array representing an SQLite database file

// Execute some sql
sqlstr = "CREATE TABLE hello (a int, b char);";
sqlstr += "INSERT INTO hello VALUES (0, 'hello');"
sqlstr += "INSERT INTO hello VALUES (1, 'world');"
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
