# api documentation for  [iconv-lite (v0.4.15)](https://github.com/ashtuchkin/iconv-lite)  [![npm package](https://img.shields.io/npm/v/npmdoc-iconv-lite.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-iconv-lite) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-iconv-lite.svg)](https://travis-ci.org/npmdoc/node-npmdoc-iconv-lite)
#### Convert character encodings in pure javascript.

[![NPM](https://nodei.co/npm/iconv-lite.png?downloads=true)](https://www.npmjs.com/package/iconv-lite)

[![apidoc](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-iconv-lite_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-iconv-lite/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-iconv-lite/build/screen-capture.npmPackageListing.svg)



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
1.  object <span class="apidocSignatureSpan">iconv-lite.</span>encodings
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
    if (iconv.supportsStreams) {
        var Readable = require('stream').Readable;

        original.ReadableSetEncoding = Readable.prototype.setEncoding;
        Readable.prototype.setEncoding = function setEncoding(enc, options) {
            // Use our own decoder, it has the same interface.
            // We cannot use original function as it doesn't handle BOM-s.
            this._readableState.decoder = iconv.getDecoder(enc, options);
            this._readableState.encoding = enc;
        }

        Readable.prototype.collect = iconv._collect;
    }
}
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


// == Exports ==================================================================
module.exports = function(iconv) {

// Additional Public API.
iconv.encodeStream = function encodeStream(encoding, options) {
    return new IconvLiteEncoderStream(iconv.getEncoder(encoding, options), options);
}

iconv.decodeStream = function decodeStream(encoding, options) {
    return new IconvLiteDecoderStream(iconv.getDecoder(encoding, options), options);
}

iconv.supportsStreams = true;
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



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
