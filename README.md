# api documentation for  [gulp-coverage (v0.3.38)](https://github.com/dylanb/gulp-coverage)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-coverage.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-coverage) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-coverage.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-coverage)
#### Instrument and generate code coverage independent of test runner

[![NPM](https://nodei.co/npm/gulp-coverage.png?downloads=true)](https://www.npmjs.com/package/gulp-coverage)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-coverage/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-coverage_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-coverage/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-coverage/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-coverage/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "dylan@barrell.com"
    },
    "bugs": {
        "url": "https://github.com/dylanb/gulp-coverage/issues"
    },
    "dependencies": {
        "extend": "~1.2.1",
        "gulp-util": "~2.2.13",
        "instrumentjs": "0.0.2",
        "jade": "~1.1.4",
        "multimatch": "~0.1.0",
        "through2": "~0.4.0",
        "underscore": "~1.5.2"
    },
    "description": "Instrument and generate code coverage independent of test runner",
    "devDependencies": {
        "gulp": "~3.4.0",
        "gulp-coveralls": "^0.1.2",
        "gulp-jasmine": "~0.1.3",
        "gulp-jshint": "~1.3.4",
        "gulp-mocha": "~0.4.1",
        "rewire": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "86a3e73ac9993df376600538b82519cd35047847",
        "tarball": "https://registry.npmjs.org/gulp-coverage/-/gulp-coverage-0.3.38.tgz"
    },
    "gitHead": "5af703edd3a69e7c463e1726e3a388c094fb4ada",
    "homepage": "https://github.com/dylanb/gulp-coverage",
    "keywords": [
        "coverage",
        "code coverage",
        "mocha",
        "jasmine",
        "gulpplugin"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "dylanb",
            "email": "dylan@barrell.com"
        }
    ],
    "name": "gulp-coverage",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dylanb/gulp-coverage.git"
    },
    "scripts": {
        "test": "gulp test"
    },
    "version": "0.3.38"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-coverage](#apidoc.module.gulp-coverage)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>chainable ()](#apidoc.element.gulp-coverage.chainable)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>enforce (options)](#apidoc.element.gulp-coverage.enforce)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>format (options)](#apidoc.element.gulp-coverage.format)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>gather ()](#apidoc.element.gulp-coverage.gather)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>instrument (options)](#apidoc.element.gulp-coverage.instrument)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>report (options)](#apidoc.element.gulp-coverage.report)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>test3 ()](#apidoc.element.gulp-coverage.test3)
1.  object <span class="apidocSignatureSpan">gulp-coverage.</span>chainable.prototype
1.  object <span class="apidocSignatureSpan">gulp-coverage.</span>cover
1.  object <span class="apidocSignatureSpan">gulp-coverage.</span>coverage_store
1.  object <span class="apidocSignatureSpan">gulp-coverage.</span>myModule
1.  object <span class="apidocSignatureSpan">gulp-coverage.</span>test3.prototype

#### [module gulp-coverage.chainable](#apidoc.module.gulp-coverage.chainable)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>chainable ()](#apidoc.element.gulp-coverage.chainable.chainable)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.chainable.</span>super_ ()](#apidoc.element.gulp-coverage.chainable.super_)

#### [module gulp-coverage.chainable.prototype](#apidoc.module.gulp-coverage.chainable.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>find (qTerm)](#apidoc.element.gulp-coverage.chainable.prototype.find)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>format (options)](#apidoc.element.gulp-coverage.chainable.prototype.format)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>remove (index, number)](#apidoc.element.gulp-coverage.chainable.prototype.remove)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>write ()](#apidoc.element.gulp-coverage.chainable.prototype.write)

#### [module gulp-coverage.cover](#apidoc.module.gulp-coverage.cover)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>cover (pattern, debugDirectory)](#apidoc.element.gulp-coverage.cover.cover)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.cover.</span>cleanup ()](#apidoc.element.gulp-coverage.cover.cleanup)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.cover.</span>init ()](#apidoc.element.gulp-coverage.cover.init)
1.  object <span class="apidocSignatureSpan">gulp-coverage.cover.</span>reporters

#### [module gulp-coverage.coverage_store](#apidoc.module.gulp-coverage.coverage_store)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>clearStore ()](#apidoc.element.gulp-coverage.coverage_store.clearStore)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>getStore (filename)](#apidoc.element.gulp-coverage.coverage_store.getStore)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>getStoreData (filename)](#apidoc.element.gulp-coverage.coverage_store.getStoreData)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>register (filename)](#apidoc.element.gulp-coverage.coverage_store.register)

#### [module gulp-coverage.myModule](#apidoc.module.gulp-coverage.myModule)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.myModule.</span>myFunction ()](#apidoc.element.gulp-coverage.myModule.myFunction)

#### [module gulp-coverage.test3](#apidoc.module.gulp-coverage.test3)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.</span>test3 ()](#apidoc.element.gulp-coverage.test3.test3)

#### [module gulp-coverage.test3.prototype](#apidoc.module.gulp-coverage.test3.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.test3.prototype.</span>hide ()](#apidoc.element.gulp-coverage.test3.prototype.hide)
1.  [function <span class="apidocSignatureSpan">gulp-coverage.test3.prototype.</span>show ()](#apidoc.element.gulp-coverage.test3.prototype.show)



# <a name="apidoc.module.gulp-coverage"></a>[module gulp-coverage](#apidoc.module.gulp-coverage)

#### <a name="apidoc.element.gulp-coverage.chainable"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>chainable ()](#apidoc.element.gulp-coverage.chainable)
- description and source-code
```javascript
chainable = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.enforce"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>enforce (options)](#apidoc.element.gulp-coverage.enforce)
- description and source-code
```javascript
enforce = function (options) {
    options = options || {};
    var statements = options.statements || 100,
        blocks = options.blocks || 100,
        lines = options.lines || 100,
        uncovered = options.uncovered;
    return through2.obj(
        function (data, encoding, cb) {
            if (!data.coverage) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'Must call gather or report before calling enforce'));
                return cb();
            }
            if (data.coverage.statements < statements) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'statement coverage of ' + data.coverage.statements +
                    ' does not meet the threshold of ' + statements));
            }
            if (data.coverage.coverage < lines) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'line coverage of ' + data.coverage.coverage +
                    ' does not meet the threshold of ' + lines));
            }
            if (data.coverage.blocks < blocks) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'block coverage of ' + data.coverage.blocks +
                    ' does not meet the threshold of ' + blocks));
            }
            if (data.coverage.uncovered && uncovered !== undefined && data.coverage.uncovered.length > uncovered) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'uncovered files of ' + data.coverage.uncovered.length +
                    ' does not meet the threshold of ' + uncovered));
            }
            cb();
        }, function (cb) {
            cb();
        });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.format"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>format (options)](#apidoc.element.gulp-coverage.format)
