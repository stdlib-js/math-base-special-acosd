<!--

@license Apache-2.0

Copyright (c) 2024 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# acosd

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [arccosine][arccosine] in degrees of a double-precision floating-point number.



<section class="usage">

## Usage

```javascript
import acosd from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acosd@deno/mod.js';
```

#### acosd( x )

Computes the [arccosine][arccosine] (in degrees) of a double-precision floating-point number.

```javascript
import sqrt from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-sqrt@deno/mod.js';
var v = acosd( 0.0 );
// returns 90.0

v = acosd( 0.5 );
// returns ~60.0

v = acosd( sqrt( 2 ) / 2 );
// returns ~45.0

v = acosd( sqrt( 3 ) / 2 );
// returns ~30.0

v = acosd( NaN );
// returns NaN
```

The domain of `x` is restricted to `[-1,1]`. If `|x| > 1`, the function returns `NaN`.

```javascript
var v = acosd( -3.14 );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import linspace from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@deno/mod.js';
import acosd from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-acosd@deno/mod.js';

var x = linspace( -1.0, 1.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( acosd( x[ i ] ) );
}
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/acos`][@stdlib/math/base/special/acos]</span><span class="delimiter">: </span><span class="description">compute the arccosine of a double-precision floating-point number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/acosh`][@stdlib/math/base/special/acosh]</span><span class="delimiter">: </span><span class="description">compute the hyperbolic arccosine of a double-precision floating-point number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/asind`][@stdlib/math/base/special/asind]</span><span class="delimiter">: </span><span class="description">compute the arcsine (in degrees) of a double-precision floating-point number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/atand`][@stdlib/math/base/special/atand]</span><span class="delimiter">: </span><span class="description">compute the arctangent(in degrees) of a double-precision floating-point number.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2025. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-acosd.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-acosd

[test-image]: https://github.com/stdlib-js/math-base-special-acosd/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-acosd/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-acosd/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-acosd?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-acosd.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-acosd/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-acosd/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-acosd/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-acosd/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-acosd/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-acosd/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-acosd/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-acosd/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-acosd/main/LICENSE

[arccosine]: https://en.wikipedia.org/wiki/Inverse_trigonometric_functions

<!-- <related-links> -->

[@stdlib/math/base/special/acos]: https://github.com/stdlib-js/math-base-special-acos/tree/deno

[@stdlib/math/base/special/acosh]: https://github.com/stdlib-js/math-base-special-acosh/tree/deno

[@stdlib/math/base/special/asind]: https://github.com/stdlib-js/math-base-special-asind/tree/deno

[@stdlib/math/base/special/atand]: https://github.com/stdlib-js/math-base-special-atand/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
