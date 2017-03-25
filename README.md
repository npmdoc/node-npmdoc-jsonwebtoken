# api documentation for  [jsonwebtoken (v7.3.0)](https://github.com/auth0/node-jsonwebtoken#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jsonwebtoken.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jsonwebtoken)
#### JSON Web Token implementation (symmetric and asymmetric)

[![NPM](https://nodei.co/npm/jsonwebtoken.png?downloads=true)](https://www.npmjs.com/package/jsonwebtoken)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jsonwebtoken/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jsonwebtoken_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jsonwebtoken/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-jsonwebtoken/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "auth0"
    },
    "bugs": {
        "url": "https://github.com/auth0/node-jsonwebtoken/issues"
    },
    "dependencies": {
        "joi": "^6.10.1",
        "jws": "^3.1.4",
        "lodash.once": "^4.0.0",
        "ms": "^0.7.1",
        "xtend": "^4.0.1"
    },
    "description": "JSON Web Token implementation (symmetric and asymmetric)",
    "devDependencies": {
        "atob": "^1.1.2",
        "chai": "^1.10.0",
        "conventional-changelog": "~1.1.0",
        "mocha": "^2.1.0",
        "nsp": "^2.6.2",
        "sinon": "^1.15.4"
    },
    "directories": {},
    "dist": {
        "shasum": "85118d6a70e3fccdf14389f4e7a1c3f9c8a9fbba",
        "tarball": "https://registry.npmjs.org/jsonwebtoken/-/jsonwebtoken-7.3.0.tgz"
    },
    "engines": {
        "node": ">=0.12",
        "npm": ">=1.4.28"
    },
    "gitHead": "94007b3e17accb8f0d74f94c2926fdc8924f82b6",
    "homepage": "https://github.com/auth0/node-jsonwebtoken#readme",
    "keywords": [
        "jwt"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "dschenkelman",
            "email": "damian.schenkelman@gmail.com"
        },
        {
            "name": "iaco",
            "email": "sebastian.iacomuzzi@gmail.com"
        },
        {
            "name": "jaredhanson",
            "email": "jaredhanson@gmail.com"
        },
        {
            "name": "jfromaniello",
            "email": "jfromaniello@gmail.com"
        },
        {
            "name": "pose",
            "email": "albertopose@gmail.com"
        },
        {
            "name": "rolodato",
            "email": "rolodato@rolodato.com"
        },
        {
            "name": "woloski",
            "email": "matiasw@gmail.com"
        },
        {
            "name": "ziluvatar",
            "email": "eduardo.diaz@auth0.com"
        }
    ],
    "name": "jsonwebtoken",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/auth0/node-jsonwebtoken.git"
    },
    "scripts": {
        "test": "mocha --require test/util/fakeDate && nsp check"
    },
    "version": "7.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jsonwebtoken](#apidoc.module.jsonwebtoken)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>JsonWebTokenError (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>NotBeforeError (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>TokenExpiredError (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>decode (jwt, options)](#apidoc.element.jsonwebtoken.decode)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>sign (payload, secretOrPrivateKey, options, callback)](#apidoc.element.jsonwebtoken.sign)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>verify (jwtString, secretOrPublicKey, options, callback)](#apidoc.element.jsonwebtoken.verify)
1.  object <span class="apidocSignatureSpan">jsonwebtoken.</span>JsonWebTokenError.prototype
1.  object <span class="apidocSignatureSpan">jsonwebtoken.</span>NotBeforeError.prototype
1.  object <span class="apidocSignatureSpan">jsonwebtoken.</span>TokenExpiredError.prototype

#### [module jsonwebtoken.JsonWebTokenError](#apidoc.module.jsonwebtoken.JsonWebTokenError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>JsonWebTokenError (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError.JsonWebTokenError)

#### [module jsonwebtoken.JsonWebTokenError.prototype](#apidoc.module.jsonwebtoken.JsonWebTokenError.prototype)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.JsonWebTokenError.prototype.</span>constructor (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError.prototype.constructor)