- description and source-code
```javascript
format = function (options) {
    var reporters = options || [{}];
    if (!Array.isArray(reporters)) reporters = [reporters];
    return through2.obj(
        function (data, encoding, cb) {
            var file;
            if (!data.coverage) {
                this.emit('error', new gutil.PluginError('gulp-coverage',
                    'Must call gather before calling enforce'));
                cb();
                return;
            }
            reporters.forEach(function(opts) {
                if (typeof opts === 'string') opts = { reporter: opts };
                var reporter = opts.reporter || 'html';
                var outfile = opts.outFile || 'coverage.' + reporter;
                file = new gutil.File({
                    base: path.join(__dirname, './'),
                    cwd: __dirname,
                    path: path.join(__dirname, './', outfile),
                    contents: new Buffer(cover.reporters[reporter](data.coverage))
                });
                file.coverage = data.coverage;
                this.push(file);
            }, this);
            cb();
        }, function (cb) {
            cb();
        });
}
```
- example usage
```shell
...
        return gulp.src(['src.js', 'src2.js'], { read: false })
                .pipe(cover.instrument({
                    pattern: ['**/test*'],
                    debugDirectory: 'debug'
                }))
                .pipe(mocha())
                .pipe(cover.gather())
                .pipe(cover.format())
                .pipe(gulp.dest('reports'));
    });
'''

To instrument and report using Jasmine as your test system:

'''js
...
```

