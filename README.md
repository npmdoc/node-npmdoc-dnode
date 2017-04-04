# api documentation for  [dnode (v1.2.2)](https://github.com/substack/dnode#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-dnode.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-dnode) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-dnode.svg)](https://travis-ci.org/npmdoc/node-npmdoc-dnode)
#### freestyle rpc

[![NPM](https://nodei.co/npm/dnode.png?downloads=true)](https://www.npmjs.com/package/dnode)

[![apidoc](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-dnode_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-dnode/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-dnode/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "email": "mail@substack.net",
        "url": "http://substack.net"
    },
    "browserify": "browser.js",
    "bugs": {
        "url": "https://github.com/substack/dnode/issues"
    },
    "dependencies": {
        "dnode-protocol": "~0.2.2",
        "jsonify": "~0.0.0",
        "weak": "^1.0.0"
    },
    "description": "freestyle rpc",
    "devDependencies": {
        "tape": "~2.3.2"
    },
    "directories": {},
    "dist": {
        "shasum": "4ac3cfe26e292b3b39b8258ae7d94edc58132efa",
        "tarball": "https://registry.npmjs.org/dnode/-/dnode-1.2.2.tgz"
    },
    "engine": {
        "node": ">=0.6.0"
    },
    "gitHead": "32e8a7e36f4603672b17fa4b0fbecc05c66022df",
    "homepage": "https://github.com/substack/dnode#readme",
    "keywords": [
        "rpc",
        "callbacks"
    ],
    "main": "./index.js",
    "maintainers": [
        {
            "name": "substack",
            "email": "substack@gmail.com"
        },
        {
            "name": "seethroughtrees",
            "email": "seethroughtrees+npm@gmail.com"
        }
    ],
    "name": "dnode",
    "optionalDependencies": {
        "weak": "^1.0.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/substack/dnode.git"
    },
    "scripts": {
        "test": "tape test/*.js test/server/*.js"
    },
    "testling": {
        "files": "test/*.js",
        "browsers": [
            "ie/6..latest",
            "chrome/10",
            "chrome/latest",
            "chrome/canary",
            "firefox/10",
            "firefox/latest",
            "firefox/nightly",
            "safari/latest",
            "opera/11.0..latest",
            "iphone/6",
            "ipad/6",
            "android-browser/latest"
        ]
    },
    "version": "1.2.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module dnode](#apidoc.module.dnode)
1.  [function <span class="apidocSignatureSpan"></span>dnode (cons, opts)](#apidoc.element.dnode.dnode)
1.  [function <span class="apidocSignatureSpan">dnode.</span>connect ()](#apidoc.element.dnode.connect)
1.  [function <span class="apidocSignatureSpan">dnode.</span>listen ()](#apidoc.element.dnode.listen)
1.  object <span class="apidocSignatureSpan">dnode.</span>dnode.prototype

#### [module dnode.dnode](#apidoc.module.dnode.dnode)
1.  [function <span class="apidocSignatureSpan">dnode.</span>dnode (cons, opts)](#apidoc.element.dnode.dnode.dnode)

#### [module dnode.dnode.prototype](#apidoc.module.dnode.dnode.prototype)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>_createProto ()](#apidoc.element.dnode.dnode.prototype._createProto)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>addListener (type, listener)](#apidoc.element.dnode.dnode.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>destroy ()](#apidoc.element.dnode.dnode.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>emit (type)](#apidoc.element.dnode.dnode.prototype.emit)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>end ()](#apidoc.element.dnode.dnode.prototype.end)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>eventNames ()](#apidoc.element.dnode.dnode.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>getMaxListeners ()](#apidoc.element.dnode.dnode.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>handle (row)](#apidoc.element.dnode.dnode.prototype.handle)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listen ()](#apidoc.element.dnode.dnode.prototype.listen)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listenerCount (type)](#apidoc.element.dnode.dnode.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listeners (type)](#apidoc.element.dnode.dnode.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>on (type, listener)](#apidoc.element.dnode.dnode.prototype.on)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>once (type, listener)](#apidoc.element.dnode.dnode.prototype.once)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>pipe (dest, options)](#apidoc.element.dnode.dnode.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>prependListener (type, listener)](#apidoc.element.dnode.dnode.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.dnode.dnode.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>removeAllListeners (type)](#apidoc.element.dnode.dnode.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>removeListener (type, listener)](#apidoc.element.dnode.dnode.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>setMaxListeners (n)](#apidoc.element.dnode.dnode.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>write (buf)](#apidoc.element.dnode.dnode.prototype.write)
1.  undefined <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>domain



# <a name="apidoc.module.dnode"></a>[module dnode](#apidoc.module.dnode)

#### <a name="apidoc.element.dnode.dnode"></a>[function <span class="apidocSignatureSpan"></span>dnode (cons, opts)](#apidoc.element.dnode.dnode)
- description and source-code
```javascript
function dnode(cons, opts) {
    Stream.call(this);
    var self = this;

    self.opts = opts || {};

    self.cons = typeof cons === 'function'
        ? cons
        : function () { return cons || {} }
    ;

    self.readable = true;
    self.writable = true;

    process.nextTick(function () {
        if (self._ended) return;
        self.proto = self._createProto();
        self.proto.start();

        if (!self._handleQueue) return;
        for (var i = 0; i < self._handleQueue.length; i++) {
            self.handle(self._handleQueue[i]);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.connect"></a>[function <span class="apidocSignatureSpan">dnode.</span>connect ()](#apidoc.element.dnode.connect)
- description and source-code
```javascript
connect = function () {
    var d = new D();
    return d.connect.apply(d, arguments);
}
```
- example usage
```shell
...

D.prototype.connect = function () {
var self = this;
var params = parseArgs(arguments);

var stream;
if (params.path) {
    stream = net.connect(params.path);
}
else if (params.port) {
    stream = net.connect(params.port, params.host);
}
else {
    throw new Error('no port or unix path given');
}
...
```

#### <a name="apidoc.element.dnode.listen"></a>[function <span class="apidocSignatureSpan">dnode.</span>listen ()](#apidoc.element.dnode.listen)
- description and source-code
```javascript
listen = function () {
    var d = new D();
    return d.listen.apply(d, arguments);
}
```
- example usage
```shell
...
    stream.pipe(d);
    d.pipe(stream);
});

server.sessions = {};

if (typeof params.port === 'number' && params.port >= 0) {
    server.listen(params.port, params.host);
}
else if (params.path) {
    server.listen(params.path);
}
else {
    throw new Error('no port or path provided');
}
...
```



# <a name="apidoc.module.dnode.dnode"></a>[module dnode.dnode](#apidoc.module.dnode.dnode)

#### <a name="apidoc.element.dnode.dnode.dnode"></a>[function <span class="apidocSignatureSpan">dnode.</span>dnode (cons, opts)](#apidoc.element.dnode.dnode.dnode)
- description and source-code
```javascript
function dnode(cons, opts) {
    Stream.call(this);
    var self = this;

    self.opts = opts || {};

    self.cons = typeof cons === 'function'
        ? cons
        : function () { return cons || {} }
    ;

    self.readable = true;
    self.writable = true;

    process.nextTick(function () {
        if (self._ended) return;
        self.proto = self._createProto();
        self.proto.start();

        if (!self._handleQueue) return;
        for (var i = 0; i < self._handleQueue.length; i++) {
            self.handle(self._handleQueue[i]);
        }
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dnode.dnode.prototype"></a>[module dnode.dnode.prototype](#apidoc.module.dnode.dnode.prototype)

#### <a name="apidoc.element.dnode.dnode.prototype._createProto"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>_createProto ()](#apidoc.element.dnode.dnode.prototype._createProto)
- description and source-code
```javascript
_createProto = function () {
    var self = this;
    var proto = protocol(function (remote) {
        if (self._ended) return;

        var ref = self.cons.call(this, remote, self);
        if (typeof ref !== 'object') ref = this;

        self.emit('local', ref, self);

        return ref;
    }, self.opts.proto);

    proto.on('remote', function (remote) {
        self.emit('remote', remote, self);
        self.emit('ready'); // backwards compatability, deprecated
    });

    proto.on('request', function (req) {
        if (!self.readable) return;

        if (self.opts.emit === 'object') {
            self.emit('data', req);
        }
        else self.emit('data', json.stringify(req) + '\n');
    });

    proto.on('fail', function (err) {
        // errors that the remote end was responsible for
        self.emit('fail', err);
    });

    proto.on('error', function (err) {
        // errors that the local code was responsible for
        self.emit('error', err);
    });

    return proto;
}
```
- example usage
```shell
...
;

self.readable = true;
self.writable = true;

process.nextTick(function () {
    if (self._ended) return;
    self.proto = self._createProto();
    self.proto.start();

    if (!self._handleQueue) return;
    for (var i = 0; i < self._handleQueue.length; i++) {
        self.handle(self._handleQueue[i]);
    }
});
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.addListener"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>addListener (type, listener)](#apidoc.element.dnode.dnode.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.destroy"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>destroy ()](#apidoc.element.dnode.dnode.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
    this.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.emit"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>emit (type)](#apidoc.element.dnode.dnode.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
    throw new Error('no port or unix path given');
}

if (params.block) self.on('remote', params.block);

stream.on('error', function (err) {
    if (err && err.code === 'EPIPE') return; // eat EPIPEs
    self.emit('error', err);
});

self.id = randomId();
self.stream = stream;
stream.pipe(self);
self.pipe(stream);
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.end"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>end ()](#apidoc.element.dnode.dnode.prototype.end)
- description and source-code
```javascript
end = function () {
    if (this._ended) return;
    this._ended = true;
    this.writable = false;
    this.readable = false;
    this.emit('end');
}
```
- example usage
```shell
...

dnode.prototype.listen = function () {
var self = this;

// just copy over the opts and cons, the rest will need to be re-created
var cons = self.cons, opts = self.opts;
self.cons = function () {};
self.end();

var params = parseArgs(arguments);

var server = net.createServer(function (stream) {
    var d = new dnode(cons, opts);
    do { d.id = randomId() }
    while (server.sessions[d.id]);
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>eventNames ()](#apidoc.element.dnode.dnode.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>getMaxListeners ()](#apidoc.element.dnode.dnode.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.handle"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>handle (row)](#apidoc.element.dnode.dnode.prototype.handle)
- description and source-code
```javascript
handle = function (row) {
    if (!this.proto) {
        if (!this._handleQueue) this._handleQueue = [];
        this._handleQueue.push(row);
    }
    else this.proto.handle(row);
}
```
- example usage
```shell
...
process.nextTick(function () {
    if (self._ended) return;
    self.proto = self._createProto();
    self.proto.start();

    if (!self._handleQueue) return;
    for (var i = 0; i < self._handleQueue.length; i++) {
        self.handle(self._handleQueue[i]);
    }
});
}

dnode.prototype._createProto = function () {
var self = this;
var proto = protocol(function (remote) {
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.listen"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listen ()](#apidoc.element.dnode.dnode.prototype.listen)
- description and source-code
```javascript
listen = function () {
    var self = this;

    // just copy over the opts and cons, the rest will need to be re-created
    var cons = self.cons, opts = self.opts;
    self.cons = function () {};
    self.end();

    var params = parseArgs(arguments);

    var server = net.createServer(function (stream) {
        var d = new dnode(cons, opts);
        do { d.id = randomId() }
        while (server.sessions[d.id]);

        server.sessions[d.id] = d;
        d.on('end', function () {
            delete server.sessions[d.id];
        });

        d.on('local', function (ref) {
            server.emit('local', ref, d);
        });

        d.on('remote', function (remote) {
            server.emit('remote', remote, d);
        });

        stream.on('error', function (err) {
            if (err && err.code === 'EPIPE') return; // eat EPIPEs
            d.emit('error', err);
        });

        d.stream = stream;
        stream.pipe(d);
        d.pipe(stream);
    });

    server.sessions = {};

    if (typeof params.port === 'number' && params.port >= 0) {
        server.listen(params.port, params.host);
    }
    else if (params.path) {
        server.listen(params.path);
    }
    else {
        throw new Error('no port or path provided');
    }

    if (params.block) server.on('listening', params.block);

    return server;
}
```
- example usage
```shell
...
    stream.pipe(d);
    d.pipe(stream);
});

server.sessions = {};

if (typeof params.port === 'number' && params.port >= 0) {
    server.listen(params.port, params.host);
}
else if (params.path) {
    server.listen(params.path);
}
else {
    throw new Error('no port or path provided');
}
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listenerCount (type)](#apidoc.element.dnode.dnode.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.listeners"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>listeners (type)](#apidoc.element.dnode.dnode.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.on"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>on (type, listener)](#apidoc.element.dnode.dnode.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
else if (params.port) {
    stream = net.connect(params.port, params.host);
}
else {
    throw new Error('no port or unix path given');
}

if (params.block) self.on('remote', params.block);

stream.on('error', function (err) {
    if (err && err.code === 'EPIPE') return; // eat EPIPEs
    self.emit('error', err);
});

self.id = randomId();
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.once"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>once (type, listener)](#apidoc.element.dnode.dnode.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.pipe"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>pipe (dest, options)](#apidoc.element.dnode.dnode.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, options) {
  var source = this;

  function ondata(chunk) {
    if (dest.writable) {
      if (false === dest.write(chunk) && source.pause) {
        source.pause();
      }
    }
  }

  source.on('data', ondata);

  function ondrain() {
    if (source.readable && source.resume) {
      source.resume();
    }
  }

  dest.on('drain', ondrain);

  // If the 'end' option is not supplied, dest.end() will be called when
  // source gets the 'end' or 'close' events.  Only dest.end() once.
  if (!dest._isStdio && (!options || options.end !== false)) {
    source.on('end', onend);
    source.on('close', onclose);
  }

  var didOnEnd = false;
  function onend() {
    if (didOnEnd) return;
    didOnEnd = true;

    dest.end();
  }


  function onclose() {
    if (didOnEnd) return;
    didOnEnd = true;

    if (typeof dest.destroy === 'function') dest.destroy();
  }

  // don't leave dangling pipes when there are errors.
  function onerror(er) {
    cleanup();
    if (EE.listenerCount(this, 'error') === 0) {
      throw er; // Unhandled stream error in pipe.
    }
  }

  source.on('error', onerror);
  dest.on('error', onerror);

  // remove all the event listeners that were added.
  function cleanup() {
    source.removeListener('data', ondata);
    dest.removeListener('drain', ondrain);

    source.removeListener('end', onend);
    source.removeListener('close', onclose);

    source.removeListener('error', onerror);
    dest.removeListener('error', onerror);

    source.removeListener('end', cleanup);
    source.removeListener('close', cleanup);

    dest.removeListener('close', cleanup);
  }

  source.on('end', cleanup);
  source.on('close', cleanup);

  dest.on('close', cleanup);
  dest.emit('pipe', source);

  // Allow for unix-like usage: A.pipe(B).pipe(C)
  return dest;
}
```
- example usage
```shell
...
stream.on('error', function (err) {
    if (err && err.code === 'EPIPE') return; // eat EPIPEs
    self.emit('error', err);
});

self.id = randomId();
self.stream = stream;
stream.pipe(self);
self.pipe(stream);

return self;
};

dnode.prototype.listen = function () {
var self = this;
...
```

#### <a name="apidoc.element.dnode.dnode.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>prependListener (type, listener)](#apidoc.element.dnode.dnode.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.dnode.dnode.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>removeAllListeners (type)](#apidoc.element.dnode.dnode.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>removeListener (type, listener)](#apidoc.element.dnode.dnode.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>setMaxListeners (n)](#apidoc.element.dnode.dnode.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dnode.dnode.prototype.write"></a>[function <span class="apidocSignatureSpan">dnode.dnode.prototype.</span>write (buf)](#apidoc.element.dnode.dnode.prototype.write)
- description and source-code
```javascript
write = function (buf) {
    if (this._ended) return;
    var self = this;
    var row;

    if (buf && typeof buf === 'object'
    && buf.constructor && buf.constructor.name === 'Buffer'
    && buf.length
    && typeof buf.slice === 'function') {
        // treat like a buffer
        if (!self._bufs) self._bufs = [];

        // treat like a buffer
        for (var i = 0, j = 0; i < buf.length; i++) {
            if (buf[i] === 0x0a) {
                self._bufs.push(buf.slice(j, i));

                var line = '';
                for (var k = 0; k < self._bufs.length; k++) {
                    line += String(self._bufs[k]);
                }

                try { row = json.parse(line) }
                catch (err) { return self.end() }

                j = i + 1;

                self.handle(row);
                self._bufs = [];
            }
        }

        if (j < buf.length) self._bufs.push(buf.slice(j, buf.length));
    }
    else if (buf && typeof buf === 'object') {
        // .isBuffer() without the Buffer
        // Use self to pipe JSONStream.parse() streams.
        self.handle(buf);
    }
    else {
        if (typeof buf !== 'string') buf = String(buf);
        if (!self._line) self._line = '';

        for (var i = 0; i < buf.length; i++) {
            if (buf.charCodeAt(i) === 0x0a) {
                try { row = json.parse(self._line) }
                catch (err) { return self.end() }

                self._line = '';
                self.handle(row);
            }
            else self._line += buf.charAt(i)
        }
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
