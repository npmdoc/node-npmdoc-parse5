# api documentation for  [parse5 (v3.0.2)](https://github.com/inikulin/parse5)  [![npm package](https://img.shields.io/npm/v/npmdoc-parse5.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-parse5) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-parse5.svg)](https://travis-ci.org/npmdoc/node-npmdoc-parse5)
#### HTML parsing/serialization toolset for Node.js. WHATWG HTML Living Standard (aka HTML5)-compliant.

[![NPM](https://nodei.co/npm/parse5.png?downloads=true)](https://www.npmjs.com/package/parse5)

[![apidoc](https://npmdoc.github.io/node-npmdoc-parse5/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-parse5_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-parse5/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-parse5/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-parse5/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ivan Nikulin",
        "email": "ifaaan@gmail.com",
        "url": "https://github.com/inikulin"
    },
    "bugs": {
        "url": "https://github.com/inikulin/parse5/issues"
    },
    "contributors": "https://github.com/inikulin/parse5/graphs/contributors",
    "dependencies": {
        "@types/node": "^6.0.46"
    },
    "description": "HTML parsing/serialization toolset for Node.js. WHATWG HTML Living Standard (aka HTML5)-compliant.",
    "devDependencies": {
        "del": "^2.0.2",
        "gulp": "^3.9.0",
        "gulp-benchmark": "^1.1.1",
        "gulp-download": "0.0.1",
        "gulp-eslint": "^3.0.1",
        "gulp-install": "^0.6.0",
        "gulp-mocha": "^2.1.3",
        "gulp-rename": "^1.2.2",
        "gulp-typedoc": "^2.0.0",
        "gulp-typescript": "^3.1.2",
        "publish-please": "^2.2.0",
        "through2": "^2.0.0",
        "typedoc": "^0.5.1",
        "typescript": "^2.0.6"
    },
    "directories": {},
    "dist": {
        "shasum": "05eff57f0ef4577fb144a79f8b9a967a6cc44510",
        "tarball": "https://registry.npmjs.org/parse5/-/parse5-3.0.2.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "969ed22f53db38c101449e05a1b804ea456d4e04",
    "homepage": "https://github.com/inikulin/parse5",
    "keywords": [
        "html",
        "parser",
        "html5",
        "WHATWG",
        "specification",
        "fast",
        "html parser",
        "html5 parser",
        "htmlparser",
        "parse5",
        "serializer",
        "html serializer",
        "htmlserializer",
        "sax",
        "simple api",
        "parse",
        "tokenize",
        "serialize",
        "tokenizer"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "inikulin",
            "email": "ifaaan@gmail.com"
        }
    ],
    "name": "parse5",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/inikulin/parse5.git"
    },
    "scripts": {
        "prepublish": "publish-please guard",
        "publish-please": "publish-please",
        "test": "gulp test"
    },
    "types": "./lib/index.d.ts",
    "version": "3.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module parse5](#apidoc.module.parse5)
1.  [function <span class="apidocSignatureSpan">parse5.</span>ParserStream (options)](#apidoc.element.parse5.ParserStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>PlainTextConversionStream (options)](#apidoc.element.parse5.PlainTextConversionStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>SAXParser (options)](#apidoc.element.parse5.SAXParser)
1.  [function <span class="apidocSignatureSpan">parse5.</span>SerializerStream (node, options)](#apidoc.element.parse5.SerializerStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>parse (html, options)](#apidoc.element.parse5.parse)
1.  [function <span class="apidocSignatureSpan">parse5.</span>parseFragment (fragmentContext, html, options)](#apidoc.element.parse5.parseFragment)
1.  [function <span class="apidocSignatureSpan">parse5.</span>serialize (node, options)](#apidoc.element.parse5.serialize)
1.  object <span class="apidocSignatureSpan">parse5.</span>ParserStream.prototype
1.  object <span class="apidocSignatureSpan">parse5.</span>SAXParser.prototype
1.  object <span class="apidocSignatureSpan">parse5.</span>SerializerStream.prototype
1.  object <span class="apidocSignatureSpan">parse5.</span>treeAdapters

#### [module parse5.ParserStream](#apidoc.module.parse5.ParserStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>ParserStream (options)](#apidoc.element.parse5.ParserStream.ParserStream)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.</span>super_ (options)](#apidoc.element.parse5.ParserStream.super_)

#### [module parse5.ParserStream.prototype](#apidoc.module.parse5.ParserStream.prototype)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_documentWrite (html)](#apidoc.element.parse5.ParserStream.prototype._documentWrite)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_resume ()](#apidoc.element.parse5.ParserStream.prototype._resume)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_runParsingLoop ()](#apidoc.element.parse5.ParserStream.prototype._runParsingLoop)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_scriptHandler (scriptElement)](#apidoc.element.parse5.ParserStream.prototype._scriptHandler)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.parse5.ParserStream.prototype._write)
1.  [function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>end (chunk, encoding, callback)](#apidoc.element.parse5.ParserStream.prototype.end)

#### [module parse5.PlainTextConversionStream](#apidoc.module.parse5.PlainTextConversionStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>PlainTextConversionStream (options)](#apidoc.element.parse5.PlainTextConversionStream.PlainTextConversionStream)
1.  [function <span class="apidocSignatureSpan">parse5.PlainTextConversionStream.</span>super_ (options)](#apidoc.element.parse5.PlainTextConversionStream.super_)

#### [module parse5.SAXParser](#apidoc.module.parse5.SAXParser)
1.  [function <span class="apidocSignatureSpan">parse5.</span>SAXParser (options)](#apidoc.element.parse5.SAXParser.SAXParser)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.</span>super_ (options)](#apidoc.element.parse5.SAXParser.super_)

#### [module parse5.SAXParser.prototype](#apidoc.module.parse5.SAXParser.prototype)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_emitPendingText ()](#apidoc.element.parse5.SAXParser.prototype._emitPendingText)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_flush (callback)](#apidoc.element.parse5.SAXParser.prototype._flush)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_handleToken (token)](#apidoc.element.parse5.SAXParser.prototype._handleToken)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_runParsingLoop ()](#apidoc.element.parse5.SAXParser.prototype._runParsingLoop)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.parse5.SAXParser.prototype._transform)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>end (chunk, encoding, callback)](#apidoc.element.parse5.SAXParser.prototype.end)
1.  [function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>stop ()](#apidoc.element.parse5.SAXParser.prototype.stop)

#### [module parse5.SerializerStream](#apidoc.module.parse5.SerializerStream)
1.  [function <span class="apidocSignatureSpan">parse5.</span>SerializerStream (node, options)](#apidoc.element.parse5.SerializerStream.SerializerStream)
1.  [function <span class="apidocSignatureSpan">parse5.SerializerStream.</span>super_ (options)](#apidoc.element.parse5.SerializerStream.super_)

#### [module parse5.SerializerStream.prototype](#apidoc.module.parse5.SerializerStream.prototype)
1.  [function <span class="apidocSignatureSpan">parse5.SerializerStream.prototype.</span>_read ()](#apidoc.element.parse5.SerializerStream.prototype._read)



# <a name="apidoc.module.parse5"></a>[module parse5](#apidoc.module.parse5)

#### <a name="apidoc.element.parse5.ParserStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>ParserStream (options)](#apidoc.element.parse5.ParserStream)
- description and source-code
```javascript
ParserStream = function (options) {
    WritableStream.call(this);

    this.parser = new Parser(options);

    this.lastChunkWritten = false;
    this.writeCallback = null;
    this.pausedByScript = false;

    this.document = this.parser.treeAdapter.createDocument();

    this.pendingHtmlInsertions = [];

    this._resume = this._resume.bind(this);
    this._documentWrite = this._documentWrite.bind(this);
    this._scriptHandler = this._scriptHandler.bind(this);

    this.parser._bootstrap(this.document, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.PlainTextConversionStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>PlainTextConversionStream (options)](#apidoc.element.parse5.PlainTextConversionStream)
- description and source-code
```javascript
PlainTextConversionStream = function (options) {
    ParserStream.call(this, options);

    // NOTE: see https://html.spec.whatwg.org/#read-text
    this.parser._insertFakeElement($.HTML);
    this.parser._insertFakeElement($.HEAD);
    this.parser.openElements.pop();
    this.parser._insertFakeElement($.BODY);
    this.parser._insertFakeElement($.PRE);
    this.parser.treeAdapter.insertText(this.parser.openElements.current, '\n');
    this.parser.switchToPlaintextParsing();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser"></a>[function <span class="apidocSignatureSpan">parse5.</span>SAXParser (options)](#apidoc.element.parse5.SAXParser)
- description and source-code
```javascript
SAXParser = function (options) {
    TransformStream.call(this);

    this.options = mergeOptions(DEFAULT_OPTIONS, options);

    this.tokenizer = new Tokenizer(options);
    this.parserFeedbackSimulator = new ParserFeedbackSimulator(this.tokenizer);

    this.pendingText = null;
    this.currentTokenLocation = void 0;

    this.lastChunkWritten = false;
    this.stopped = false;

    // NOTE: always pipe stream to the /dev/null stream to avoid
    // 'highWaterMark' hit even if we don't have consumers.
    // (see: https://github.com/inikulin/parse5/issues/97#issuecomment-171940774)
    this.pipe(new DevNullStream());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SerializerStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>SerializerStream (node, options)](#apidoc.element.parse5.SerializerStream)
- description and source-code
```javascript
SerializerStream = function (node, options) {
    ReadableStream.call(this);

    this.serializer = new Serializer(node, options);

    Object.defineProperty(this.serializer, 'html', {
        //NOTE: To make '+=' concat operator work properly we define
        //getter which always returns empty string
        get: function () {
            return '';
        },
        set: this.push.bind(this)
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.parse"></a>[function <span class="apidocSignatureSpan">parse5.</span>parse (html, options)](#apidoc.element.parse5.parse)
- description and source-code
```javascript
function parse(html, options) {
    var parser = new Parser(options);

    return parser.parse(html);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.parseFragment"></a>[function <span class="apidocSignatureSpan">parse5.</span>parseFragment (fragmentContext, html, options)](#apidoc.element.parse5.parseFragment)
- description and source-code
```javascript
function parseFragment(fragmentContext, html, options) {
    if (typeof fragmentContext === 'string') {
        options = html;
        html = fragmentContext;
        fragmentContext = null;
    }

    var parser = new Parser(options);

    return parser.parseFragment(html, fragmentContext);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.serialize"></a>[function <span class="apidocSignatureSpan">parse5.</span>serialize (node, options)](#apidoc.element.parse5.serialize)
- description and source-code
```javascript
serialize = function (node, options) {
    var serializer = new Serializer(node, options);

    return serializer.serialize();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.ParserStream"></a>[module parse5.ParserStream](#apidoc.module.parse5.ParserStream)

#### <a name="apidoc.element.parse5.ParserStream.ParserStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>ParserStream (options)](#apidoc.element.parse5.ParserStream.ParserStream)
- description and source-code
```javascript
ParserStream = function (options) {
    WritableStream.call(this);

    this.parser = new Parser(options);

    this.lastChunkWritten = false;
    this.writeCallback = null;
    this.pausedByScript = false;

    this.document = this.parser.treeAdapter.createDocument();

    this.pendingHtmlInsertions = [];

    this._resume = this._resume.bind(this);
    this._documentWrite = this._documentWrite.bind(this);
    this._scriptHandler = this._scriptHandler.bind(this);

    this.parser._bootstrap(this.document, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.super_"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.</span>super_ (options)](#apidoc.element.parse5.ParserStream.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.ParserStream.prototype"></a>[module parse5.ParserStream.prototype](#apidoc.module.parse5.ParserStream.prototype)

#### <a name="apidoc.element.parse5.ParserStream.prototype._documentWrite"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_documentWrite (html)](#apidoc.element.parse5.ParserStream.prototype._documentWrite)
- description and source-code
```javascript
_documentWrite = function (html) {
    if (!this.parser.stopped)
        this.pendingHtmlInsertions.push(html);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.prototype._resume"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_resume ()](#apidoc.element.parse5.ParserStream.prototype._resume)
- description and source-code
```javascript
_resume = function () {
    if (!this.pausedByScript)
        throw new Error('Parser was already resumed');

    while (this.pendingHtmlInsertions.length) {
        var html = this.pendingHtmlInsertions.pop();

        this.parser.tokenizer.insertHtmlAtCurrentPos(html);
    }

    this.pausedByScript = false;

    //NOTE: keep parsing if we don't wait for the next input chunk
    if (this.parser.tokenizer.active)
        this._runParsingLoop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.prototype._runParsingLoop"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_runParsingLoop ()](#apidoc.element.parse5.ParserStream.prototype._runParsingLoop)
- description and source-code
```javascript
_runParsingLoop = function () {
    this.parser.runParsingLoopForCurrentChunk(this.writeCallback, this._scriptHandler);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.prototype._scriptHandler"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_scriptHandler (scriptElement)](#apidoc.element.parse5.ParserStream.prototype._scriptHandler)
- description and source-code
```javascript
_scriptHandler = function (scriptElement) {
    if (this.listeners('script').length) {
        this.pausedByScript = true;
        this.emit('script', scriptElement, this._documentWrite, this._resume);
    }
    else
        this._runParsingLoop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.prototype._write"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.parse5.ParserStream.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
    this.writeCallback = callback;
    this.parser.tokenizer.write(chunk.toString('utf8'), this.lastChunkWritten);
    this._runParsingLoop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.ParserStream.prototype.end"></a>[function <span class="apidocSignatureSpan">parse5.ParserStream.prototype.</span>end (chunk, encoding, callback)](#apidoc.element.parse5.ParserStream.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, callback) {
    this.lastChunkWritten = true;
    WritableStream.prototype.end.call(this, chunk, encoding, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.PlainTextConversionStream"></a>[module parse5.PlainTextConversionStream](#apidoc.module.parse5.PlainTextConversionStream)

#### <a name="apidoc.element.parse5.PlainTextConversionStream.PlainTextConversionStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>PlainTextConversionStream (options)](#apidoc.element.parse5.PlainTextConversionStream.PlainTextConversionStream)
- description and source-code
```javascript
PlainTextConversionStream = function (options) {
    ParserStream.call(this, options);

    // NOTE: see https://html.spec.whatwg.org/#read-text
    this.parser._insertFakeElement($.HTML);
    this.parser._insertFakeElement($.HEAD);
    this.parser.openElements.pop();
    this.parser._insertFakeElement($.BODY);
    this.parser._insertFakeElement($.PRE);
    this.parser.treeAdapter.insertText(this.parser.openElements.current, '\n');
    this.parser.switchToPlaintextParsing();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.PlainTextConversionStream.super_"></a>[function <span class="apidocSignatureSpan">parse5.PlainTextConversionStream.</span>super_ (options)](#apidoc.element.parse5.PlainTextConversionStream.super_)
- description and source-code
```javascript
super_ = function (options) {
    WritableStream.call(this);

    this.parser = new Parser(options);

    this.lastChunkWritten = false;
    this.writeCallback = null;
    this.pausedByScript = false;

    this.document = this.parser.treeAdapter.createDocument();

    this.pendingHtmlInsertions = [];

    this._resume = this._resume.bind(this);
    this._documentWrite = this._documentWrite.bind(this);
    this._scriptHandler = this._scriptHandler.bind(this);

    this.parser._bootstrap(this.document, null);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.SAXParser"></a>[module parse5.SAXParser](#apidoc.module.parse5.SAXParser)

#### <a name="apidoc.element.parse5.SAXParser.SAXParser"></a>[function <span class="apidocSignatureSpan">parse5.</span>SAXParser (options)](#apidoc.element.parse5.SAXParser.SAXParser)
- description and source-code
```javascript
SAXParser = function (options) {
    TransformStream.call(this);

    this.options = mergeOptions(DEFAULT_OPTIONS, options);

    this.tokenizer = new Tokenizer(options);
    this.parserFeedbackSimulator = new ParserFeedbackSimulator(this.tokenizer);

    this.pendingText = null;
    this.currentTokenLocation = void 0;

    this.lastChunkWritten = false;
    this.stopped = false;

    // NOTE: always pipe stream to the /dev/null stream to avoid
    // 'highWaterMark' hit even if we don't have consumers.
    // (see: https://github.com/inikulin/parse5/issues/97#issuecomment-171940774)
    this.pipe(new DevNullStream());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.super_"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.</span>super_ (options)](#apidoc.element.parse5.SAXParser.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function')
      this._transform = options.transform;

    if (typeof options.flush === 'function')
      this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function() {
    if (typeof this._flush === 'function')
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.SAXParser.prototype"></a>[module parse5.SAXParser.prototype](#apidoc.module.parse5.SAXParser.prototype)

#### <a name="apidoc.element.parse5.SAXParser.prototype._emitPendingText"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_emitPendingText ()](#apidoc.element.parse5.SAXParser.prototype._emitPendingText)
- description and source-code
```javascript
_emitPendingText = function () {
    if (this.pendingText !== null) {
        this.emit('text', this.pendingText, this.currentTokenLocation);
        this.pendingText = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype._flush"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_flush (callback)](#apidoc.element.parse5.SAXParser.prototype._flush)
- description and source-code
```javascript
_flush = function (callback) {
    callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype._handleToken"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_handleToken (token)](#apidoc.element.parse5.SAXParser.prototype._handleToken)
- description and source-code
```javascript
_handleToken = function (token) {
    if (this.options.locationInfo)
        this.currentTokenLocation = token.location;

    if (token.type === Tokenizer.START_TAG_TOKEN)
        this.emit('startTag', token.tagName, token.attrs, token.selfClosing, this.currentTokenLocation);

    else if (token.type === Tokenizer.END_TAG_TOKEN)
        this.emit('endTag', token.tagName, this.currentTokenLocation);

    else if (token.type === Tokenizer.COMMENT_TOKEN)
        this.emit('comment', token.data, this.currentTokenLocation);

    else if (token.type === Tokenizer.DOCTYPE_TOKEN)
        this.emit('doctype', token.name, token.publicId, token.systemId, this.currentTokenLocation);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype._runParsingLoop"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_runParsingLoop ()](#apidoc.element.parse5.SAXParser.prototype._runParsingLoop)
- description and source-code
```javascript
_runParsingLoop = function () {
    do {
        var token = this.parserFeedbackSimulator.getNextToken();

        if (token.type === Tokenizer.HIBERNATION_TOKEN)
            break;

        if (token.type === Tokenizer.CHARACTER_TOKEN ||
            token.type === Tokenizer.WHITESPACE_CHARACTER_TOKEN ||
            token.type === Tokenizer.NULL_CHARACTER_TOKEN) {

            if (this.options.locationInfo) {
                if (this.pendingText === null)
                    this.currentTokenLocation = token.location;

                else
                    this.currentTokenLocation.endOffset = token.location.endOffset;
            }

            this.pendingText = (this.pendingText || '') + token.chars;
        }

        else {
            this._emitPendingText();
            this._handleToken(token);
        }
    } while (!this.stopped && token.type !== Tokenizer.EOF_TOKEN);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype._transform"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>_transform (chunk, encoding, callback)](#apidoc.element.parse5.SAXParser.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, callback) {
    if (!this.stopped) {
        this.tokenizer.write(chunk.toString('utf8'), this.lastChunkWritten);
        this._runParsingLoop();
    }

    this.push(chunk);

    callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype.end"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>end (chunk, encoding, callback)](#apidoc.element.parse5.SAXParser.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, callback) {
    this.lastChunkWritten = true;
    TransformStream.prototype.end.call(this, chunk, encoding, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SAXParser.prototype.stop"></a>[function <span class="apidocSignatureSpan">parse5.SAXParser.prototype.</span>stop ()](#apidoc.element.parse5.SAXParser.prototype.stop)
- description and source-code
```javascript
stop = function () {
    this.stopped = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.SerializerStream"></a>[module parse5.SerializerStream](#apidoc.module.parse5.SerializerStream)

#### <a name="apidoc.element.parse5.SerializerStream.SerializerStream"></a>[function <span class="apidocSignatureSpan">parse5.</span>SerializerStream (node, options)](#apidoc.element.parse5.SerializerStream.SerializerStream)
- description and source-code
```javascript
SerializerStream = function (node, options) {
    ReadableStream.call(this);

    this.serializer = new Serializer(node, options);

    Object.defineProperty(this.serializer, 'html', {
        //NOTE: To make '+=' concat operator work properly we define
        //getter which always returns empty string
        get: function () {
            return '';
        },
        set: this.push.bind(this)
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse5.SerializerStream.super_"></a>[function <span class="apidocSignatureSpan">parse5.SerializerStream.</span>super_ (options)](#apidoc.element.parse5.SerializerStream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse5.SerializerStream.prototype"></a>[module parse5.SerializerStream.prototype](#apidoc.module.parse5.SerializerStream.prototype)

#### <a name="apidoc.element.parse5.SerializerStream.prototype._read"></a>[function <span class="apidocSignatureSpan">parse5.SerializerStream.prototype.</span>_read ()](#apidoc.element.parse5.SerializerStream.prototype._read)
- description and source-code
```javascript
_read = function () {
    this.serializer.serialize();
    this.push(null);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