#### <a name="apidoc.element.gulp-coverage.gather"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>gather ()](#apidoc.element.gulp-coverage.gather)
- description and source-code
```javascript
gather = function () {
    return through2.obj(
        function (file, encoding, cb) {
            if (!file.path) {
                this.emit('error', new gutil.PluginError('gulp-coverage', 'Streaming not supported'));
                return cb();
            }
            cb();
        }, function (cb) {
            var stats;

            if (!coverInst) {
                throw new Error('Must call instrument before calling report');
            }
            stats = coverInst.allStats();
            this.push({ coverage: stats });
            cb();
        });
}
```
- example usage
```shell
...
    gulp.task('test', function () {
        return gulp.src(['src.js', 'src2.js'], { read: false })
                .pipe(cover.instrument({
                    pattern: ['**/test*'],
                    debugDirectory: 'debug'
                }))
                .pipe(mocha())
                .pipe(cover.gather())
                .pipe(cover.format())
                .pipe(gulp.dest('reports'));
    });
'''

To instrument and report using Jasmine as your test system:
...
```

#### <a name="apidoc.element.gulp-coverage.instrument"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>instrument (options)](#apidoc.element.gulp-coverage.instrument)
- description and source-code
```javascript
instrument = function (options) {
    options = options || {};
    cover.cleanup();
    cover.init();
    if (coverInst) {
        coverInst.release();
    }
    coverInst = cover.cover(options.pattern, options.debugDirectory);

    return through2.obj(function (file, encoding, cb) {
        if (!file.path) {
            this.emit('error', new gutil.PluginError('gulp-coverage', 'Streaming not supported'));
            return cb();
        }

        this.push(file);
        cb();
    },
    function (cb) {
        cb();
    });
}
```
- example usage
```shell
...

'''js
mocha = require('gulp-mocha');
cover = require('gulp-coverage');

gulp.task('test', function () {
    return gulp.src(['src.js', 'src2.js'], { read: false })
            .pipe(cover.instrument({
                pattern: ['**/test*'],
                debugDirectory: 'debug'
            }))
            .pipe(mocha())
            .pipe(cover.gather())
            .pipe(cover.format())
            .pipe(gulp.dest('reports'));
...
```

