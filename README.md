# api documentation for  [bignum (v0.12.5)](https://github.com/justmoon/node-bignum#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bignum.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bignum) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bignum.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bignum)
#### Arbitrary-precision integer arithmetic using OpenSSL

[![NPM](https://nodei.co/npm/bignum.png?downloads=true)](https://www.npmjs.com/package/bignum)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.buildApidoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-bignum%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bignum/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bignum/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stefan Thomas",
        "email": "justmoon@members.fsf.org",
        "url": "http://www.justmoon.net"
    },
    "binary": {
        "host": "https://rvagg-node.s3-us-west-2.amazonaws.com",
        "module_name": "bignum",
        "module_path": "binding/",
        "remote_path": "./{name}/v{version}"
    },
    "bugs": {
        "url": "https://github.com/justmoon/node-bignum/issues"
    },
    "contributors": [
        {
            "name": "James Halliday",
            "email": "mail@substack.net"
        },
        {
            "name": "Rod Vagg",
            "email": "rod@vagg.org"
        }
    ],
    "dependencies": {
        "nan": "^2.3.4",
        "node-pre-gyp": "~0.6.28"
    },
    "description": "Arbitrary-precision integer arithmetic using OpenSSL",
    "devDependencies": {
        "aws-sdk": "~2.4.0",
        "put": "~0.0.5",
        "standard": "~7.1.2",
        "tap": "~5.7.2"
    },
    "directories": {},
    "dist": {
        "shasum": "208f2b0e18eb8fd6950917e3718e4cd85cccffcd",
        "tarball": "https://registry.npmjs.org/bignum/-/bignum-0.12.5.tgz"
    },
    "gitHead": "9c3254dbf19c8a56679311e68bba0ae64ef4df7a",
    "homepage": "https://github.com/justmoon/node-bignum#readme",
    "keywords": [
        "openssl",
        "big",
        "bignum",
        "bigint",
        "integer",
        "arithmetic",
        "precision"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "bitcoinjs",
            "email": "bitcoinjs@justmoon.net"
        },
        {
            "name": "justmoon",
            "email": "justmoon@members.fsf.org"
        },
        {
            "name": "rvagg",
            "email": "rod@vagg.org"
        }
    ],
    "name": "bignum",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/justmoon/node-bignum.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "test": "standard && tap test/*.js"
    },
    "version": "0.12.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bignum](#apidoc.module.bignum)
