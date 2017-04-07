# api documentation for  [iconv-lite (v0.4.15)](https://github.com/ashtuchkin/iconv-lite)  [![npm package](https://img.shields.io/npm/v/npmdoc-iconv-lite.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-iconv-lite) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-iconv-lite.svg)](https://travis-ci.org/npmdoc/node-npmdoc-iconv-lite)
#### Convert character encodings in pure javascript.

[![NPM](https://nodei.co/npm/iconv-lite.png?downloads=true)](https://www.npmjs.com/package/iconv-lite)

[![apidoc](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-iconv-lite%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alexander Shtuchkin",
        "email": "ashtuchkin@gmail.com"
    },
    "browser": {
        "./extend-node": false,
        "./streams": false
    },
    "bugs": {
        "url": "https://github.com/ashtuchkin/iconv-lite/issues"
    },
    "contributors": [
        {
            "name": "Jinwu Zhan",
            "url": "https://github.com/jenkinv"
        },
        {
            "name": "Adamansky Anton",
            "url": "https://github.com/adamansky"
        },
        {
            "name": "George Stagas",
            "url": "https://github.com/stagas"
        },
        {
            "name": "Mike D Pilsbury",
            "url": "https://github.com/pekim"
        },
        {
            "name": "Niggler",
            "url": "https://github.com/Niggler"
        },
        {
            "name": "wychi",
            "url": "https://github.com/wychi"
        },
        {
            "name": "David Kuo",
            "url": "https://github.com/david50407"
        },
        {
            "name": "ChangZhuo Chen",
            "url": "https://github.com/czchen"
        },
        {
            "name": "Lee Treveil",
            "url": "https://github.com/leetreveil"
        },
        {
            "name": "Brian White",
            "url": "https://github.com/mscdex"
        },
        {
            "name": "Mithgol",
            "url": "https://github.com/Mithgol"
        },
        {
            "name": "Nazar Leush",
            "url": "https://github.com/nleush"
        }
    ],
    "dependencies": {},
    "description": "Convert character encodings in pure javascript.",
    "devDependencies": {
        "async": "*",
        "errto": "*",
        "iconv": "*",
        "istanbul": "*",
        "mocha": "*",
        "request": "*",
        "unorm": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "fe265a218ac6a57cfe854927e9d04c19825eddeb",
        "tarball": "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.4.15.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "c3bcedcd6a5025c25e39ed1782347acaed1d290f",
    "homepage": "https://github.com/ashtuchkin/iconv-lite",
    "keywords": [
        "iconv",
        "convert",
        "charset",
        "icu"
    ],
    "license": "MIT",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "ashtuchkin",
            "email": "ashtuchkin@gmail.com"
        }
    ],
    "name": "iconv-lite",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/ashtuchkin/iconv-lite.git"
    },
    "scripts": {
        "coverage": "istanbul cover _mocha -- --grep .",
        "coverage-open": "open coverage/lcov-report/index.html",
        "test": "mocha --reporter spec --grep ."
    },
    "typings": "./lib/index.d.ts",
    "version": "0.4.15"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module iconv-lite](#apidoc.module.iconv-lite)
1.  boolean <span class="apidocSignatureSpan">iconv-lite.</span>supportsNodeEncodingsExtension
1.  boolean <span class="apidocSignatureSpan">iconv-lite.</span>supportsStreams
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteDecoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteDecoderStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteEncoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteEncoderStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>_collect (cb)](#apidoc.element.iconv-lite._collect)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>decode (buf, encoding, options)](#apidoc.element.iconv-lite.decode)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>decodeStream (encoding, options)](#apidoc.element.iconv-lite.decodeStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>encode (str, encoding, options)](#apidoc.element.iconv-lite.encode)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>encodeStream (encoding, options)](#apidoc.element.iconv-lite.encodeStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>encodingExists (enc)](#apidoc.element.iconv-lite.encodingExists)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>extendNodeEncodings ()](#apidoc.element.iconv-lite.extendNodeEncodings)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>fromEncoding (buf, encoding, options)](#apidoc.element.iconv-lite.fromEncoding)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>getCodec (encoding)](#apidoc.element.iconv-lite.getCodec)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>getDecoder (encoding, options)](#apidoc.element.iconv-lite.getDecoder)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>getEncoder (encoding, options)](#apidoc.element.iconv-lite.getEncoder)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>toEncoding (str, encoding, options)](#apidoc.element.iconv-lite.toEncoding)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>undoExtendNodeEncodings ()](#apidoc.element.iconv-lite.undoExtendNodeEncodings)
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteDecoderStream.prototype
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteEncoderStream.prototype
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>_codecDataCache
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>bom_handling
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>dbcs_codec
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>encodings
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>internal
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>sbcs_codec
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>utf16
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>utf7
1.  string <span class="apidocSignatureSpan">iconv-lite.</span>defaultCharSingleByte
1.  string <span class="apidocSignatureSpan">iconv-lite.</span>defaultCharUnicode

#### [module iconv-lite.IconvLiteDecoderStream](#apidoc.module.iconv-lite.IconvLiteDecoderStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteDecoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.IconvLiteDecoderStream)

#### [module iconv-lite.IconvLiteDecoderStream.prototype](#apidoc.module.iconv-lite.IconvLiteDecoderStream.prototype)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>_flush (done)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._flush)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>_transform (chunk, encoding, done)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._transform)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>collect (cb)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype.collect)

#### [module iconv-lite.IconvLiteEncoderStream](#apidoc.module.iconv-lite.IconvLiteEncoderStream)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteEncoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.IconvLiteEncoderStream)

#### [module iconv-lite.IconvLiteEncoderStream.prototype](#apidoc.module.iconv-lite.IconvLiteEncoderStream.prototype)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>_flush (done)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._flush)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>_transform (chunk, encoding, done)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._transform)
1.  [function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>collect (cb)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype.collect)

#### [module iconv-lite.bom_handling](#apidoc.module.iconv-lite.bom_handling)
1.  [function <span class="apidocSignatureSpan">iconv-lite.bom_handling.</span>PrependBOM (encoder, options)](#apidoc.element.iconv-lite.bom_handling.PrependBOM)
1.  [function <span class="apidocSignatureSpan">iconv-lite.bom_handling.</span>StripBOM (decoder, options)](#apidoc.element.iconv-lite.bom_handling.StripBOM)

#### [module iconv-lite.dbcs_codec](#apidoc.module.iconv-lite.dbcs_codec)
1.  [function <span class="apidocSignatureSpan">iconv-lite.dbcs_codec.</span>_dbcs (codecOptions, iconv)](#apidoc.element.iconv-lite.dbcs_codec._dbcs)

#### [module iconv-lite.internal](#apidoc.module.iconv-lite.internal)
1.  [function <span class="apidocSignatureSpan">iconv-lite.internal.</span>_internal (codecOptions, iconv)](#apidoc.element.iconv-lite.internal._internal)
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>base64
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>binary
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>cesu8
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>hex
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>ucs2
1.  object <span class="apidocSignatureSpan">iconv-lite.internal.</span>utf8
1.  string <span class="apidocSignatureSpan">iconv-lite.internal.</span>unicode11utf8
1.  string <span class="apidocSignatureSpan">iconv-lite.internal.</span>utf16le

#### [module iconv-lite.sbcs_codec](#apidoc.module.iconv-lite.sbcs_codec)
1.  [function <span class="apidocSignatureSpan">iconv-lite.sbcs_codec.</span>_sbcs (codecOptions, iconv)](#apidoc.element.iconv-lite.sbcs_codec._sbcs)

#### [module iconv-lite.utf16](#apidoc.module.iconv-lite.utf16)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>utf16 (codecOptions, iconv)](#apidoc.element.iconv-lite.utf16.utf16)
1.  [function <span class="apidocSignatureSpan">iconv-lite.utf16.</span>utf16be ()](#apidoc.element.iconv-lite.utf16.utf16be)

#### [module iconv-lite.utf7](#apidoc.module.iconv-lite.utf7)
1.  [function <span class="apidocSignatureSpan">iconv-lite.</span>utf7 (codecOptions, iconv)](#apidoc.element.iconv-lite.utf7.utf7)
1.  [function <span class="apidocSignatureSpan">iconv-lite.utf7.</span>utf7imap (codecOptions, iconv)](#apidoc.element.iconv-lite.utf7.utf7imap)
1.  string <span class="apidocSignatureSpan">iconv-lite.utf7.</span>unicode11utf7



# <a name="apidoc.module.iconv-lite"></a>[module iconv-lite](#apidoc.module.iconv-lite)

#### <a name="apidoc.element.iconv-lite.IconvLiteDecoderStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteDecoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteDecoderStream)
- description and source-code
```javascript
function IconvLiteDecoderStream(conv, options) {
    this.conv = conv;
    options = options || {};
    options.encoding = this.encoding = 'utf8'; // We output strings.
    Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.IconvLiteEncoderStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteEncoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteEncoderStream)
- description and source-code
```javascript
function IconvLiteEncoderStream(conv, options) {
    this.conv = conv;
    options = options || {};
    options.decodeStrings = false; // We accept only strings, so we don't need to decode them.
    Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite._collect"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>_collect (cb)](#apidoc.element.iconv-lite._collect)
- description and source-code
```javascript
_collect = function (cb) {
    var res = '';
    this.on('error', cb);
    this.on('data', function(chunk) { res += chunk; });
    this.on('end', function() {
        cb(null, res);
    });
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.decode"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>decode (buf, encoding, options)](#apidoc.element.iconv-lite.decode)
- description and source-code
```javascript
function decode(buf, encoding, options) {
    if (typeof buf === 'string') {
        if (!iconv.skipDecodeWarning) {
            console.error('Iconv-lite warning: decode()-ing strings is deprecated. Refer to https://github.com/ashtuchkin/iconv-
lite/wiki/Use-Buffers-when-decoding');
            iconv.skipDecodeWarning = true;
        }

        buf = new Buffer("" + (buf || ""), "binary"); // Ensure buffer.
    }

    var decoder = iconv.getDecoder(encoding, options);

    var res = decoder.write(buf);
    var trail = decoder.end();

    return trail ? (res + trail) : res;
}
```
- example usage
```shell
...

## Usage
### Basic API
'''javascript
var iconv = require('iconv-lite');

// Convert from an encoded buffer to js string.
str = iconv.decode(new Buffer([0x68, 0x65, 0x6c, 0x6c, 0x6f]), 'win1251');

// Convert from js string to an encoded buffer.
buf = iconv.encode("Sample input string", 'win1251');

// Check if encoding is supported
iconv.encodingExists("us-ascii")
'''
...
```

#### <a name="apidoc.element.iconv-lite.decodeStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>decodeStream (encoding, options)](#apidoc.element.iconv-lite.decodeStream)
- description and source-code
```javascript
function decodeStream(encoding, options) {
    return new IconvLiteDecoderStream(iconv.getDecoder(encoding, options), options);
}
```
- example usage
```shell
...
'''

### Streaming API (Node v0.10+)
'''javascript

// Decode stream (from binary stream to js strings)
http.createServer(function(req, res) {
    var converterStream = iconv.decodeStream('win1251');
    req.pipe(converterStream);

    converterStream.on('data', function(str) {
        console.log(str); // Do something with decoded strings, chunk-by-chunk.
    });
});
...
```

#### <a name="apidoc.element.iconv-lite.encode"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>encode (str, encoding, options)](#apidoc.element.iconv-lite.encode)
- description and source-code
```javascript
function encode(str, encoding, options) {
    str = "" + (str || ""); // Ensure string.

    var encoder = iconv.getEncoder(encoding, options);

    var res = encoder.write(str);
    var trail = encoder.end();

    return (trail && trail.length > 0) ? Buffer.concat([res, trail]) : res;
}
```
- example usage
```shell
...
'''javascript
var iconv = require('iconv-lite');

// Convert from an encoded buffer to js string.
str = iconv.decode(new Buffer([0x68, 0x65, 0x6c, 0x6c, 0x6f]), 'win1251');

// Convert from js string to an encoded buffer.
buf = iconv.encode("Sample input string", 'win1251');

// Check if encoding is supported
iconv.encodingExists("us-ascii")
'''

### Streaming API (Node v0.10+)
'''javascript
...
```

#### <a name="apidoc.element.iconv-lite.encodeStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>encodeStream (encoding, options)](#apidoc.element.iconv-lite.encodeStream)
- description and source-code
```javascript
function encodeStream(encoding, options) {
    return new IconvLiteEncoderStream(iconv.getEncoder(encoding, options), options);
}
```
- example usage
```shell
...
    console.log(str); // Do something with decoded strings, chunk-by-chunk.
});
});

// Convert encoding streaming example
fs.createReadStream('file-in-win1251.txt')
.pipe(iconv.decodeStream('win1251'))
.pipe(iconv.encodeStream('ucs2'))
.pipe(fs.createWriteStream('file-in-ucs2.txt'));

// Sugar: all encode/decode streams have .collect(cb) method to accumulate data.
http.createServer(function(req, res) {
req.pipe(iconv.decodeStream('win1251')).collect(function(err, body) {
    assert(typeof body == 'string');
    console.log(body); // full request body string
...
```

#### <a name="apidoc.element.iconv-lite.encodingExists"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>encodingExists (enc)](#apidoc.element.iconv-lite.encodingExists)
- description and source-code
```javascript
function encodingExists(enc) {
    try {
        iconv.getCodec(enc);
        return true;
    } catch (e) {
        return false;
    }
}
```
- example usage
```shell
...
// Convert from an encoded buffer to js string.
str = iconv.decode(new Buffer([0x68, 0x65, 0x6c, 0x6c, 0x6f]), 'win1251');

// Convert from js string to an encoded buffer.
buf = iconv.encode("Sample input string", 'win1251');

// Check if encoding is supported
iconv.encodingExists("us-ascii")
'''

### Streaming API (Node v0.10+)
'''javascript

// Decode stream (from binary stream to js strings)
http.createServer(function(req, res) {
...
```

#### <a name="apidoc.element.iconv-lite.extendNodeEncodings"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>extendNodeEncodings ()](#apidoc.element.iconv-lite.extendNodeEncodings)
- description and source-code
```javascript
function extendNodeEncodings() {
    if (original) return;
    original = {};

    if (!iconv.supportsNodeEncodingsExtension) {
        console.error("ACTION NEEDED: require('iconv-lite').extendNodeEncodings() is not supported in your version of Node");
        console.error("See more info at https://github.com/ashtuchkin/iconv-lite/wiki/Node-v4-compatibility");
        return;
    }

    var nodeNativeEncodings = {
        'hex': true, 'utf8': true, 'utf-8': true, 'ascii': true, 'binary': true,
        'base64': true, 'ucs2': true, 'ucs-2': true, 'utf16le': true, 'utf-16le': true,
    };

    Buffer.isNativeEncoding = function(enc) {
        return enc && nodeNativeEncodings[enc.toLowerCase()];
    }

    // -- SlowBuffer -----------------------------------------------------------
    var SlowBuffer = require('buffer').SlowBuffer;

    original.SlowBufferToString = SlowBuffer.prototype.toString;
    SlowBuffer.prototype.toString = function(encoding, start, end) {
        encoding = String(encoding || 'utf8').toLowerCase();

        // Use native conversion when possible
        if (Buffer.isNativeEncoding(encoding))
            return original.SlowBufferToString.call(this, encoding, start, end);

        // Otherwise, use our decoding method.
        if (typeof start == 'undefined') start = 0;
        if (typeof end == 'undefined') end = this.length;
        return iconv.decode(this.slice(start, end), encoding);
    }

    original.SlowBufferWrite = SlowBuffer.prototype.write;
    SlowBuffer.prototype.write = function(string, offset, length, encoding) {
        // Support both (string, offset, length, encoding)
        // and the legacy (string, encoding, offset, length)
        if (isFinite(offset)) {
            if (!isFinite(length)) {
                encoding = length;
                length = undefined;
            }
        } else {  // legacy
            var swap = encoding;
            encoding = offset;
            offset = length;
            length = swap;
        }

        offset = +offset || 0;
        var remaining = this.length - offset;
        if (!length) {
            length = remaining;
        } else {
            length = +length;
            if (length > remaining) {
                length = remaining;
            }
        }
        encoding = String(encoding || 'utf8').toLowerCase();

        // Use native conversion when possible
        if (Buffer.isNativeEncoding(encoding))
            return original.SlowBufferWrite.call(this, string, offset, length, encoding);

        if (string.length > 0 && (length < 0 || offset < 0))
            throw new RangeError('attempt to write beyond buffer bounds');

        // Otherwise, use our encoding method.
        var buf = iconv.encode(string, encoding);
        if (buf.length < length) length = buf.length;
        buf.copy(this, offset, 0, length);
        return length;
    }

    // -- Buffer ---------------------------------------------------------------

    original.BufferIsEncoding = Buffer.isEncoding;
    Buffer.isEncoding = function(encoding) {
        return Buffer.isNativeEncoding(encoding) || iconv.encodingExists(encoding);
    }

    original.BufferByteLength = Buffer.byteLength;
    Buffer.byteLength = SlowBuffer.byteLength = function(str, encoding) {
        encoding = String(encoding || 'utf8').toLowerCase();

        // Use native conversion when possible
        if (Buffer.isNativeEncoding(encoding))
            return original.BufferByteLength.call(this, str, encoding);

        // Slow, I know, but we don't have a better way yet.
        return iconv.encode(str, encoding).length;
    }

    original.BufferToString = Buffer.prototype.toString;
    Buffer.prototype.toString = function(encoding, start, end) {
        encoding = String(encoding || 'utf8').toLowerCase();

        // Use native conversion when possible
        if (Buffer.isNativeEncoding(encoding))
            return original.BufferToString.call(this, encoding, start, end);

        // Otherwise, use our decoding method.
        if (typeof start == 'undefined') start = 0; ...
```
- example usage
```shell
...
'''

### [Deprecated] Extend Node.js own encodings
> NOTE: This doesn't work on latest Node versions. See [details](https://github.com/ashtuchkin/iconv-lite/wiki/Node-v4-compatibility
).

'''javascript
// After this call all Node basic primitives will understand iconv-lite encodings.
iconv.extendNodeEncodings();

// Examples:
buf = new Buffer(str, 'win1251');
buf.write(str, 'gbk');
str = buf.toString('latin1');
assert(Buffer.isEncoding('iso-8859-15'));
Buffer.byteLength(str, 'us-ascii');
...
```

#### <a name="apidoc.element.iconv-lite.fromEncoding"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>fromEncoding (buf, encoding, options)](#apidoc.element.iconv-lite.fromEncoding)
- description and source-code
```javascript
function decode(buf, encoding, options) {
    if (typeof buf === 'string') {
        if (!iconv.skipDecodeWarning) {
            console.error('Iconv-lite warning: decode()-ing strings is deprecated. Refer to https://github.com/ashtuchkin/iconv-
lite/wiki/Use-Buffers-when-decoding');
            iconv.skipDecodeWarning = true;
        }

        buf = new Buffer("" + (buf || ""), "binary"); // Ensure buffer.
    }

    var decoder = iconv.getDecoder(encoding, options);

    var res = decoder.write(buf);
    var trail = decoder.end();

    return trail ? (res + trail) : res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.getCodec"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>getCodec (encoding)](#apidoc.element.iconv-lite.getCodec)
- description and source-code
```javascript
function getCodec(encoding) {
    if (!iconv.encodings)
        iconv.encodings = require("../encodings"); // Lazy load all encoding definitions.

    // Canonicalize encoding name: strip all non-alphanumeric chars and appended year.
    var enc = (''+encoding).toLowerCase().replace(/[^0-9a-z]|:\d{4}$/g, "");

    // Traverse iconv.encodings to find actual codec.
    var codecOptions = {};
    while (true) {
        var codec = iconv._codecDataCache[enc];
        if (codec)
            return codec;

        var codecDef = iconv.encodings[enc];

        switch (typeof codecDef) {
            case "string": // Direct alias to other encoding.
                enc = codecDef;
                break;

            case "object": // Alias with options. Can be layered.
                for (var key in codecDef)
                    codecOptions[key] = codecDef[key];

                if (!codecOptions.encodingName)
                    codecOptions.encodingName = enc;

                enc = codecDef.type;
                break;

            case "function": // Codec itself.
                if (!codecOptions.encodingName)
                    codecOptions.encodingName = enc;

                // The codec function must load all tables and return object with .encoder and .decoder methods.
                // It'll be called only once (for each different options object).
                codec = new codecDef(codecOptions, iconv);

                iconv._codecDataCache[codecOptions.encodingName] = codec; // Save it to be reused later.
                return codec;

            default:
                throw new Error("Encoding not recognized: '" + encoding + "' (searched as: '"+enc+"')");
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.getDecoder"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>getDecoder (encoding, options)](#apidoc.element.iconv-lite.getDecoder)
- description and source-code
```javascript
function getDecoder(encoding, options) {
    var codec = iconv.getCodec(encoding),
        decoder = new codec.decoder(options, codec);

    if (codec.bomAware && !(options && options.stripBOM === false))
        decoder = new bomHandling.StripBOM(decoder, options);

    return decoder;
}
```
- example usage
```shell
...

        if (this.initialBytesLen < 16) // We need more bytes to use space heuristic (see below)
            return '';

        // We have enough bytes -> detect endianness.
        var buf = Buffer.concat(this.initialBytes),
            encoding = detectEncoding(buf, this.options.defaultEncoding);
        this.decoder = this.iconv.getDecoder(encoding, this.options);
        this.initialBytes.length = this.initialBytesLen = 0;
    }

    return this.decoder.write(buf);
}

Utf16Decoder.prototype.end = function() {
...
```

#### <a name="apidoc.element.iconv-lite.getEncoder"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>getEncoder (encoding, options)](#apidoc.element.iconv-lite.getEncoder)
- description and source-code
```javascript
function getEncoder(encoding, options) {
    var codec = iconv.getCodec(encoding),
        encoder = new codec.encoder(options, codec);

    if (codec.bomAware && options && options.addBOM)
        encoder = new bomHandling.PrependBOM(encoder, options);

    return encoder;
}
```
- example usage
```shell
...

// -- Encoding (pass-through)

function Utf16Encoder(options, codec) {
    options = options || {};
    if (options.addBOM === undefined)
        options.addBOM = true;
    this.encoder = codec.iconv.getEncoder('utf-16le', options);
}

Utf16Encoder.prototype.write = function(str) {
    return this.encoder.write(str);
}

Utf16Encoder.prototype.end = function() {
...
```

#### <a name="apidoc.element.iconv-lite.toEncoding"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>toEncoding (str, encoding, options)](#apidoc.element.iconv-lite.toEncoding)
- description and source-code
```javascript
function encode(str, encoding, options) {
    str = "" + (str || ""); // Ensure string.

    var encoder = iconv.getEncoder(encoding, options);

    var res = encoder.write(str);
    var trail = encoder.end();

    return (trail && trail.length > 0) ? Buffer.concat([res, trail]) : res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.undoExtendNodeEncodings"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>undoExtendNodeEncodings ()](#apidoc.element.iconv-lite.undoExtendNodeEncodings)
- description and source-code
```javascript
function undoExtendNodeEncodings() {
    if (!iconv.supportsNodeEncodingsExtension)
        return;
    if (!original)
        throw new Error("require('iconv-lite').undoExtendNodeEncodings(): Nothing to undo; extendNodeEncodings() is not called.")

    delete Buffer.isNativeEncoding;

    var SlowBuffer = require('buffer').SlowBuffer;

    SlowBuffer.prototype.toString = original.SlowBufferToString;
    SlowBuffer.prototype.write = original.SlowBufferWrite;

    Buffer.isEncoding = original.BufferIsEncoding;
    Buffer.byteLength = original.BufferByteLength;
    Buffer.prototype.toString = original.BufferToString;
    Buffer.prototype.write = original.BufferWrite;

    if (iconv.supportsStreams) {
        var Readable = require('stream').Readable;

        Readable.prototype.setEncoding = original.ReadableSetEncoding;
        delete Readable.prototype.collect;
    }

    original = undefined;
}
```
- example usage
```shell
...
request = require('request');
request({
   url: "http://github.com/",
   encoding: "cp932"
});

// To remove extensions
iconv.undoExtendNodeEncodings();
'''

## Supported encodings

*  All node.js native encodings: utf8, ucs2 / utf16-le, ascii, binary, base64, hex.
*  Additional unicode encodings: utf16, utf16-be, utf-7, utf-7-imap.
*  All widespread singlebyte encodings: Windows 125x family, ISO-8859 family,
...
```



# <a name="apidoc.module.iconv-lite.IconvLiteDecoderStream"></a>[module iconv-lite.IconvLiteDecoderStream](#apidoc.module.iconv-lite.IconvLiteDecoderStream)

#### <a name="apidoc.element.iconv-lite.IconvLiteDecoderStream.IconvLiteDecoderStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteDecoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.IconvLiteDecoderStream)
- description and source-code
```javascript
function IconvLiteDecoderStream(conv, options) {
    this.conv = conv;
    options = options || {};
    options.encoding = this.encoding = 'utf8'; // We output strings.
    Transform.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.IconvLiteDecoderStream.prototype"></a>[module iconv-lite.IconvLiteDecoderStream.prototype](#apidoc.module.iconv-lite.IconvLiteDecoderStream.prototype)

#### <a name="apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._flush"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>_flush (done)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._flush)
- description and source-code
```javascript
_flush = function (done) {
    try {
        var res = this.conv.end();
        if (res && res.length) this.push(res, this.encoding);
        done();
    }
    catch (e) {
        done(e);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._transform"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>_transform (chunk, encoding, done)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, done) {
    if (!Buffer.isBuffer(chunk))
        return done(new Error("Iconv decoding stream needs buffers as its input."));
    try {
        var res = this.conv.write(chunk);
        if (res && res.length) this.push(res, this.encoding);
        done();
    }
    catch (e) {
        done(e);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype.collect"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteDecoderStream.prototype.</span>collect (cb)](#apidoc.element.iconv-lite.IconvLiteDecoderStream.prototype.collect)
- description and source-code
```javascript
collect = function (cb) {
    var res = '';
    this.on('error', cb);
    this.on('data', function(chunk) { res += chunk; });
    this.on('end', function() {
        cb(null, res);
    });
    return this;
}
```
- example usage
```shell
...

// Convert encoding streaming example
fs.createReadStream('file-in-win1251.txt')
    .pipe(iconv.decodeStream('win1251'))
    .pipe(iconv.encodeStream('ucs2'))
    .pipe(fs.createWriteStream('file-in-ucs2.txt'));

// Sugar: all encode/decode streams have .collect(cb) method to accumulate data.
http.createServer(function(req, res) {
    req.pipe(iconv.decodeStream('win1251')).collect(function(err, body) {
        assert(typeof body == 'string');
        console.log(body); // full request body string
    });
});
'''
...
```



# <a name="apidoc.module.iconv-lite.IconvLiteEncoderStream"></a>[module iconv-lite.IconvLiteEncoderStream](#apidoc.module.iconv-lite.IconvLiteEncoderStream)

#### <a name="apidoc.element.iconv-lite.IconvLiteEncoderStream.IconvLiteEncoderStream"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>IconvLiteEncoderStream (conv, options)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.IconvLiteEncoderStream)
- description and source-code
```javascript
function IconvLiteEncoderStream(conv, options) {
    this.conv = conv;
    options = options || {};
    options.decodeStrings = false; // We accept only strings, so we don't need to decode them.
    Transform.call(this, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.IconvLiteEncoderStream.prototype"></a>[module iconv-lite.IconvLiteEncoderStream.prototype](#apidoc.module.iconv-lite.IconvLiteEncoderStream.prototype)

#### <a name="apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._flush"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>_flush (done)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._flush)
- description and source-code
```javascript
_flush = function (done) {
    try {
        var res = this.conv.end();
        if (res && res.length) this.push(res);
        done();
    }
    catch (e) {
        done(e);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._transform"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>_transform (chunk, encoding, done)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, done) {
    if (typeof chunk != 'string')
        return done(new Error("Iconv encoding stream needs strings as its input."));
    try {
        var res = this.conv.write(chunk);
        if (res && res.length) this.push(res);
        done();
    }
    catch (e) {
        done(e);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype.collect"></a>[function <span class="apidocSignatureSpan">iconv-lite.IconvLiteEncoderStream.prototype.</span>collect (cb)](#apidoc.element.iconv-lite.IconvLiteEncoderStream.prototype.collect)
- description and source-code
```javascript
collect = function (cb) {
    var chunks = [];
    this.on('error', cb);
    this.on('data', function(chunk) { chunks.push(chunk); });
    this.on('end', function() {
        cb(null, Buffer.concat(chunks));
    });
    return this;
}
```
- example usage
```shell
...

// Convert encoding streaming example
fs.createReadStream('file-in-win1251.txt')
    .pipe(iconv.decodeStream('win1251'))
    .pipe(iconv.encodeStream('ucs2'))
    .pipe(fs.createWriteStream('file-in-ucs2.txt'));

// Sugar: all encode/decode streams have .collect(cb) method to accumulate data.
http.createServer(function(req, res) {
    req.pipe(iconv.decodeStream('win1251')).collect(function(err, body) {
        assert(typeof body == 'string');
        console.log(body); // full request body string
    });
});
'''
...
```



# <a name="apidoc.module.iconv-lite.bom_handling"></a>[module iconv-lite.bom_handling](#apidoc.module.iconv-lite.bom_handling)

#### <a name="apidoc.element.iconv-lite.bom_handling.PrependBOM"></a>[function <span class="apidocSignatureSpan">iconv-lite.bom_handling.</span>PrependBOM (encoder, options)](#apidoc.element.iconv-lite.bom_handling.PrependBOM)
- description and source-code
```javascript
function PrependBOMWrapper(encoder, options) {
    this.encoder = encoder;
    this.addBOM = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.bom_handling.StripBOM"></a>[function <span class="apidocSignatureSpan">iconv-lite.bom_handling.</span>StripBOM (decoder, options)](#apidoc.element.iconv-lite.bom_handling.StripBOM)
- description and source-code
```javascript
function StripBOMWrapper(decoder, options) {
    this.decoder = decoder;
    this.pass = false;
    this.options = options || {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.dbcs_codec"></a>[module iconv-lite.dbcs_codec](#apidoc.module.iconv-lite.dbcs_codec)

#### <a name="apidoc.element.iconv-lite.dbcs_codec._dbcs"></a>[function <span class="apidocSignatureSpan">iconv-lite.dbcs_codec.</span>_dbcs (codecOptions, iconv)](#apidoc.element.iconv-lite.dbcs_codec._dbcs)
- description and source-code
```javascript
function DBCSCodec(codecOptions, iconv) {
    this.encodingName = codecOptions.encodingName;
    if (!codecOptions)
        throw new Error("DBCS codec is called without the data.")
    if (!codecOptions.table)
        throw new Error("Encoding '" + this.encodingName + "' has no data.");

    // Load tables.
    var mappingTable = codecOptions.table();


    // Decode tables: MBCS -> Unicode.

    // decodeTables is a trie, encoded as an array of arrays of integers. Internal arrays are trie nodes and all have len = 256.
    // Trie root is decodeTables[0].
    // Values: >=  0 -> unicode character code. can be > 0xFFFF
    //         == UNASSIGNED -> unknown/unassigned sequence.
    //         == GB18030_CODE -> this is the end of a GB18030 4-byte sequence.
    //         <= NODE_START -> index of the next node in our trie to process next byte.
    //         <= SEQ_START  -> index of the start of a character code sequence, in decodeTableSeq.
    this.decodeTables = [];
    this.decodeTables[0] = UNASSIGNED_NODE.slice(0); // Create root node.

    // Sometimes a MBCS char corresponds to a sequence of unicode chars. We store them as arrays of integers here.
    this.decodeTableSeq = [];

    // Actual mapping tables consist of chunks. Use them to fill up decode tables.
    for (var i = 0; i < mappingTable.length; i++)
        this._addDecodeChunk(mappingTable[i]);

    this.defaultCharUnicode = iconv.defaultCharUnicode;


    // Encode tables: Unicode -> DBCS.

    // 'encodeTable' is array mapping from unicode char to encoded char. All its values are integers for performance.
    // Because it can be sparse, it is represented as array of buckets by 256 chars each. Bucket can be null.
    // Values: >=  0 -> it is a normal char. Write the value (if <=256 then 1 byte, if <=65536 then 2 bytes, etc.).
    //         == UNASSIGNED -> no conversion found. Output a default char.
    //         <= SEQ_START  -> it's an index in encodeTableSeq, see below. The character starts a sequence.
    this.encodeTable = [];

    // 'encodeTableSeq' is used when a sequence of unicode characters is encoded as a single code. We use a tree of
    // objects where keys correspond to characters in sequence and leafs are the encoded dbcs values. A special DEF_CHAR key
    // means end of sequence (needed when one sequence is a strict subsequence of another).
    // Objects are kept separately from encodeTable to increase performance.
    this.encodeTableSeq = [];

    // Some chars can be decoded, but need not be encoded.
    var skipEncodeChars = {};
    if (codecOptions.encodeSkipVals)
        for (var i = 0; i < codecOptions.encodeSkipVals.length; i++) {
            var val = codecOptions.encodeSkipVals[i];
            if (typeof val === 'number')
                skipEncodeChars[val] = true;
            else
                for (var j = val.from; j <= val.to; j++)
                    skipEncodeChars[j] = true;
        }

    // Use decode trie to recursively fill out encode tables.
    this._fillEncodeTable(0, 0, skipEncodeChars);

    // Add more encoding pairs when needed.
    if (codecOptions.encodeAdd) {
        for (var uChar in codecOptions.encodeAdd)
            if (Object.prototype.hasOwnProperty.call(codecOptions.encodeAdd, uChar))
                this._setEncodeChar(uChar.charCodeAt(0), codecOptions.encodeAdd[uChar]);
    }

    this.defCharSB  = this.encodeTable[0][iconv.defaultCharSingleByte.charCodeAt(0)];
    if (this.defCharSB === UNASSIGNED) this.defCharSB = this.encodeTable[0]['?'];
    if (this.defCharSB === UNASSIGNED) this.defCharSB = "?".charCodeAt(0);


    // Load & create GB18030 tables when needed.
    if (typeof codecOptions.gb18030 === 'function') {
        this.gb18030 = codecOptions.gb18030(); // Load GB18030 ranges.

        // Add GB18030 decode tables.
        var thirdByteNodeIdx = this.decodeTables.length;
        var thirdByteNode = this.decodeTables[thirdByteNodeIdx] = UNASSIGNED_NODE.slice(0);

        var fourthByteNodeIdx = this.decodeTables.length;
        var fourthByteNode = this.decod ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.internal"></a>[module iconv-lite.internal](#apidoc.module.iconv-lite.internal)

#### <a name="apidoc.element.iconv-lite.internal._internal"></a>[function <span class="apidocSignatureSpan">iconv-lite.internal.</span>_internal (codecOptions, iconv)](#apidoc.element.iconv-lite.internal._internal)
- description and source-code
```javascript
function InternalCodec(codecOptions, iconv) {
    this.enc = codecOptions.encodingName;
    this.bomAware = codecOptions.bomAware;

    if (this.enc === "base64")
        this.encoder = InternalEncoderBase64;
    else if (this.enc === "cesu8") {
        this.enc = "utf8"; // Use utf8 for decoding.
        this.encoder = InternalEncoderCesu8;

        // Add decoder for versions of Node not supporting CESU-8
        if (new Buffer("eda080", 'hex').toString().length == 3) {
            this.decoder = InternalDecoderCesu8;
            this.defaultCharUnicode = iconv.defaultCharUnicode;
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.sbcs_codec"></a>[module iconv-lite.sbcs_codec](#apidoc.module.iconv-lite.sbcs_codec)

#### <a name="apidoc.element.iconv-lite.sbcs_codec._sbcs"></a>[function <span class="apidocSignatureSpan">iconv-lite.sbcs_codec.</span>_sbcs (codecOptions, iconv)](#apidoc.element.iconv-lite.sbcs_codec._sbcs)
- description and source-code
```javascript
function SBCSCodec(codecOptions, iconv) {
    if (!codecOptions)
        throw new Error("SBCS codec is called without the data.")

    // Prepare char buffer for decoding.
    if (!codecOptions.chars || (codecOptions.chars.length !== 128 && codecOptions.chars.length !== 256))
        throw new Error("Encoding '"+codecOptions.type+"' has incorrect 'chars' (must be of len 128 or 256)");

    if (codecOptions.chars.length === 128) {
        var asciiString = "";
        for (var i = 0; i < 128; i++)
            asciiString += String.fromCharCode(i);
        codecOptions.chars = asciiString + codecOptions.chars;
    }

    this.decodeBuf = new Buffer(codecOptions.chars, 'ucs2');

    // Encoding buffer.
    var encodeBuf = new Buffer(65536);
    encodeBuf.fill(iconv.defaultCharSingleByte.charCodeAt(0));

    for (var i = 0; i < codecOptions.chars.length; i++)
        encodeBuf[codecOptions.chars.charCodeAt(i)] = i;

    this.encodeBuf = encodeBuf;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.utf16"></a>[module iconv-lite.utf16](#apidoc.module.iconv-lite.utf16)

#### <a name="apidoc.element.iconv-lite.utf16.utf16"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>utf16 (codecOptions, iconv)](#apidoc.element.iconv-lite.utf16.utf16)
- description and source-code
```javascript
function Utf16Codec(codecOptions, iconv) {
    this.iconv = iconv;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.utf16.utf16be"></a>[function <span class="apidocSignatureSpan">iconv-lite.utf16.</span>utf16be ()](#apidoc.element.iconv-lite.utf16.utf16be)
- description and source-code
```javascript
function Utf16BECodec() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.iconv-lite.utf7"></a>[module iconv-lite.utf7](#apidoc.module.iconv-lite.utf7)

#### <a name="apidoc.element.iconv-lite.utf7.utf7"></a>[function <span class="apidocSignatureSpan">iconv-lite.</span>utf7 (codecOptions, iconv)](#apidoc.element.iconv-lite.utf7.utf7)
- description and source-code
```javascript
function Utf7Codec(codecOptions, iconv) {
    this.iconv = iconv;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.iconv-lite.utf7.utf7imap"></a>[function <span class="apidocSignatureSpan">iconv-lite.utf7.</span>utf7imap (codecOptions, iconv)](#apidoc.element.iconv-lite.utf7.utf7imap)
- description and source-code
```javascript
function Utf7IMAPCodec(codecOptions, iconv) {
    this.iconv = iconv;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