#### [module jsonwebtoken.NotBeforeError](#apidoc.module.jsonwebtoken.NotBeforeError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>NotBeforeError (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError.NotBeforeError)

#### [module jsonwebtoken.NotBeforeError.prototype](#apidoc.module.jsonwebtoken.NotBeforeError.prototype)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.NotBeforeError.prototype.</span>constructor (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError.prototype.constructor)

#### [module jsonwebtoken.TokenExpiredError](#apidoc.module.jsonwebtoken.TokenExpiredError)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.</span>TokenExpiredError (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError.TokenExpiredError)

#### [module jsonwebtoken.TokenExpiredError.prototype](#apidoc.module.jsonwebtoken.TokenExpiredError.prototype)
1.  [function <span class="apidocSignatureSpan">jsonwebtoken.TokenExpiredError.prototype.</span>constructor (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError.prototype.constructor)



# <a name="apidoc.module.jsonwebtoken"></a>[module jsonwebtoken](#apidoc.module.jsonwebtoken)

#### <a name="apidoc.element.jsonwebtoken.JsonWebTokenError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>JsonWebTokenError (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError)
- description and source-code
```javascript
JsonWebTokenError = function (message, error) {
  Error.call(this, message);
  Error.captureStackTrace(this, this.constructor);
  this.name = 'JsonWebTokenError';
  this.message = message;
  if (error) this.inner = error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsonwebtoken.NotBeforeError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>NotBeforeError (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError)
- description and source-code
```javascript
NotBeforeError = function (message, date) {
  JsonWebTokenError.call(this, message);
  this.name = 'NotBeforeError';
  this.date = date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsonwebtoken.TokenExpiredError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>TokenExpiredError (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError)
- description and source-code
```javascript
TokenExpiredError = function (message, expiredAt) {
  JsonWebTokenError.call(this, message);
  this.name = 'TokenExpiredError';
  this.expiredAt = expiredAt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsonwebtoken.decode"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>decode (jwt, options)](#apidoc.element.jsonwebtoken.decode)
- description and source-code
```javascript
decode = function (jwt, options) {
  options = options || {};
  var decoded = jws.decode(jwt, options);
  if (!decoded) { return null; }
  var payload = decoded.payload;

  //try parse the payload
  if(typeof payload === 'string') {
    try {
      var obj = JSON.parse(payload);
      if(typeof obj === 'object') {
        payload = obj;
      }
    } catch (e) { }
  }

  //return header if 'complete' option is enabled.  header includes claims
  //such as 'kid' and 'alg' used to select the key within a JWKS needed to
  //verify the signature
  if (options.complete === true) {
    return {
      header: decoded.header,
      payload: payload,
      signature: decoded.signature
    };
  }
  return payload;
}
```
- example usage
```shell
...
var cert = fs.readFileSync('public.pem'); // get public key
jwt.verify(token, cert, { algorithms: ['RS256'] }, function (err, payload) {
  // if token alg != RS256,  err == invalid signature
});

'''

### jwt.decode(token [, options])

(Synchronous) Returns the decoded payload without verifying if the signature is valid.

__Warning:__ This will __not__ verify whether the signature is valid. You should __not__ use this for untrusted messages. You most
 likely want to use 'jwt.verify' instead.

'token' is the JsonWebToken string
...
```

#### <a name="apidoc.element.jsonwebtoken.sign"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>sign (payload, secretOrPrivateKey, options, callback)](#apidoc.element.jsonwebtoken.sign)
- description and source-code
```javascript
sign = function (payload, secretOrPrivateKey, options, callback) {
  options = options || {};

  var isObjectPayload = typeof payload === 'object' &&
                        !Buffer.isBuffer(payload);

  var header = xtend({
    alg: options.algorithm || 'HS256',
    typ: isObjectPayload ? 'JWT' : undefined,
    kid: options.keyid
  }, options.header);

  function failure(err) {
    if (callback) {
      return callback(err);
    }
    throw err;
  }


  if (typeof payload === 'undefined') {
    return failure(new Error('payload is required'));
  } else if (isObjectPayload) {
    var payload_validation_result = registered_claims_schema.validate(payload);

    if (payload_validation_result.error) {
      return failure(payload_validation_result.error);
    }

    payload = xtend(payload);
  } else {
    var invalid_options = options_for_objects.filter(function (opt) {
      return typeof options[opt] !== 'undefined';
    });

    if (invalid_options.length > 0) {
      return failure(new Error('invalid ' + invalid_options.join(',') + ' option for ' + (typeof payload ) + ' payload'));
    }
  }

  if (typeof payload.exp !== 'undefined' && typeof options.expiresIn !== 'undefined') {
    return failure(new Error('Bad "options.expiresIn" option the payload already has an "exp" property.'));
  }

  if (typeof payload.nbf !== 'undefined' && typeof options.notBefore !== 'undefined') {
    return failure(new Error('Bad "options.notBefore" option the payload already has an "nbf" property.'));
  }

  var validation_result = sign_options_schema.validate(options);

  if (validation_result.error) {
    return failure(validation_result.error);
  }

  var timestamp = payload.iat || Math.floor(Date.now() / 1000);

  if (!options.noTimestamp) {
    payload.iat = timestamp;
  } else {
    delete payload.iat;
  }

  if (typeof options.notBefore !== 'undefined') {
    payload.nbf = timespan(options.notBefore);
    if (typeof payload.nbf === 'undefined') {
      return failure(new Error('"notBefore" should be a number of seconds or string representing a timespan eg: "1d", "20h", 60'));
    }
  }

  if (typeof options.expiresIn !== 'undefined' && typeof payload === 'object') {
    payload.exp = timespan(options.expiresIn, timestamp);
    if (typeof payload.exp === 'undefined') {
      return failure(new Error('"expiresIn" should be a number of seconds or string representing a timespan eg: "1d", "20h", 60'));
    }
  }

  Object.keys(options_to_payload).forEach(function (key) {
    var claim = options_to_payload[key];
    if (typeof options[key] !== 'undefined') {
      if (typeof payload[claim] !== 'undefined') {
        return failure(new Error('Bad "options.' + key + '" option. The payload already has an "' + claim + '" property.'));
      }
      payload[claim] = options[key];
    }
  });

  var encoding = options.encoding || 'utf8';

  if (typeof callback === 'function') {
    callback = callback && once(callback);

    jws.createSign({
      header: header,
      privateKey: secretOrPrivateKey,
      payload: payload,
      encoding: encoding
    }).once('error', callback)
      .once('done', function (signature) {
        callback(null, signature);
      });
  } else {
    return jws.sign({header: header, payload: payload, secret: secretOrPrivateKey, encoding: encoding});
  }
}
```
- example usage
```shell
...

'''bash
$ npm install jsonwebtoken
'''

# Usage

### jwt.sign(payload, secretOrPrivateKey, options, [callback])

(Asynchronous) If a callback is supplied, callback is called with the 'err' or the JWT.

(Synchronous) Returns the JsonWebToken as string

'payload' could be an object literal, buffer or string. *Please note that* 'exp' is only set if the payload is an object literal
.
...
```

#### <a name="apidoc.element.jsonwebtoken.verify"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>verify (jwtString, secretOrPublicKey, options, callback)](#apidoc.element.jsonwebtoken.verify)
- description and source-code
```javascript
verify = function (jwtString, secretOrPublicKey, options, callback) {
  if ((typeof options === 'function') && !callback) {
    callback = options;
    options = {};
  }

  if (!options) {
    options = {};
  }

  //clone this object since we are going to mutate it.
  options = xtend(options);
  var done;

  if (callback) {
    done = function() {
      var args = Array.prototype.slice.call(arguments, 0);
      return process.nextTick(function() {
        callback.apply(null, args);
      });
    };
  } else {
    done = function(err, data) {
      if (err) throw err;
      return data;
    };
  }

  if (options.clockTimestamp && typeof options.clockTimestamp !== 'number') {
    return done(new JsonWebTokenError('clockTimestamp must be a number'));
  }

  var clockTimestamp = options.clockTimestamp || Math.floor(Date.now() / 1000);

  if (!jwtString){
    return done(new JsonWebTokenError('jwt must be provided'));
  }

  if (typeof jwtString !== 'string') {
    return done(new JsonWebTokenError('jwt must be a string'));
  }

  var parts = jwtString.split('.');

  if (parts.length !== 3){
    return done(new JsonWebTokenError('jwt malformed'));
  }

  var hasSignature = parts[2].trim() !== '';

  if (!hasSignature && secretOrPublicKey){
    return done(new JsonWebTokenError('jwt signature is required'));
  }

  if (hasSignature && !secretOrPublicKey) {
    return done(new JsonWebTokenError('secret or public key must be provided'));
  }

  if (!hasSignature && !options.algorithms) {
    options.algorithms = ['none'];
  }

  if (!options.algorithms) {
    options.algorithms = ~secretOrPublicKey.toString().indexOf('BEGIN CERTIFICATE') ||
                         ~secretOrPublicKey.toString().indexOf('BEGIN PUBLIC KEY') ?
                          [ 'RS256','RS384','RS512','ES256','ES384','ES512' ] :
                         ~secretOrPublicKey.toString().indexOf('BEGIN RSA PUBLIC KEY') ?
                          [ 'RS256','RS384','RS512' ] :
                          [ 'HS256','HS384','HS512' ];

  }

  var decodedToken;
  try {
    decodedToken = jws.decode(jwtString);
  } catch(err) {
    return done(err);
  }

  if (!decodedToken) {
    return done(new JsonWebTokenError('invalid token'));
  }

  var header = decodedToken.header;

  if (!~options.algorithms.indexOf(header.alg)) {
    return done(new JsonWebTokenError('invalid algorithm'));
  }

  var valid;

  try {
    valid = jws.verify(jwtString, header.alg, secretOrPublicKey);
  } catch (e) {
    return done(e);
  }

  if (!valid)
    return done(new JsonWebTokenError('invalid signature'));

  var payload;

  try {
    payload = decode(jwtString);
  } catch(err) {
    return done(err);
  }

  if (typeof payload.nbf !== 'undefined' && !options.ignoreNotBefore) {
    if (typeof payload.nbf !== 'number') {
      return done(new JsonWebTokenError('invalid nbf value'));
    }
    if (payload.nbf > clockTimestamp + (options.clockTolerance || 0)) {
      return done(new NotBeforeError('jwt not active', new Date(payload.nbf * 1000)));
    }
  }

  if (typeof payload.exp !== 'undefined' && !options.ignoreExpiration) {
    if (typeof payload.exp !== 'number') {
      return done(new JsonWebTokenError('invalid exp value'));
    }
    if (clockTimestamp >= payload.exp + (options.clockTolerance || 0)) {
      return done(new TokenExpiredError('jwt expired', new Date(payload.exp * 1000)));
    }
  }

  if (options.audience) {
    var audiences = Array.isArray(options.audience)? options.audience : [options.audience];
    var target = Array.isArray(payload.aud) ? payload.aud : [payload.aud];

    var match = target.some(function(aud) { return audiences.indexOf(aud) != -1; });

    if (!match)
      return done(new JsonWebTokenError('jwt audience invalid. expected: ' + audiences.join(' or ')));
  }

  if (options.issuer) {
    var invalid_issuer =
        (typeof options.issuer === 'string' && payload.iss !== options.issuer) ||
        (Array.isArray(options.issuer) && options.issuer.indexOf(payload.iss) === -1);

    if (invalid_issuer) {
      return done(new JsonWebTokenError('jwt issuer inv ...
```
- example usage
```shell
...
//or even better:

jwt.sign({
  data: 'foobar'
}, 'secret', { expiresIn: '1h' });
'''

### jwt.verify(token, secretOrPublicKey, [options, callback])

(Asynchronous) If a callback is supplied, function acts asynchronously. Callback is passed the decoded payload if the signature
and optional expiration, audience, or issuer are valid. If not, it will be passed the error.

(Synchronous) If a callback is not supplied, function acts synchronously. Returns the payload decoded if the signature (and, optionally
, expiration, audience, issuer) are valid. If not, it will throw the error.

'token' is the JsonWebToken string
...
```



# <a name="apidoc.module.jsonwebtoken.JsonWebTokenError"></a>[module jsonwebtoken.JsonWebTokenError](#apidoc.module.jsonwebtoken.JsonWebTokenError)

#### <a name="apidoc.element.jsonwebtoken.JsonWebTokenError.JsonWebTokenError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>JsonWebTokenError (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError.JsonWebTokenError)
- description and source-code
```javascript
JsonWebTokenError = function (message, error) {
  Error.call(this, message);
  Error.captureStackTrace(this, this.constructor);
  this.name = 'JsonWebTokenError';
  this.message = message;
  if (error) this.inner = error;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsonwebtoken.JsonWebTokenError.prototype"></a>[module jsonwebtoken.JsonWebTokenError.prototype](#apidoc.module.jsonwebtoken.JsonWebTokenError.prototype)

#### <a name="apidoc.element.jsonwebtoken.JsonWebTokenError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.JsonWebTokenError.prototype.</span>constructor (message, error)](#apidoc.element.jsonwebtoken.JsonWebTokenError.prototype.constructor)
- description and source-code
```javascript
constructor = function (message, error) {
  Error.call(this, message);
  Error.captureStackTrace(this, this.constructor);
  this.name = 'JsonWebTokenError';
  this.message = message;
  if (error) this.inner = error;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsonwebtoken.NotBeforeError"></a>[module jsonwebtoken.NotBeforeError](#apidoc.module.jsonwebtoken.NotBeforeError)

#### <a name="apidoc.element.jsonwebtoken.NotBeforeError.NotBeforeError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>NotBeforeError (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError.NotBeforeError)
- description and source-code
```javascript
NotBeforeError = function (message, date) {
  JsonWebTokenError.call(this, message);
  this.name = 'NotBeforeError';
  this.date = date;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsonwebtoken.NotBeforeError.prototype"></a>[module jsonwebtoken.NotBeforeError.prototype](#apidoc.module.jsonwebtoken.NotBeforeError.prototype)

#### <a name="apidoc.element.jsonwebtoken.NotBeforeError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.NotBeforeError.prototype.</span>constructor (message, date)](#apidoc.element.jsonwebtoken.NotBeforeError.prototype.constructor)
- description and source-code
```javascript
constructor = function (message, date) {
  JsonWebTokenError.call(this, message);
  this.name = 'NotBeforeError';
  this.date = date;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsonwebtoken.TokenExpiredError"></a>[module jsonwebtoken.TokenExpiredError](#apidoc.module.jsonwebtoken.TokenExpiredError)

#### <a name="apidoc.element.jsonwebtoken.TokenExpiredError.TokenExpiredError"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.</span>TokenExpiredError (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError.TokenExpiredError)
- description and source-code
```javascript
TokenExpiredError = function (message, expiredAt) {
  JsonWebTokenError.call(this, message);
  this.name = 'TokenExpiredError';
  this.expiredAt = expiredAt;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsonwebtoken.TokenExpiredError.prototype"></a>[module jsonwebtoken.TokenExpiredError.prototype](#apidoc.module.jsonwebtoken.TokenExpiredError.prototype)

#### <a name="apidoc.element.jsonwebtoken.TokenExpiredError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">jsonwebtoken.TokenExpiredError.prototype.</span>constructor (message, expiredAt)](#apidoc.element.jsonwebtoken.TokenExpiredError.prototype.constructor)
- description and source-code
```javascript
constructor = function (message, expiredAt) {
  JsonWebTokenError.call(this, message);
  this.name = 'TokenExpiredError';
  this.expiredAt = expiredAt;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