1.  [function <span class="apidocSignatureSpan">bignum.</span>abs (num)](#apidoc.element.bignum.abs)
1.  [function <span class="apidocSignatureSpan">bignum.</span>add (num)](#apidoc.element.bignum.add)
1.  [function <span class="apidocSignatureSpan">bignum.</span>and (num)](#apidoc.element.bignum.and)
1.  [function <span class="apidocSignatureSpan">bignum.</span>babs (num)](#apidoc.element.bignum.babs)
1.  [function <span class="apidocSignatureSpan">bignum.</span>badd (num)](#apidoc.element.bignum.badd)
1.  [function <span class="apidocSignatureSpan">bignum.</span>band (num)](#apidoc.element.bignum.band)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bcompare (num)](#apidoc.element.bignum.bcompare)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bdiv (num)](#apidoc.element.bignum.bdiv)
1.  [function <span class="apidocSignatureSpan">bignum.</span>binvertm (num)](#apidoc.element.bignum.binvertm)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bitLength (num)](#apidoc.element.bignum.bitLength)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bmod (num)](#apidoc.element.bignum.bmod)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bmul (num)](#apidoc.element.bignum.bmul)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bneg (num)](#apidoc.element.bignum.bneg)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bor (num)](#apidoc.element.bignum.bor)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bpowm (num)](#apidoc.element.bignum.bpowm)
1.  [function <span class="apidocSignatureSpan">bignum.</span>brand0 (num)](#apidoc.element.bignum.brand0)
1.  [function <span class="apidocSignatureSpan">bignum.</span>broot (num)](#apidoc.element.bignum.broot)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bsqrt (num)](#apidoc.element.bignum.bsqrt)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bsub (num)](#apidoc.element.bignum.bsub)
1.  [function <span class="apidocSignatureSpan">bignum.</span>bxor (num)](#apidoc.element.bignum.bxor)
1.  [function <span class="apidocSignatureSpan">bignum.</span>cmp (num)](#apidoc.element.bignum.cmp)
1.  [function <span class="apidocSignatureSpan">bignum.</span>conditionArgs (num, base)](#apidoc.element.bignum.conditionArgs)
1.  [function <span class="apidocSignatureSpan">bignum.</span>div (num)](#apidoc.element.bignum.div)
1.  [function <span class="apidocSignatureSpan">bignum.</span>eq (num)](#apidoc.element.bignum.eq)
1.  [function <span class="apidocSignatureSpan">bignum.</span>fromBuffer (buf, opts)](#apidoc.element.bignum.fromBuffer)
1.  [function <span class="apidocSignatureSpan">bignum.</span>gcd (num)](#apidoc.element.bignum.gcd)
1.  [function <span class="apidocSignatureSpan">bignum.</span>ge (num)](#apidoc.element.bignum.ge)
1.  [function <span class="apidocSignatureSpan">bignum.</span>gt (num)](#apidoc.element.bignum.gt)
1.  [function <span class="apidocSignatureSpan">bignum.</span>invertm (num)](#apidoc.element.bignum.invertm)
1.  [function <span class="apidocSignatureSpan">bignum.</span>isBigNum (num)](#apidoc.element.bignum.isBigNum)
1.  [function <span class="apidocSignatureSpan">bignum.</span>isBitSet (num)](#apidoc.element.bignum.isBitSet)
1.  [function <span class="apidocSignatureSpan">bignum.</span>isbitset (num)](#apidoc.element.bignum.isbitset)
1.  [function <span class="apidocSignatureSpan">bignum.</span>jacobi (num)](#apidoc.element.bignum.jacobi)
1.  [function <span class="apidocSignatureSpan">bignum.</span>le (num)](#apidoc.element.bignum.le)
1.  [function <span class="apidocSignatureSpan">bignum.</span>lt (num)](#apidoc.element.bignum.lt)
1.  [function <span class="apidocSignatureSpan">bignum.</span>mod (num)](#apidoc.element.bignum.mod)
1.  [function <span class="apidocSignatureSpan">bignum.</span>mul (num)](#apidoc.element.bignum.mul)
1.  [function <span class="apidocSignatureSpan">bignum.</span>ne (num)](#apidoc.element.bignum.ne)
1.  [function <span class="apidocSignatureSpan">bignum.</span>neg (num)](#apidoc.element.bignum.neg)
1.  [function <span class="apidocSignatureSpan">bignum.</span>nextPrime (num)](#apidoc.element.bignum.nextPrime)
1.  [function <span class="apidocSignatureSpan">bignum.</span>or (num)](#apidoc.element.bignum.or)
1.  [function <span class="apidocSignatureSpan">bignum.</span>pow (num)](#apidoc.element.bignum.pow)
1.  [function <span class="apidocSignatureSpan">bignum.</span>powm (num)](#apidoc.element.bignum.powm)
1.  [function <span class="apidocSignatureSpan">bignum.</span>prime (bits, safe)](#apidoc.element.bignum.prime)
1.  [function <span class="apidocSignatureSpan">bignum.</span>probPrime (num)](#apidoc.element.bignum.probPrime)
1.  [function <span class="apidocSignatureSpan">bignum.</span>probprime (num)](#apidoc.element.bignum.probprime)
1.  [function <span class="apidocSignatureSpan">bignum.</span>rand (num)](#apidoc.element.bignum.rand)
1.  [function <span class="apidocSignatureSpan">bignum.</span>root (num)](#apidoc.element.bignum.root)
1.  [function <span class="apidocSignatureSpan">bignum.</span>scompare (num)](#apidoc.element.bignum.scompare)
1.  [function <span class="apidocSignatureSpan">bignum.</span>setCompact (num)](#apidoc.element.bignum.setCompact)
1.  [function <span class="apidocSignatureSpan">bignum.</span>shiftLeft (num)](#apidoc.element.bignum.shiftLeft)
1.  [function <span class="apidocSignatureSpan">bignum.</span>shiftRight (num)](#apidoc.element.bignum.shiftRight)
1.  [function <span class="apidocSignatureSpan">bignum.</span>sqrt (num)](#apidoc.element.bignum.sqrt)
1.  [function <span class="apidocSignatureSpan">bignum.</span>sub (num)](#apidoc.element.bignum.sub)
1.  [function <span class="apidocSignatureSpan">bignum.</span>toBuffer (num)](#apidoc.element.bignum.toBuffer)
1.  [function <span class="apidocSignatureSpan">bignum.</span>toNumber (num)](#apidoc.element.bignum.toNumber)
1.  [function <span class="apidocSignatureSpan">bignum.</span>tostring (num)](#apidoc.element.bignum.tostring)
1.  [function <span class="apidocSignatureSpan">bignum.</span>uadd (num)](#apidoc.element.bignum.uadd)
1.  [function <span class="apidocSignatureSpan">bignum.</span>ucompare (num)](#apidoc.element.bignum.ucompare)
1.  [function <span class="apidocSignatureSpan">bignum.</span>udiv (num)](#apidoc.element.bignum.udiv)
1.  [function <span class="apidocSignatureSpan">bignum.</span>udiv2exp (num)](#apidoc.element.bignum.udiv2exp)
1.  [function <span class="apidocSignatureSpan">bignum.</span>umod (num)](#apidoc.element.bignum.umod)
1.  [function <span class="apidocSignatureSpan">bignum.</span>umul (num)](#apidoc.element.bignum.umul)
1.  [function <span class="apidocSignatureSpan">bignum.</span>umul2exp (num)](#apidoc.element.bignum.umul2exp)
1.  [function <span class="apidocSignatureSpan">bignum.</span>upow (num)](#apidoc.element.bignum.upow)
1.  [function <span class="apidocSignatureSpan">bignum.</span>upowm (num)](#apidoc.element.bignum.upowm)
1.  [function <span class="apidocSignatureSpan">bignum.</span>uprime0 ()](#apidoc.element.bignum.uprime0)
1.  [function <span class="apidocSignatureSpan">bignum.</span>usub (num)](#apidoc.element.bignum.usub)
1.  [function <span class="apidocSignatureSpan">bignum.</span>xor (num)](#apidoc.element.bignum.xor)



# <a name="apidoc.module.bignum"></a>[module bignum](#apidoc.module.bignum)

#### <a name="apidoc.element.bignum.abs"></a>[function <span class="apidocSignatureSpan">bignum.</span>abs (num)](#apidoc.element.bignum.abs)
- description and source-code
```javascript
abs = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Return a new 'bignum' containing the instance value multiplied by 'n'.

.div(n)
-------

Return a new 'bignum' containing the instance value integrally divided by 'n'.

.abs()
------

Return a new 'bignum' with the absolute value of the instance.

.neg()
------
...
```

#### <a name="apidoc.element.bignum.add"></a>[function <span class="apidocSignatureSpan">bignum.</span>add (num)](#apidoc.element.bignum.add)
- description and source-code
```javascript
add = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
    endian : 'big',
    size : 1, // number of bytes in each word
}
'''

Note that endian doesn't matter when size = 1. If you wish to reverse the entire buffer byte by byte, pass size: 'auto'.

.add(n)
-------

Return a new 'bignum' containing the instance value plus 'n'.

.sub(n)
-------
...
```

#### <a name="apidoc.element.bignum.and"></a>[function <span class="apidocSignatureSpan">bignum.</span>and (num)](#apidoc.element.bignum.and)
- description and source-code
```javascript
and = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.le(n)
------

Return a boolean: whether the instance value is less than or equal to n
('<= n').

.and(n)
-------

Return a new 'bignum' with the instance value bitwise AND (&)-ed with 'n'.

.or(n)
------
...
```

#### <a name="apidoc.element.bignum.babs"></a>[function <span class="apidocSignatureSpan">bignum.</span>babs (num)](#apidoc.element.bignum.babs)
- description and source-code
```javascript
babs = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
      throw new TypeError('Unspecified operation for type ' +
        (typeof num) + ' for ' + op)
    }
  }
})

BigNum.prototype.abs = function () {
  return this.babs()
}

BigNum.prototype.neg = function () {
  return this.bneg()
}

BigNum.prototype.powm = function (num, mod) {
...
```

#### <a name="apidoc.element.bignum.badd"></a>[function <span class="apidocSignatureSpan">bignum.</span>badd (num)](#apidoc.element.bignum.badd)
- description and source-code
```javascript
badd = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.band"></a>[function <span class="apidocSignatureSpan">bignum.</span>band (num)](#apidoc.element.bignum.band)
- description and source-code
```javascript
band = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.bcompare"></a>[function <span class="apidocSignatureSpan">bignum.</span>bcompare (num)](#apidoc.element.bignum.bcompare)
- description and source-code
```javascript
bcompare = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  var x = parseInt(num.toString(), 10)
  return BigNum.prototype.shiftRight.call(this, x)
}
}

BigNum.prototype.cmp = function (num) {
if (BigNum.isBigNum(num)) {
  return this.bcompare(num)
} else if (typeof num === 'number') {
  if (num < 0) {
    return this.scompare(num)
  } else {
    return this.ucompare(num)
  }
} else {
...
```

#### <a name="apidoc.element.bignum.bdiv"></a>[function <span class="apidocSignatureSpan">bignum.</span>bdiv (num)](#apidoc.element.bignum.bdiv)
- description and source-code
```javascript
bdiv = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.binvertm"></a>[function <span class="apidocSignatureSpan">bignum.</span>binvertm (num)](#apidoc.element.bignum.binvertm)
- description and source-code
```javascript
binvertm = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
     : BigNum(to).sub(this)
    return x.brand0().add(this)
  }
}

BigNum.prototype.invertm = function (mod) {
  if (BigNum.isBigNum(mod)) {
    return this.binvertm(mod)
  } else {
    var x = BigNum(mod)
    return this.binvertm(x)
  }
}

BigNum.prime = function (bits, safe) {
...
```

#### <a name="apidoc.element.bignum.bitLength"></a>[function <span class="apidocSignatureSpan">bignum.</span>bitLength (num)](#apidoc.element.bignum.bitLength)
- description and source-code
```javascript
bitLength = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
-------

Return the Jacobi symbol (or Legendre symbol if 'n' is prime) of the current
'bignum' (= a) over 'n'. Note that 'n' must be odd and >= 3. 0 <= a < n.

Returns -1 or 1 as an int (NOT a bignum). Throws an error on failure.

.bitLength()
------------

Return the number of bits used to represent the current 'bignum'.

install
=======
...
```

#### <a name="apidoc.element.bignum.bmod"></a>[function <span class="apidocSignatureSpan">bignum.</span>bmod (num)](#apidoc.element.bignum.bmod)
- description and source-code
```javascript
bmod = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  m = mod
}

if ((typeof num) === 'number') {
  return this.umod(num, m)
} else if ((typeof num) === 'string') {
  var n = BigNum(num)
  return this.bmod(n, m)
} else if (BigNum.isBigNum(num)) {
  return this.bmod(num, m)
}
}

BigNum.prototype.pow = function (num) {
if (typeof num === 'number') {
...
```

#### <a name="apidoc.element.bignum.bmul"></a>[function <span class="apidocSignatureSpan">bignum.</span>bmul (num)](#apidoc.element.bignum.bmul)
- description and source-code
```javascript
bmul = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.bneg"></a>[function <span class="apidocSignatureSpan">bignum.</span>bneg (num)](#apidoc.element.bignum.bneg)
- description and source-code
```javascript
bneg = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
})

BigNum.prototype.abs = function () {
return this.babs()
}

BigNum.prototype.neg = function () {
return this.bneg()
}

BigNum.prototype.powm = function (num, mod) {
var m

if ((typeof mod) === 'number' || (typeof mod) === 'string') {
  m = BigNum(mod)
...
```

#### <a name="apidoc.element.bignum.bor"></a>[function <span class="apidocSignatureSpan">bignum.</span>bor (num)](#apidoc.element.bignum.bor)
- description and source-code
```javascript
bor = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.bpowm"></a>[function <span class="apidocSignatureSpan">bignum.</span>bpowm (num)](#apidoc.element.bignum.bpowm)
- description and source-code
```javascript
bpowm = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  m = mod
}

if ((typeof num) === 'number') {
  return this.upowm(num, m)
} else if ((typeof num) === 'string') {
  var n = BigNum(num)
  return this.bpowm(n, m)
} else if (BigNum.isBigNum(num)) {
  return this.bpowm(num, m)
}
}

BigNum.prototype.mod = function (num, mod) {
var m
...
```

#### <a name="apidoc.element.bignum.brand0"></a>[function <span class="apidocSignatureSpan">bignum.</span>brand0 (num)](#apidoc.element.bignum.brand0)
- description and source-code
```javascript
brand0 = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
}

BigNum.prototype.rand = function (to) {
if (to === undefined) {
  if (this.toString() === '1') {
    return BigNum(0)
  } else {
    return this.brand0()
  }
} else {
  var x = BigNum.isBigNum(to)
    ? to.sub(this)
   : BigNum(to).sub(this)
  return x.brand0().add(this)
}
...
```

#### <a name="apidoc.element.bignum.broot"></a>[function <span class="apidocSignatureSpan">bignum.</span>broot (num)](#apidoc.element.bignum.broot)
- description and source-code
```javascript
broot = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

BigNum.prototype.sqrt = function () {
return this.bsqrt()
}

BigNum.prototype.root = function (num) {
if (BigNum.isBigNum(num)) {
  return this.broot(num)
} else {
  return this.broot(num)
}
}

BigNum.prototype.rand = function (to) {
if (to === undefined) {
...
```

#### <a name="apidoc.element.bignum.bsqrt"></a>[function <span class="apidocSignatureSpan">bignum.</span>bsqrt (num)](#apidoc.element.bignum.bsqrt)
- description and source-code
```javascript
bsqrt = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
    var x = BigNum(num)
    return this['b' + name](x)
  }
}
})

BigNum.prototype.sqrt = function () {
return this.bsqrt()
}

BigNum.prototype.root = function (num) {
if (BigNum.isBigNum(num)) {
  return this.broot(num)
} else {
  return this.broot(num)
...
```

#### <a name="apidoc.element.bignum.bsub"></a>[function <span class="apidocSignatureSpan">bignum.</span>bsub (num)](#apidoc.element.bignum.bsub)
- description and source-code
```javascript
bsub = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.bxor"></a>[function <span class="apidocSignatureSpan">bignum.</span>bxor (num)](#apidoc.element.bignum.bxor)
- description and source-code
```javascript
bxor = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.cmp"></a>[function <span class="apidocSignatureSpan">bignum.</span>cmp (num)](#apidoc.element.bignum.cmp)
- description and source-code
```javascript
cmp = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Return a new 'bignum' with the absolute value of the instance.

.neg()
------

Return a new 'bignum' with the negative of the instance value.

.cmp(n)
-------

Compare the instance value to 'n'. Return a positive integer if '> n', a
negative integer if '< n', and 0 if '== n'.

.gt(n)
------
...
```

#### <a name="apidoc.element.bignum.conditionArgs"></a>[function <span class="apidocSignatureSpan">bignum.</span>conditionArgs (num, base)](#apidoc.element.bignum.conditionArgs)
- description and source-code
```javascript
conditionArgs = function (num, base) {
  if (typeof num !== 'string') num = num.toString(base || 10)

  if (num.match(/e\+/)) { // positive exponent
    if (!Number(num).toString().match(/e+/)) {
      return {
        num: Math.floor(Number(num)).toString(),
        base: 10
      }
    } else {
      var pow = Math.ceil(Math.log(num) / Math.log(2))
      var n = (num / Math.pow(2, pow)).toString(2)
        .replace(/^0/, '')
      var i = n.length - n.indexOf('.')
      n = n.replace(/\./, '')

      for (; i <= pow; i++) n += '0'
      return {
        num: n,
        base: 2
      }
    }
  } else if (num.match(/e\-/)) { // negative exponent
    return {
      num: Math.floor(Number(num)).toString(),
      base: base || 10
    }
  } else {
    return {
      num: num,
      base: base || 10
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.div"></a>[function <span class="apidocSignatureSpan">bignum.</span>div (num)](#apidoc.element.bignum.div)
- description and source-code
```javascript
div = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
---------

'''js
var bignum = require('bignum');

var b = bignum('782910138827292261791972728324982')
.sub('182373273283402171237474774728373')
.div(8)
;
console.log(b);
'''

***
$ node simple.js
<Bignum 75067108192986261319312244199576>
...
```

#### <a name="apidoc.element.bignum.eq"></a>[function <span class="apidocSignatureSpan">bignum.</span>eq (num)](#apidoc.element.bignum.eq)
- description and source-code
```javascript
eq = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.ge(n)
------

Return a boolean: whether the instance value is greater than or equal to n
('>= n').

.eq(n)
------

Return a boolean: whether the instance value is equal to n ('== n').

.lt(n)
------
...
```

#### <a name="apidoc.element.bignum.fromBuffer"></a>[function <span class="apidocSignatureSpan">bignum.</span>fromBuffer (buf, opts)](#apidoc.element.bignum.fromBuffer)
- description and source-code
```javascript
fromBuffer = function (buf, opts) {
  if (!opts) opts = {}

  var endian = { 1: 'big', '-1': 'little' }[opts.endian] ||
    opts.endian || 'big'

  var size = opts.size === 'auto' ? Math.ceil(buf.length) : (opts.size || 1)

  if (buf.length % size !== 0) {
    throw new RangeError('Buffer length (' + buf.length + ')' +
      ' must be a multiple of size (' + size + ')'
    )
  }

  var hex = []
  for (var i = 0; i < buf.length; i += size) {
    var chunk = []
    for (var j = 0; j < size; j++) {
      chunk.push(buf[i + (endian === 'big' ? j : (size - j - 1))])
    }

    hex.push(chunk
      .map(function (c) {
        return (c < 16 ? '0' : '') + c.toString(16)
      })
      .join('')
    )
  }

  return BigNum(hex.join(''), 16)
}
```
- example usage
```shell
...
If you pass in a string you can set the base that string is encoded in.

.toString(base=10)
------------------

Print out the 'bignum' instance in the requested base as a string.

bignum.fromBuffer(buf, opts)
----------------------------

Create a new 'bignum' from a 'Buffer'.

The default options are:

'''js
...
```

#### <a name="apidoc.element.bignum.gcd"></a>[function <span class="apidocSignatureSpan">bignum.</span>gcd (num)](#apidoc.element.bignum.gcd)
- description and source-code
```javascript
gcd = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.shiftRight(n)
--------------

Return a new 'bignum' of the value integer divided by
'2^n'. Equivalent of the '>>' operator.

.gcd(n)
-------

Return the greatest common divisor of the current 'bignum' with 'n' as a new
'bignum'.

.jacobi(n)
-------
...
```

#### <a name="apidoc.element.bignum.ge"></a>[function <span class="apidocSignatureSpan">bignum.</span>ge (num)](#apidoc.element.bignum.ge)
- description and source-code
```javascript
ge = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
negative integer if '< n', and 0 if '== n'.

.gt(n)
------

Return a boolean: whether the instance value is greater than n ('> n').

.ge(n)
------

Return a boolean: whether the instance value is greater than or equal to n
('>= n').

.eq(n)
------
...
```

#### <a name="apidoc.element.bignum.gt"></a>[function <span class="apidocSignatureSpan">bignum.</span>gt (num)](#apidoc.element.bignum.gt)
- description and source-code
```javascript
gt = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.cmp(n)
-------

Compare the instance value to 'n'. Return a positive integer if '> n', a
negative integer if '< n', and 0 if '== n'.

.gt(n)
------

Return a boolean: whether the instance value is greater than n ('> n').

.ge(n)
------
...
```

#### <a name="apidoc.element.bignum.invertm"></a>[function <span class="apidocSignatureSpan">bignum.</span>invertm (num)](#apidoc.element.bignum.invertm)
- description and source-code
```javascript
invertm = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.powm(n, m)
-----------

Return a new 'bignum' with the instance value raised to the 'n'th power modulo
'm'.

.invertm(m)
-----------

Compute the multiplicative inverse modulo 'm'.

.rand()
-------
.rand(upperBound)
...
```

#### <a name="apidoc.element.bignum.isBigNum"></a>[function <span class="apidocSignatureSpan">bignum.</span>isBigNum (num)](#apidoc.element.bignum.isBigNum)
- description and source-code
```javascript
isBigNum = function (num) {
  if (!num) {
    return false
  }
  for (var key in BigNum.prototype) {
    if (!num[key]) {
      return false
    }
  }
  return true
}
```
- example usage
```shell
...
Note that endian doesn't matter when size = 1. If you wish to reverse the entire buffer byte by byte, pass size: 'auto'.

bignum.prime(bits, safe=true)
-----------------------------

Generate a probable prime of length 'bits'. If 'safe' is true, it will be a "safe" prime of the form p=2p'+1 where p' is also prime
.

bignum.isBigNum(num)
-----------------------------

Return true if 'num' is identified as a bignum instance. Otherwise, return false.

methods[1]
==========
...
```

#### <a name="apidoc.element.bignum.isBitSet"></a>[function <span class="apidocSignatureSpan">bignum.</span>isBitSet (num)](#apidoc.element.bignum.isBitSet)
- description and source-code
```javascript
isBitSet = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.isbitset"></a>[function <span class="apidocSignatureSpan">bignum.</span>isbitset (num)](#apidoc.element.bignum.isbitset)
- description and source-code
```javascript
isbitset = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
do {
  num = num.add(1)
} while (!num.probPrime())
return num
}

BigNum.prototype.isBitSet = function (n) {
return this.isbitset(n) === 1
}

BigNum.fromBuffer = function (buf, opts) {
if (!opts) opts = {}

var endian = { 1: 'big', '-1': 'little' }[opts.endian] ||
  opts.endian || 'big'
...
```

#### <a name="apidoc.element.bignum.jacobi"></a>[function <span class="apidocSignatureSpan">bignum.</span>jacobi (num)](#apidoc.element.bignum.jacobi)
- description and source-code
```javascript
jacobi = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.gcd(n)
-------

Return the greatest common divisor of the current 'bignum' with 'n' as a new
'bignum'.

.jacobi(n)
-------

Return the Jacobi symbol (or Legendre symbol if 'n' is prime) of the current
'bignum' (= a) over 'n'. Note that 'n' must be odd and >= 3. 0 <= a < n.

Returns -1 or 1 as an int (NOT a bignum). Throws an error on failure.
...
```

#### <a name="apidoc.element.bignum.le"></a>[function <span class="apidocSignatureSpan">bignum.</span>le (num)](#apidoc.element.bignum.le)
- description and source-code
```javascript
le = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Return a boolean: whether the instance value is equal to n ('== n').

.lt(n)
------

Return a boolean: whether the instance value is less than n ('< n').

.le(n)
------

Return a boolean: whether the instance value is less than or equal to n
('<= n').

.and(n)
-------
...
```

#### <a name="apidoc.element.bignum.lt"></a>[function <span class="apidocSignatureSpan">bignum.</span>lt (num)](#apidoc.element.bignum.lt)
- description and source-code
```javascript
lt = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
('>= n').

.eq(n)
------

Return a boolean: whether the instance value is equal to n ('== n').

.lt(n)
------

Return a boolean: whether the instance value is less than n ('< n').

.le(n)
------
...
```

#### <a name="apidoc.element.bignum.mod"></a>[function <span class="apidocSignatureSpan">bignum.</span>mod (num)](#apidoc.element.bignum.mod)
- description and source-code
```javascript
mod = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.xor(n)
-------

Return a new 'bignum' with the instance value bitwise exclusive-OR (^)-ed with
'n'.

.mod(n)
-------

Return a new 'bignum' with the instance value modulo 'n'.

'm'.
.pow(n)
-------
...
```

#### <a name="apidoc.element.bignum.mul"></a>[function <span class="apidocSignatureSpan">bignum.</span>mul (num)](#apidoc.element.bignum.mul)
- description and source-code
```javascript
mul = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
'''js
// If 2**n-1 is prime, then (2**n-1) * 2**(n-1) is perfect.
var bignum = require('bignum');

for (var n = 0; n < 100; n++) {
    var p = bignum.pow(2, n).sub(1);
    if (p.probPrime(50)) {
        var perfect = p.mul(bignum.pow(2, n - 1));
        console.log(perfect.toString());
    }
}
'''

***
...
```

#### <a name="apidoc.element.bignum.ne"></a>[function <span class="apidocSignatureSpan">bignum.</span>ne (num)](#apidoc.element.bignum.ne)
- description and source-code
```javascript
ne = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.neg"></a>[function <span class="apidocSignatureSpan">bignum.</span>neg (num)](#apidoc.element.bignum.neg)
- description and source-code
```javascript
neg = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Return a new 'bignum' containing the instance value integrally divided by 'n'.

.abs()
------

Return a new 'bignum' with the absolute value of the instance.

.neg()
------

Return a new 'bignum' with the negative of the instance value.

.cmp(n)
-------
...
```

#### <a name="apidoc.element.bignum.nextPrime"></a>[function <span class="apidocSignatureSpan">bignum.</span>nextPrime (num)](#apidoc.element.bignum.nextPrime)
- description and source-code
```javascript
nextPrime = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.or"></a>[function <span class="apidocSignatureSpan">bignum.</span>or (num)](#apidoc.element.bignum.or)
- description and source-code
```javascript
or = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
('<= n').

.and(n)
-------

Return a new 'bignum' with the instance value bitwise AND (&)-ed with 'n'.

.or(n)
------

Return a new 'bignum' with the instance value bitwise inclusive-OR (|)-ed with
'n'.

.xor(n)
-------
...
```

#### <a name="apidoc.element.bignum.pow"></a>[function <span class="apidocSignatureSpan">bignum.</span>pow (num)](#apidoc.element.bignum.pow)
- description and source-code
```javascript
pow = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Generate the perfect numbers:

'''js
// If 2**n-1 is prime, then (2**n-1) * 2**(n-1) is perfect.
var bignum = require('bignum');

for (var n = 0; n < 100; n++) {
    var p = bignum.pow(2, n).sub(1);
    if (p.probPrime(50)) {
        var perfect = p.mul(bignum.pow(2, n - 1));
        console.log(perfect.toString());
    }
}
'''
...
```

#### <a name="apidoc.element.bignum.powm"></a>[function <span class="apidocSignatureSpan">bignum.</span>powm (num)](#apidoc.element.bignum.powm)
- description and source-code
```javascript
powm = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

'm'.
.pow(n)
-------

Return a new 'bignum' with the instance value raised to the 'n'th power.

.powm(n, m)
-----------

Return a new 'bignum' with the instance value raised to the 'n'th power modulo
'm'.

.invertm(m)
-----------
...
```

#### <a name="apidoc.element.bignum.prime"></a>[function <span class="apidocSignatureSpan">bignum.</span>prime (bits, safe)](#apidoc.element.bignum.prime)
- description and source-code
```javascript
prime = function (bits, safe) {
  if (typeof safe === 'undefined') {
    safe = true
  }

  // Force uint32
  bits >>>= 0

  return BigNum.uprime0(bits, !!safe)
}
```
- example usage
```shell
...
    endian : 'big',
    size : 1, // number of bytes in each word
}
'''

Note that endian doesn't matter when size = 1. If you wish to reverse the entire buffer byte by byte, pass size: 'auto'.

bignum.prime(bits, safe=true)
-----------------------------

Generate a probable prime of length 'bits'. If 'safe' is true, it will be a "safe" prime of the form p=2p'+1 where p' is also prime
.

bignum.isBigNum(num)
-----------------------------
...
```

#### <a name="apidoc.element.bignum.probPrime"></a>[function <span class="apidocSignatureSpan">bignum.</span>probPrime (num)](#apidoc.element.bignum.probPrime)
- description and source-code
```javascript
probPrime = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

'''js
// If 2**n-1 is prime, then (2**n-1) * 2**(n-1) is perfect.
var bignum = require('bignum');

for (var n = 0; n < 100; n++) {
    var p = bignum.pow(2, n).sub(1);
    if (p.probPrime(50)) {
        var perfect = p.mul(bignum.pow(2, n - 1));
        console.log(perfect.toString());
    }
}
'''

***
...
```

#### <a name="apidoc.element.bignum.probprime"></a>[function <span class="apidocSignatureSpan">bignum.</span>probprime (num)](#apidoc.element.bignum.probprime)
- description and source-code
```javascript
probprime = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
// Force uint32
bits >>>= 0

return BigNum.uprime0(bits, !!safe)
}

BigNum.prototype.probPrime = function (reps) {
var n = this.probprime(reps || 10)
return { 1: true, 0: false }[n]
}

BigNum.prototype.nextPrime = function () {
var num = this
do {
  num = num.add(1)
...
```

#### <a name="apidoc.element.bignum.rand"></a>[function <span class="apidocSignatureSpan">bignum.</span>rand (num)](#apidoc.element.bignum.rand)
- description and source-code
```javascript
rand = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
'm'.

.invertm(m)
-----------

Compute the multiplicative inverse modulo 'm'.

.rand()
-------
.rand(upperBound)
-----------------

If 'upperBound' is supplied, return a random 'bignum' between the instance value
and 'upperBound - 1', inclusive.
...
```

#### <a name="apidoc.element.bignum.root"></a>[function <span class="apidocSignatureSpan">bignum.</span>root (num)](#apidoc.element.bignum.root)
- description and source-code
```javascript
root = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
using [BN_is_prime_ex](http://www.openssl.org/docs/crypto/BN_generate_prime.html).

.sqrt()
-------

Return a new 'bignum' that is the square root. This truncates.

.root(n)
-------

Return a new 'bignum' that is the 'nth' root. This truncates.

.shiftLeft(n)
-------------
...
```

#### <a name="apidoc.element.bignum.scompare"></a>[function <span class="apidocSignatureSpan">bignum.</span>scompare (num)](#apidoc.element.bignum.scompare)
- description and source-code
```javascript
scompare = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
}

BigNum.prototype.cmp = function (num) {
if (BigNum.isBigNum(num)) {
  return this.bcompare(num)
} else if (typeof num === 'number') {
  if (num < 0) {
    return this.scompare(num)
  } else {
    return this.ucompare(num)
  }
} else {
  var x = BigNum(num)
  return this.bcompare(x)
}
...
```

#### <a name="apidoc.element.bignum.setCompact"></a>[function <span class="apidocSignatureSpan">bignum.</span>setCompact (num)](#apidoc.element.bignum.setCompact)
- description and source-code
```javascript
setCompact = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.shiftLeft"></a>[function <span class="apidocSignatureSpan">bignum.</span>shiftLeft (num)](#apidoc.element.bignum.shiftLeft)
- description and source-code
```javascript
shiftLeft = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
Return a new 'bignum' that is the square root. This truncates.

.root(n)
-------

Return a new 'bignum' that is the 'nth' root. This truncates.

.shiftLeft(n)
-------------

Return a new 'bignum' that is the '2^n' multiple. Equivalent of the '<<'
operator.

.shiftRight(n)
--------------
...
```

#### <a name="apidoc.element.bignum.shiftRight"></a>[function <span class="apidocSignatureSpan">bignum.</span>shiftRight (num)](#apidoc.element.bignum.shiftRight)
- description and source-code
```javascript
shiftRight = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.shiftLeft(n)
-------------

Return a new 'bignum' that is the '2^n' multiple. Equivalent of the '<<'
operator.

.shiftRight(n)
--------------

Return a new 'bignum' of the value integer divided by
'2^n'. Equivalent of the '>>' operator.

.gcd(n)
-------
...
```

#### <a name="apidoc.element.bignum.sqrt"></a>[function <span class="apidocSignatureSpan">bignum.</span>sqrt (num)](#apidoc.element.bignum.sqrt)
- description and source-code
```javascript
sqrt = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

* certainly prime (true)
* probably prime ('maybe')
* certainly composite (false)

using [BN_is_prime_ex](http://www.openssl.org/docs/crypto/BN_generate_prime.html).

.sqrt()
-------

Return a new 'bignum' that is the square root. This truncates.

.root(n)
-------
...
```

#### <a name="apidoc.element.bignum.sub"></a>[function <span class="apidocSignatureSpan">bignum.</span>sub (num)](#apidoc.element.bignum.sub)
- description and source-code
```javascript
sub = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
simple.js
---------

'''js
var bignum = require('bignum');

var b = bignum('782910138827292261791972728324982')
.sub('182373273283402171237474774728373')
.div(8)
;
console.log(b);
'''

***
$ node simple.js
...
```

#### <a name="apidoc.element.bignum.toBuffer"></a>[function <span class="apidocSignatureSpan">bignum.</span>toBuffer (num)](#apidoc.element.bignum.toBuffer)
- description and source-code
```javascript
toBuffer = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.toNumber()
-----------

Turn a 'bignum' into a 'Number'. If the 'bignum' is too big you'll lose
precision or you'll get ±'Infinity'.

.toBuffer(opts)
-------------

Return a new 'Buffer' with the data from the 'bignum'.

The default options are:

'''js
...
```

#### <a name="apidoc.element.bignum.toNumber"></a>[function <span class="apidocSignatureSpan">bignum.</span>toNumber (num)](#apidoc.element.bignum.toNumber)
- description and source-code
```javascript
toNumber = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

or if x is a 'bignum' instance''

'''js
x.method(y, z)
'''

.toNumber()
-----------

Turn a 'bignum' into a 'Number'. If the 'bignum' is too big you'll lose
precision or you'll get ±'Infinity'.

.toBuffer(opts)
-------------
...
```

#### <a name="apidoc.element.bignum.tostring"></a>[function <span class="apidocSignatureSpan">bignum.</span>tostring (num)](#apidoc.element.bignum.tostring)
- description and source-code
```javascript
tostring = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
BigNum.prototype.inspect = function () {
return '<BigNum ' + this.toString(10) + '>'
}

BigNum.prototype.toString = function (base) {
var value
if (base) {
  value = this.tostring(base)
} else {
  value = this.tostring()
}
if (base > 10 && typeof value === 'string') {
  value = value.toLowerCase()
}
return value
...
```

#### <a name="apidoc.element.bignum.uadd"></a>[function <span class="apidocSignatureSpan">bignum.</span>uadd (num)](#apidoc.element.bignum.uadd)
- description and source-code
```javascript
uadd = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  return this['b' + op](num)
} else if (typeof num === 'number') {
  if (num >= 0) {
    return this['u' + op](num)
  } else if (op === 'add') {
    return this.usub(-num)
  } else if (op === 'sub') {
    return this.uadd(-num)
  } else {
    x = BigNum(num)
    return this['b' + op](x)
  }
} else if (typeof num === 'string') {
  x = BigNum(num)
  return this['b' + op](x)
...
```

#### <a name="apidoc.element.bignum.ucompare"></a>[function <span class="apidocSignatureSpan">bignum.</span>ucompare (num)](#apidoc.element.bignum.ucompare)
- description and source-code
```javascript
ucompare = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
BigNum.prototype.cmp = function (num) {
  if (BigNum.isBigNum(num)) {
    return this.bcompare(num)
  } else if (typeof num === 'number') {
    if (num < 0) {
      return this.scompare(num)
    } else {
      return this.ucompare(num)
    }
  } else {
    var x = BigNum(num)
    return this.bcompare(x)
  }
}
...
```

#### <a name="apidoc.element.bignum.udiv"></a>[function <span class="apidocSignatureSpan">bignum.</span>udiv (num)](#apidoc.element.bignum.udiv)
- description and source-code
```javascript
udiv = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.udiv2exp"></a>[function <span class="apidocSignatureSpan">bignum.</span>udiv2exp (num)](#apidoc.element.bignum.udiv2exp)
- description and source-code
```javascript
udiv2exp = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  return BigNum.prototype.shiftLeft.call(this, x)
}
}

BigNum.prototype.shiftRight = function (num) {
if (typeof num === 'number') {
  if (num >= 0) {
    return this.udiv2exp(num)
  } else {
    return this.shiftLeft(-num)
  }
} else {
  var x = parseInt(num.toString(), 10)
  return BigNum.prototype.shiftRight.call(this, x)
}
...
```

#### <a name="apidoc.element.bignum.umod"></a>[function <span class="apidocSignatureSpan">bignum.</span>umod (num)](#apidoc.element.bignum.umod)
- description and source-code
```javascript
umod = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  if ((typeof mod) === 'number' || (typeof mod) === 'string') {
    m = BigNum(mod)
  } else if (BigNum.isBigNum(mod)) {
    m = mod
  }

  if ((typeof num) === 'number') {
    return this.umod(num, m)
  } else if ((typeof num) === 'string') {
    var n = BigNum(num)
    return this.bmod(n, m)
  } else if (BigNum.isBigNum(num)) {
    return this.bmod(num, m)
  }
}
...
```

#### <a name="apidoc.element.bignum.umul"></a>[function <span class="apidocSignatureSpan">bignum.</span>umul (num)](#apidoc.element.bignum.umul)
- description and source-code
```javascript
umul = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bignum.umul2exp"></a>[function <span class="apidocSignatureSpan">bignum.</span>umul2exp (num)](#apidoc.element.bignum.umul2exp)
- description and source-code
```javascript
umul2exp = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  return BigNum.prototype.pow.call(this, x)
}
}

BigNum.prototype.shiftLeft = function (num) {
if (typeof num === 'number') {
  if (num >= 0) {
    return this.umul2exp(num)
  } else {
    return this.shiftRight(-num)
  }
} else {
  var x = parseInt(num.toString(), 10)
  return BigNum.prototype.shiftLeft.call(this, x)
}
...
```

#### <a name="apidoc.element.bignum.upow"></a>[function <span class="apidocSignatureSpan">bignum.</span>upow (num)](#apidoc.element.bignum.upow)
- description and source-code
```javascript
upow = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  return this.bmod(num, m)
}
}

BigNum.prototype.pow = function (num) {
if (typeof num === 'number') {
  if (num >= 0) {
    return this.upow(num)
  } else {
    return BigNum.prototype.powm.call(this, num, this)
  }
} else {
  var x = parseInt(num.toString(), 10)
  return BigNum.prototype.pow.call(this, x)
}
...
```

#### <a name="apidoc.element.bignum.upowm"></a>[function <span class="apidocSignatureSpan">bignum.</span>upowm (num)](#apidoc.element.bignum.upowm)
- description and source-code
```javascript
upowm = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
  if ((typeof mod) === 'number' || (typeof mod) === 'string') {
    m = BigNum(mod)
  } else if (BigNum.isBigNum(mod)) {
    m = mod
  }

  if ((typeof num) === 'number') {
    return this.upowm(num, m)
  } else if ((typeof num) === 'string') {
    var n = BigNum(num)
    return this.bpowm(n, m)
  } else if (BigNum.isBigNum(num)) {
    return this.bpowm(num, m)
  }
}
...
```

#### <a name="apidoc.element.bignum.uprime0"></a>[function <span class="apidocSignatureSpan">bignum.</span>uprime0 ()](#apidoc.element.bignum.uprime0)
- description and source-code
```javascript
function uprime0() { [native code] }
```
- example usage
```shell
...
  if (typeof safe === 'undefined') {
    safe = true
  }

  // Force uint32
  bits >>>= 0

  return BigNum.uprime0(bits, !!safe)
}

BigNum.prototype.probPrime = function (reps) {
  var n = this.probprime(reps || 10)
  return { 1: true, 0: false }[n]
}
...
```

#### <a name="apidoc.element.bignum.usub"></a>[function <span class="apidocSignatureSpan">bignum.</span>usub (num)](#apidoc.element.bignum.usub)
- description and source-code
```javascript
usub = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...
var x
if (BigNum.isBigNum(num)) {
  return this['b' + op](num)
} else if (typeof num === 'number') {
  if (num >= 0) {
    return this['u' + op](num)
  } else if (op === 'add') {
    return this.usub(-num)
  } else if (op === 'sub') {
    return this.uadd(-num)
  } else {
    x = BigNum(num)
    return this['b' + op](x)
  }
} else if (typeof num === 'string') {
...
```

#### <a name="apidoc.element.bignum.xor"></a>[function <span class="apidocSignatureSpan">bignum.</span>xor (num)](#apidoc.element.bignum.xor)
- description and source-code
```javascript
xor = function (num) {
  var args = [].slice.call(arguments, 1)

  if (BigNum.isBigNum(num)) {
    return num[name].apply(num, args)
  } else {
    var bigi = BigNum(num)
    return bigi[name].apply(bigi, args)
  }
}
```
- example usage
```shell
...

.or(n)
------

Return a new 'bignum' with the instance value bitwise inclusive-OR (|)-ed with
'n'.

.xor(n)
-------

Return a new 'bignum' with the instance value bitwise exclusive-OR (^)-ed with
'n'.

.mod(n)
-------
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
