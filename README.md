# api documentation for  [express-handlebars (v3.0.0)](https://github.com/ericf/express-handlebars)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-handlebars.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-handlebars) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-handlebars.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-handlebars)
#### A Handlebars view engine for Express which doesn't suck.

[![NPM](https://nodei.co/npm/express-handlebars.png?downloads=true)](https://www.npmjs.com/package/express-handlebars)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-handlebars/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-express-handlebars%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-handlebars/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-express-handlebars/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-express-handlebars/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Eric Ferraiuolo",
        "email": "eferraiuolo@gmail.com",
        "url": "http://ericf.me/"
    },
    "bugs": {
        "url": "https://github.com/ericf/express-handlebars/issues"
    },
    "dependencies": {
        "glob": "^6.0.4",
        "graceful-fs": "^4.1.2",
        "handlebars": "^4.0.5",
        "object.assign": "^4.0.3",
        "promise": "^7.0.0"
    },
    "description": "A Handlebars view engine for Express which doesn't suck.",
    "devDependencies": {},
    "directories": {
        "example": "examples"
    },
    "dist": {
        "shasum": "80a070bb819b09e4af2ca6d0780f75ce05e75c2f",
        "tarball": "https://registry.npmjs.org/express-handlebars/-/express-handlebars-3.0.0.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "gitHead": "a7076983c39916a6525c244a8e3a39638759a318",
    "homepage": "https://github.com/ericf/express-handlebars",
    "keywords": [
        "express",
        "express3",
        "handlebars",
        "view",
        "layout",
        "partials",
        "templates"
    ],
    "license": "BSD-3-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "ericf",
            "email": "eferraiuolo@gmail.com"
        },
        {
            "name": "sahat",
            "email": "sakhat@gmail.com"
        }
    ],
    "name": "express-handlebars",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ericf/express-handlebars.git"
    },
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "3.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module express-handlebars](#apidoc.module.express-handlebars)
1.  [function <span class="apidocSignatureSpan">express-handlebars.</span>ExpressHandlebars (config)](#apidoc.element.express-handlebars.ExpressHandlebars)
1.  [function <span class="apidocSignatureSpan">express-handlebars.</span>create (config)](#apidoc.element.express-handlebars.create)
1.  object <span class="apidocSignatureSpan">express-handlebars.</span>ExpressHandlebars.prototype
1.  object <span class="apidocSignatureSpan">express-handlebars.</span>utils

#### [module express-handlebars.ExpressHandlebars](#apidoc.module.express-handlebars.ExpressHandlebars)
1.  [function <span class="apidocSignatureSpan">express-handlebars.</span>ExpressHandlebars (config)](#apidoc.element.express-handlebars.ExpressHandlebars.ExpressHandlebars)

#### [module express-handlebars.ExpressHandlebars.prototype](#apidoc.module.express-handlebars.ExpressHandlebars.prototype)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_compileTemplate (template, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._compileTemplate)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getDir (dirPath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getDir)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getFile (filePath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getFile)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getTemplateName (filePath, namespace)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getTemplateName)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_precompileTemplate (template, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._precompileTemplate)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_renderTemplate (template, context, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._renderTemplate)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_resolveLayoutPath (layoutPath)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._resolveLayoutPath)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getPartials (options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getPartials)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getTemplate (filePath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplate)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getTemplates (dirPath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplates)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>render (filePath, context, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.render)
1.  [function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>renderView (viewPath, options, callback)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.renderView)

#### [module express-handlebars.utils](#apidoc.module.express-handlebars.utils)
1.  [function <span class="apidocSignatureSpan">express-handlebars.utils.</span>assign ()](#apidoc.element.express-handlebars.utils.assign)
1.  [function <span class="apidocSignatureSpan">express-handlebars.utils.</span>passError (callback)](#apidoc.element.express-handlebars.utils.passError)
1.  [function <span class="apidocSignatureSpan">express-handlebars.utils.</span>passValue (callback)](#apidoc.element.express-handlebars.utils.passValue)



# <a name="apidoc.module.express-handlebars"></a>[module express-handlebars](#apidoc.module.express-handlebars)

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars"></a>[function <span class="apidocSignatureSpan">express-handlebars.</span>ExpressHandlebars (config)](#apidoc.element.express-handlebars.ExpressHandlebars)
- description and source-code
```javascript
function ExpressHandlebars(config) {
    // Config properties with defaults.
    utils.assign(this, {
        handlebars     : Handlebars,
        extname        : '.handlebars',
        layoutsDir     : 'views/layouts/',
        partialsDir    : 'views/partials/',
        defaultLayout  : undefined,
        helpers        : undefined,
        compilerOptions: undefined,
    }, config);

    // Express view engine integration point.
    this.engine = this.renderView.bind(this);

    // Normalize 'extname'.
    if (this.extname.charAt(0) !== '.') {
        this.extname = '.' + this.extname;
    }

    // Internal caches of compiled and precompiled templates.
    this.compiled    = Object.create(null);
    this.precompiled = Object.create(null);

    // Private internal file system cache.
    this._fsCache = Object.create(null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.create"></a>[function <span class="apidocSignatureSpan">express-handlebars.</span>create (config)](#apidoc.element.express-handlebars.create)
- description and source-code
```javascript
function create(config) {
    return new ExpressHandlebars(config);
}
```
- example usage
```shell
...
Another way to use this view engine is to create an instance(s) of 'ExpressHandlebars', allowing access to the full API:

'''javascript
var express = require('express');
var exphbs  = require('express-handlebars');

var app = express();
var hbs = exphbs.create({ /* config */ });

// Register 'hbs.engine' with the Express app.
app.engine('handlebars', hbs.engine);
app.set('view engine', 'handlebars');

// ...still have a reference to 'hbs', on which methods like 'loadPartials()'
// can be called.
...
```



# <a name="apidoc.module.express-handlebars.ExpressHandlebars"></a>[module express-handlebars.ExpressHandlebars](#apidoc.module.express-handlebars.ExpressHandlebars)

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.ExpressHandlebars"></a>[function <span class="apidocSignatureSpan">express-handlebars.</span>ExpressHandlebars (config)](#apidoc.element.express-handlebars.ExpressHandlebars.ExpressHandlebars)
- description and source-code
```javascript
function ExpressHandlebars(config) {
    // Config properties with defaults.
    utils.assign(this, {
        handlebars     : Handlebars,
        extname        : '.handlebars',
        layoutsDir     : 'views/layouts/',
        partialsDir    : 'views/partials/',
        defaultLayout  : undefined,
        helpers        : undefined,
        compilerOptions: undefined,
    }, config);

    // Express view engine integration point.
    this.engine = this.renderView.bind(this);

    // Normalize 'extname'.
    if (this.extname.charAt(0) !== '.') {
        this.extname = '.' + this.extname;
    }

    // Internal caches of compiled and precompiled templates.
    this.compiled    = Object.create(null);
    this.precompiled = Object.create(null);

    // Private internal file system cache.
    this._fsCache = Object.create(null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-handlebars.ExpressHandlebars.prototype"></a>[module express-handlebars.ExpressHandlebars.prototype](#apidoc.module.express-handlebars.ExpressHandlebars.prototype)

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._compileTemplate"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_compileTemplate (template, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._compileTemplate)
- description and source-code
```javascript
_compileTemplate = function (template, options) {
    return this.handlebars.compile(template, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._getDir"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getDir (dirPath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getDir)
- description and source-code
```javascript
_getDir = function (dirPath, options) {
    dirPath = path.resolve(dirPath);
    options || (options = {});

    var cache = this._fsCache;
    var dir   = options.cache && cache[dirPath];

    if (dir) {
        return dir.then(function (dir) {
            return dir.concat();
        });
    }

    var pattern = '**/*' + this.extname;

    // Optimistically cache dir promise to reduce file system I/O, but remove
    // from cache if there was a problem.
    dir = cache[dirPath] = new Promise(function (resolve, reject) {
        glob(pattern, {
            cwd   : dirPath,
            follow: true
        }, function (err, dir) {
            if (err) {
                reject(err);
            } else {
                resolve(dir);
            }
        });
    });

    return dir.then(function (dir) {
        return dir.concat();
    }).catch(function (err) {
        delete cache[dirPath];
        throw err;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._getFile"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getFile (filePath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getFile)
- description and source-code
```javascript
_getFile = function (filePath, options) {
    filePath = path.resolve(filePath);
    options || (options = {});

    var cache = this._fsCache;
    var file  = options.cache && cache[filePath];

    if (file) {
        return file;
    }

    // Optimistically cache file promise to reduce file system I/O, but remove
    // from cache if there was a problem.
    file = cache[filePath] = new Promise(function (resolve, reject) {
        fs.readFile(filePath, 'utf8', function (err, file) {
            if (err) {
                reject(err);
            } else {
                resolve(file);
            }
        });
    });

    return file.catch(function (err) {
        delete cache[filePath];
        throw err;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._getTemplateName"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_getTemplateName (filePath, namespace)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._getTemplateName)
- description and source-code
```javascript
_getTemplateName = function (filePath, namespace) {
    var extRegex = new RegExp(this.extname + '$');
    var name     = filePath.replace(extRegex, '');

    if (namespace) {
        name = namespace + '/' + name;
    }

    return name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._precompileTemplate"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_precompileTemplate (template, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._precompileTemplate)
- description and source-code
```javascript
_precompileTemplate = function (template, options) {
    return this.handlebars.precompile(template, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._renderTemplate"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_renderTemplate (template, context, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._renderTemplate)
- description and source-code
```javascript
_renderTemplate = function (template, context, options) {
    return template(context, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype._resolveLayoutPath"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>_resolveLayoutPath (layoutPath)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype._resolveLayoutPath)
- description and source-code
```javascript
_resolveLayoutPath = function (layoutPath) {
    if (!layoutPath) {
        return null;
    }

    if (!path.extname(layoutPath)) {
        layoutPath += this.extname;
    }

    return path.resolve(this.layoutsDir, layoutPath);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype.getPartials"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getPartials (options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getPartials)
- description and source-code
```javascript
getPartials = function (options) {
    var partialsDirs = Array.isArray(this.partialsDir) ?
            this.partialsDir : [this.partialsDir];

    partialsDirs = partialsDirs.map(function (dir) {
        var dirPath;
        var dirTemplates;
        var dirNamespace;

        // Support 'partialsDir' collection with object entries that contain a
        // templates promise and a namespace.
        if (typeof dir === 'string') {
            dirPath = dir;
        } else if (typeof dir === 'object') {
            dirTemplates = dir.templates;
            dirNamespace = dir.namespace;
            dirPath      = dir.dir;
        }

        // We must have some path to templates, or templates themselves.
        if (!(dirPath || dirTemplates)) {
            throw new Error('A partials dir must be a string or config object');
        }

        // Make sure we're have a promise for the templates.
        var templatesPromise = dirTemplates ? Promise.resolve(dirTemplates) :
                this.getTemplates(dirPath, options);

        return templatesPromise.then(function (templates) {
            return {
                templates: templates,
                namespace: dirNamespace,
            };
        });
    }, this);

    return Promise.all(partialsDirs).then(function (dirs) {
        var getTemplateName = this._getTemplateName.bind(this);

        return dirs.reduce(function (partials, dir) {
            var templates = dir.templates;
            var namespace = dir.namespace;
            var filePaths = Object.keys(templates);

            filePaths.forEach(function (filePath) {
                var partialName       = getTemplateName(filePath, namespace);
                partials[partialName] = templates[filePath];
            });

            return partials;
        }, {});
    }.bind(this));
}
```
- example usage
```shell
...
'''

'getPartials()' would produce the following result:

'''javascript
var hbs = require('express-handlebars').create();

hbs.getPartials().then(function (partials) {
    console.log(partials);
    // => { 'foo/bar': [Function],
    // =>    title: [Function] }
});
'''

#### 'getTemplate(filePath, [options])'
...
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplate"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getTemplate (filePath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplate)
- description and source-code
```javascript
getTemplate = function (filePath, options) {
    filePath = path.resolve(filePath);
    options || (options = {});

    var precompiled = options.precompiled;
    var cache       = precompiled ? this.precompiled : this.compiled;
    var template    = options.cache && cache[filePath];

    if (template) {
        return template;
    }

    // Optimistically cache template promise to reduce file system I/O, but
    // remove from cache if there was a problem.
    template = cache[filePath] = this._getFile(filePath, {cache: options.cache})
        .then(function (file) {
            if (precompiled) {
                return this._precompileTemplate(file, this.compilerOptions);
            }

            return this._compileTemplate(file, this.compilerOptions);
        }.bind(this));

    return template.catch(function (err) {
        delete cache[filePath];
        throw err;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplates"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>getTemplates (dirPath, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.getTemplates)
- description and source-code
```javascript
getTemplates = function (dirPath, options) {
    options || (options = {});
    var cache = options.cache;

    return this._getDir(dirPath, {cache: cache}).then(function (filePaths) {
        var templates = filePaths.map(function (filePath) {
            return this.getTemplate(path.join(dirPath, filePath), options);
        }, this);

        return Promise.all(templates).then(function (templates) {
            return filePaths.reduce(function (hash, filePath, i) {
                hash[filePath] = templates[i];
                return hash;
            }, {});
        });
    }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype.render"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>render (filePath, context, options)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.render)
- description and source-code
```javascript
render = function (filePath, context, options) {
    options || (options = {});

    return Promise.all([
        this.getTemplate(filePath, {cache: options.cache}),
        options.partials || this.getPartials({cache: options.cache}),
    ]).then(function (templates) {
        var template = templates[0];
        var partials = templates[1];
        var helpers  = options.helpers || this.helpers;

        // Add ExpressHandlebars metadata to the data channel so that it's
        // accessible within the templates and helpers, namespaced under:
        // '@exphbs.*'
        var data = utils.assign({}, options.data, {
            exphbs: utils.assign({}, options, {
                filePath: filePath,
                helpers : helpers,
                partials: partials,
            }),
        });

        return this._renderTemplate(template, context, {
            data    : data,
            helpers : helpers,
            partials: partials,
        });
    }.bind(this));
}
```
- example usage
```shell
...

var app = express();

app.engine('handlebars', exphbs({defaultLayout: 'main'}));
app.set('view engine', 'handlebars');

app.get('/', function (req, res) {
    res.render('home');
});

app.listen(3000);
'''

**views/layouts/main.handlebars:**
...
```

#### <a name="apidoc.element.express-handlebars.ExpressHandlebars.prototype.renderView"></a>[function <span class="apidocSignatureSpan">express-handlebars.ExpressHandlebars.prototype.</span>renderView (viewPath, options, callback)](#apidoc.element.express-handlebars.ExpressHandlebars.prototype.renderView)
- description and source-code
```javascript
renderView = function (viewPath, options, callback) {
    options || (options = {});

    var context = options;

    // Express provides 'settings.views' which is the path to the views dir that
    // the developer set on the Express app. When this value exists, it's used
    // to compute the view's name.
    var view;
    var viewsPath = options.settings && options.settings.views;
    if (viewsPath) {
        view = this._getTemplateName(path.relative(viewsPath, viewPath));
    }

    // Merge render-level and instance-level helpers together.
    var helpers = utils.assign({}, this.helpers, options.helpers);

    // Merge render-level and instance-level partials together.
    var partials = Promise.all([
        this.getPartials({cache: options.cache}),
        Promise.resolve(options.partials),
    ]).then(function (partials) {
        return utils.assign.apply(null, [{}].concat(partials));
    });

    // Pluck-out ExpressHandlebars-specific options and Handlebars-specific
    // rendering options.
    options = {
        cache : options.cache,
        view  : view,
        layout: 'layout' in options ? options.layout : this.defaultLayout,

        data    : options.data,
        helpers : helpers,
        partials: partials,
    };

    this.render(viewPath, context, options)
        .then(function (body) {
            var layoutPath = this._resolveLayoutPath(options.layout);

            if (layoutPath) {
                return this.render(
                    layoutPath,
                    utils.assign({}, context, {body: body}),
                    utils.assign({}, options, {layout: undefined})
                );
            }

            return body;
        }.bind(this))
        .then(utils.passValue(callback))
        .catch(utils.passError(callback));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-handlebars.utils"></a>[module express-handlebars.utils](#apidoc.module.express-handlebars.utils)

#### <a name="apidoc.element.express-handlebars.utils.assign"></a>[function <span class="apidocSignatureSpan">express-handlebars.utils.</span>assign ()](#apidoc.element.express-handlebars.utils.assign)
- description and source-code
```javascript
function assign() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.utils.passError"></a>[function <span class="apidocSignatureSpan">express-handlebars.utils.</span>passError (callback)](#apidoc.element.express-handlebars.utils.passError)
- description and source-code
```javascript
function passError(callback) {
    return function (reason) {
        setImmediate(function () {
            callback(reason);
        });
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-handlebars.utils.passValue"></a>[function <span class="apidocSignatureSpan">express-handlebars.utils.</span>passValue (callback)](#apidoc.element.express-handlebars.utils.passValue)
- description and source-code
```javascript
function passValue(callback) {
    return function (value) {
        setImmediate(function () {
            callback(null, value);
        });
    };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