#### <a name="apidoc.element.gulp-coverage.report"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>report (options)](#apidoc.element.gulp-coverage.report)
- description and source-code
```javascript
report = function (options) {
    options = options || {};
    var reporter = options.reporter || 'html';

    return through2.obj(
        function (file, encoding, cb) {
            if (!file.path) {
                this.emit('error', new gutil.PluginError('gulp-coverage', 'Streaming not supported'));
                return cb();
            }
            cb();
        }, function (cb) {
            var stats;

            if (!coverInst) {
                throw new Error('Must call instrument before calling report');
            }
            stats = coverInst.allStats();
            cover.reporters[reporter](stats, options.outFile ? options.outFile : undefined);
            this.push({ coverage: stats });
            cb();
        });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.test3"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>test3 ()](#apidoc.element.gulp-coverage.test3)
- description and source-code
```javascript
test3 = function () {
    this.count = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-coverage.chainable"></a>[module gulp-coverage.chainable](#apidoc.module.gulp-coverage.chainable)

#### <a name="apidoc.element.gulp-coverage.chainable.chainable"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>chainable ()](#apidoc.element.gulp-coverage.chainable.chainable)
- description and source-code
```javascript
chainable = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.chainable.super_"></a>[function <span class="apidocSignatureSpan">gulp-coverage.chainable.</span>super_ ()](#apidoc.element.gulp-coverage.chainable.super_)
- description and source-code
```javascript
function Array() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-coverage.chainable.prototype"></a>[module gulp-coverage.chainable.prototype](#apidoc.module.gulp-coverage.chainable.prototype)

#### <a name="apidoc.element.gulp-coverage.chainable.prototype.find"></a>[function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>find (qTerm)](#apidoc.element.gulp-coverage.chainable.prototype.find)
- description and source-code
```javascript
find = function (qTerm) {
    var q = qTerm.toLowerCase();
    dataBase.forEach(function(item) {
        if (item.indexOf(q) !== -1) {
            this.push(item);
        }
    }, this);
    return this;
}
```
- example usage
```shell
...

// Chanable function
f.func = function () {return this};
f.func().func();

// Chainable object
chain = new Chainable();
chain.find('zack').format({middle: false}).remove(0, 1).write();

// non-object method call (looks like a chainable from a syntax tree perspective)
str = str.substr(0, 2);

Math.floor(
    Math.random()*
    10+
...
```

#### <a name="apidoc.element.gulp-coverage.chainable.prototype.format"></a>[function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>format (options)](#apidoc.element.gulp-coverage.chainable.prototype.format)
- description and source-code
```javascript
format = function (options) {
    var defaultOptions = {
        first: true,
        last: true,
        middle : true
    };
    extend(defaultOptions, options);
    this.forEach(function(item, index) {
        var arr = item.trim().split(' '),
            i;
        if (defaultOptions.middle && arr.length > 2) {
            for (i = 1; i < arr.length - 1; i++) {
                arr[i] = arr[i][0].toUpperCase() + arr[i].substring(1);
            }
        }
        if (defaultOptions.first) {
            arr[0] = arr[0][0].toUpperCase() + arr[0].substring(1);
        }
        if (defaultOptions.last) {
            arr[arr.length - 1] = arr[arr.length - 1][0].toUpperCase() + arr[arr.length - 1].substring(1);
        }
        this[index] = arr.join(' ');
    }, this);
    return this;
}
```
- example usage
```shell
...
        return gulp.src(['src.js', 'src2.js'], { read: false })
                .pipe(cover.instrument({
                    pattern: ['**/test*'],
                    debugDirectory: 'debug'
                }))
                .pipe(mocha())
                .pipe(cover.gather())
                .pipe(cover.format())
                .pipe(gulp.dest('reports'));
    });
'''

To instrument and report using Jasmine as your test system:

'''js
...
```

#### <a name="apidoc.element.gulp-coverage.chainable.prototype.remove"></a>[function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>remove (index, number)](#apidoc.element.gulp-coverage.chainable.prototype.remove)
- description and source-code
```javascript
remove = function (index, number) {
    if (index !== -1) {
        this.splice(index, number !== undefined ? number : 1);
    }
    return this;
}
```
- example usage
```shell
...

// Chanable function
f.func = function () {return this};
f.func().func();

// Chainable object
chain = new Chainable();
chain.find('zack').format({middle: false}).remove(0, 1).write();

// non-object method call (looks like a chainable from a syntax tree perspective)
str = str.substr(0, 2);

Math.floor(
    Math.random()*
    10+
...
```

#### <a name="apidoc.element.gulp-coverage.chainable.prototype.write"></a>[function <span class="apidocSignatureSpan">gulp-coverage.chainable.prototype.</span>write ()](#apidoc.element.gulp-coverage.chainable.prototype.write)
- description and source-code
```javascript
write = function () {
    // noop
    return this;
}
```
- example usage
```shell
...

// Chanable function
f.func = function () {return this};
f.func().func();

// Chainable object
chain = new Chainable();
chain.find('zack').format({middle: false}).remove(0, 1).write();

// non-object method call (looks like a chainable from a syntax tree perspective)
str = str.substr(0, 2);

Math.floor(
    Math.random()*
    10+
...
```



# <a name="apidoc.module.gulp-coverage.cover"></a>[module gulp-coverage.cover](#apidoc.module.gulp-coverage.cover)

#### <a name="apidoc.element.gulp-coverage.cover.cover"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>cover (pattern, debugDirectory)](#apidoc.element.gulp-coverage.cover.cover)
- description and source-code
```javascript
cover = function (pattern, debugDirectory) {
    return new CoverageSession(pattern, debugDirectory);
}
```
- example usage
```shell
...
module.exports.instrument = function (options) {
options = options || {};
cover.cleanup();
cover.init();
if (coverInst) {
    coverInst.release();
}
coverInst = cover.cover(options.pattern, options.debugDirectory);

return through2.obj(function (file, encoding, cb) {
    if (!file.path) {
        this.emit('error', new gutil.PluginError('gulp-coverage', 'Streaming not supported'));
        return cb();
    }
...
```

#### <a name="apidoc.element.gulp-coverage.cover.cleanup"></a>[function <span class="apidocSignatureSpan">gulp-coverage.cover.</span>cleanup ()](#apidoc.element.gulp-coverage.cover.cleanup)
- description and source-code
```javascript
cleanup = function () {
    var store = require('./coverage_store');

    store.clearStore();
}
```
- example usage
```shell
...
var cover = require('./contrib/cover');
var through2 = require('through2');
var gutil = require('gulp-util');
var coverInst;

module.exports.instrument = function (options) {
options = options || {};
cover.cleanup();
cover.init();
if (coverInst) {
    coverInst.release();
}
coverInst = cover.cover(options.pattern, options.debugDirectory);

return through2.obj(function (file, encoding, cb) {
...
```

#### <a name="apidoc.element.gulp-coverage.cover.init"></a>[function <span class="apidocSignatureSpan">gulp-coverage.cover.</span>init ()](#apidoc.element.gulp-coverage.cover.init)
- description and source-code
```javascript
init = function () {
    var directoryName = '.cover_' + Math.random().toString().substring(2),
        dataDir = path.join(process.cwd(), '.coverdata');
    if (!fs.existsSync(dataDir)) {
        fs.mkdirSync(dataDir);
    } else {
        fs.readdirSync(dataDir).forEach(function(name) {
            if (name !== '.' && name !== '..') {
                removeDir(path.join(dataDir, name));
            }
        });
    }
    fs.mkdirSync(path.join(dataDir, directoryName));
    fd = fs.writeFileSync(path.join(process.cwd(), '.coverrun'), '{ "run" : "' + directoryName + '" }');
}
```
- example usage
```shell
...
var through2 = require('through2');
var gutil = require('gulp-util');
var coverInst;

module.exports.instrument = function (options) {
options = options || {};
cover.cleanup();
cover.init();
if (coverInst) {
    coverInst.release();
}
coverInst = cover.cover(options.pattern, options.debugDirectory);

return through2.obj(function (file, encoding, cb) {
    if (!file.path) {
...
```



# <a name="apidoc.module.gulp-coverage.coverage_store"></a>[module gulp-coverage.coverage_store](#apidoc.module.gulp-coverage.coverage_store)

#### <a name="apidoc.element.gulp-coverage.coverage_store.clearStore"></a>[function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>clearStore ()](#apidoc.element.gulp-coverage.coverage_store.clearStore)
- description and source-code
```javascript
clearStore = function () {
    var filename;
    for (filename in coverageStore) {
        if (coverageStore.hasOwnProperty(filename)) {
            fs.closeSync(coverageStore[filename]);
            coverageStore[filename] = undefined;
            delete coverageStore[filename];
        }
    }
}
```
- example usage
```shell
...
fs.mkdirSync(path.join(dataDir, directoryName));
fd = fs.writeFileSync(path.join(process.cwd(), '.coverrun'), '{ "run" : "' + directoryName + '" }');
};

var cleanup = function() {
var store = require('./coverage_store');

store.clearStore();
};

module.exports = {
cover: cover,
init: init,
cleanup: cleanup,
reporters: {
...
```

#### <a name="apidoc.element.gulp-coverage.coverage_store.getStore"></a>[function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>getStore (filename)](#apidoc.element.gulp-coverage.coverage_store.getStore)
- description and source-code
```javascript
getStore = function (filename) {
    var run = JSON.parse(fs.readFileSync(process.cwd() + '/.coverrun')).run,
        runDirectory = process.cwd() + '/.coverdata/' + run + '/';

    filename = filename.replace(/[\/|\:|\\]/g, "_");
    if (!coverageStore[filename]) {
        coverageStore[filename] = fs.openSync(runDirectory + filename, 'a');
    }
    return coverageStore[filename];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.coverage_store.getStoreData"></a>[function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>getStoreData (filename)](#apidoc.element.gulp-coverage.coverage_store.getStoreData)
- description and source-code
```javascript
getStoreData = function (filename) {
    var run = JSON.parse(fs.readFileSync(process.cwd() + '/.coverrun')).run,
        runDirectory = process.cwd() + '/.coverdata/' + run + '/';

    filename = filename.replace(/[\/|\:|\\]/g, "_");
    return fs.readFileSync(runDirectory + filename);
}
```
- example usage
```shell
...
 *
 * @private
 * @method _prepare
 * @return {undefined}
 */
FileCoverageData.prototype._prepare = function() {
// console.log('PREPARE');
var data = require('./coverage_store').getStoreData(this.filename),
    rawData, store, index;

data = '[' + data  + '{}]';
// console.log('DATA: ', data);
rawData = JSON.parse(data);
store = {nodes: {}, blocks: {}};
rawData.forEach(function(item) {
...
```

#### <a name="apidoc.element.gulp-coverage.coverage_store.register"></a>[function <span class="apidocSignatureSpan">gulp-coverage.coverage_store.</span>register (filename)](#apidoc.element.gulp-coverage.coverage_store.register)
- description and source-code
```javascript
register = function (filename) {
    var run = JSON.parse(fs.readFileSync(process.cwd() + '/.coverrun')).run,
        runDirectory = process.cwd() + '/.coverdata/' + run + '/';

    filename = filename.replace(/[\/|\:|\\]/g, "_");
    if (!coverageStore[filename] || !fs.existsSync(runDirectory + filename)) {
        if (coverageStore.hasOwnProperty(filename)) {
            fs.closeSync(coverageStore[filename]);
            coverageStore[filename] = undefined;
            delete coverageStore[filename];
        }
        coverageStore[filename] = fs.openSync(runDirectory + filename, 'w');
    }
    return coverageStore[filename];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-coverage.myModule"></a>[module gulp-coverage.myModule](#apidoc.module.gulp-coverage.myModule)

#### <a name="apidoc.element.gulp-coverage.myModule.myFunction"></a>[function <span class="apidocSignatureSpan">gulp-coverage.myModule.</span>myFunction ()](#apidoc.element.gulp-coverage.myModule.myFunction)
- description and source-code
```javascript
myFunction = function () {
    myLocalGlobal();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-coverage.test3"></a>[module gulp-coverage.test3](#apidoc.module.gulp-coverage.test3)

#### <a name="apidoc.element.gulp-coverage.test3.test3"></a>[function <span class="apidocSignatureSpan">gulp-coverage.</span>test3 ()](#apidoc.element.gulp-coverage.test3.test3)
- description and source-code
```javascript
test3 = function () {
    this.count = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-coverage.test3.prototype"></a>[module gulp-coverage.test3.prototype](#apidoc.module.gulp-coverage.test3.prototype)

#### <a name="apidoc.element.gulp-coverage.test3.prototype.hide"></a>[function <span class="apidocSignatureSpan">gulp-coverage.test3.prototype.</span>hide ()](#apidoc.element.gulp-coverage.test3.prototype.hide)
- description and source-code
```javascript
hide = function () {
    this.count--;
    return this.count;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-coverage.test3.prototype.show"></a>[function <span class="apidocSignatureSpan">gulp-coverage.test3.prototype.</span>show ()](#apidoc.element.gulp-coverage.test3.prototype.show)
- description and source-code
```javascript
show = function () {
    this.count++;
    return this.count;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
