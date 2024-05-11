<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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

# Iterators

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Iterator utilities.

<section class="installation">

## Installation

```bash
npm install @micromint1npm/est-doloribus-officiis
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@micromint1npm/est-doloribus-officiis' );
```

#### ns

Namespace containing iterator utilities.

```javascript
var objectKeys = require( '@stdlib/utils/keys' );

var keys = objectKeys( ns );
// e.g., returns [ 'iterAny', 'iterAnyBy', ... ]
```

<!-- <toc pattern="*"> -->

<div class="namespace-toc">

-   <span class="signature">[`iterAdvance( iterator[, n] )`][@micromint1npm/est-doloribus-officiis/advance]</span><span class="delimiter">: </span><span class="description">advance an iterator.</span>
-   <span class="signature">[`iterAnyBy( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/any-by]</span><span class="delimiter">: </span><span class="description">test whether at least one iterated value passes a test implemented by a predicate function.</span>
-   <span class="signature">[`iterAny( iterator )`][@micromint1npm/est-doloribus-officiis/any]</span><span class="delimiter">: </span><span class="description">test whether at least one iterated value is truthy.</span>
-   <span class="signature">[`iterConcat( iter0, ...iterator )`][@micromint1npm/est-doloribus-officiis/concat]</span><span class="delimiter">: </span><span class="description">create an iterator which iterates over the values of two or more iterators.</span>
-   <span class="signature">[`iterConstant( value[, options] )`][@micromint1npm/est-doloribus-officiis/constant]</span><span class="delimiter">: </span><span class="description">create an iterator which always returns the same value.</span>
-   <span class="signature">[`iterCounter( iterator )`][@micromint1npm/est-doloribus-officiis/counter]</span><span class="delimiter">: </span><span class="description">create an iterator which iteratively computes the number of iterated values.</span>
-   <span class="signature">[`iterDatespace( start, stop[, N][, options] )`][@micromint1npm/est-doloribus-officiis/datespace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced dates over a specified interval.</span>
-   <span class="signature">[`iterDedupeBy( iterator, [limit,] fcn )`][@micromint1npm/est-doloribus-officiis/dedupe-by]</span><span class="delimiter">: </span><span class="description">create an iterator which removes consecutive values that resolve to the same value according to a provided function.</span>
-   <span class="signature">[`iterDedupe( iterator[, limit] )`][@micromint1npm/est-doloribus-officiis/dedupe]</span><span class="delimiter">: </span><span class="description">create an iterator which removes consecutive duplicated values.</span>
-   <span class="signature">[`iterEmpty()`][@micromint1npm/est-doloribus-officiis/empty]</span><span class="delimiter">: </span><span class="description">create an empty iterator.</span>
-   <span class="signature">[`iterEveryBy( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/every-by]</span><span class="delimiter">: </span><span class="description">test whether every iterated value passes a test implemented by a predicate function.</span>
-   <span class="signature">[`iterEvery( iterator )`][@micromint1npm/est-doloribus-officiis/every]</span><span class="delimiter">: </span><span class="description">test whether all iterated values are truthy.</span>
-   <span class="signature">[`iterFill( iterator, value[, begin[, end]] )`][@micromint1npm/est-doloribus-officiis/fill]</span><span class="delimiter">: </span><span class="description">create an iterator which replaces all values from a provided iterator from a start index to an end index with a static value.</span>
-   <span class="signature">[`iterFilterMap( iterator, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/filter-map]</span><span class="delimiter">: </span><span class="description">create an iterator which both filters and maps the values of another iterator.</span>
-   <span class="signature">[`iterFilter( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/filter]</span><span class="delimiter">: </span><span class="description">create an iterator which filters the values of another iterator according to a predicate function.</span>
-   <span class="signature">[`iterFirst( iterator )`][@micromint1npm/est-doloribus-officiis/first]</span><span class="delimiter">: </span><span class="description">return the first iterated value.</span>
-   <span class="signature">[`iterFlow( methods )`][@micromint1npm/est-doloribus-officiis/flow]</span><span class="delimiter">: </span><span class="description">create a fluent interface for chaining together iterator methods.</span>
-   <span class="signature">[`iterForEach( iterator, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/for-each]</span><span class="delimiter">: </span><span class="description">create an iterator which invokes a function for each iterated value before returning the iterated value.</span>
-   <span class="signature">[`iterHead( iterator, n )`][@micromint1npm/est-doloribus-officiis/head]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the first `n` values of a provided iterator.</span>
-   <span class="signature">[`iterIncrspace( start, stop[, increment] )`][@micromint1npm/est-doloribus-officiis/incrspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers according to a specified increment.</span>
-   <span class="signature">[`iterIntersectionByHash( iter0, ...iterator, hashFcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/intersection-by-hash]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the intersection of two or more iterators according to a hash function.</span>
-   <span class="signature">[`iterIntersection( iter0, ...iterator )`][@micromint1npm/est-doloribus-officiis/intersection]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the intersection of two or more iterators.</span>
-   <span class="signature">[`iterLast( iterator )`][@micromint1npm/est-doloribus-officiis/last]</span><span class="delimiter">: </span><span class="description">consume an entire iterator and return the last iterated value.</span>
-   <span class="signature">[`iterLength( iterator )`][@micromint1npm/est-doloribus-officiis/length]</span><span class="delimiter">: </span><span class="description">return an iterator's length.</span>
-   <span class="signature">[`iterLinspace( start, stop[, N] )`][@micromint1npm/est-doloribus-officiis/linspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers over a specified interval.</span>
-   <span class="signature">[`iterLogspace( start, stop[, N][, options] )`][@micromint1npm/est-doloribus-officiis/logspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers over a specified interval.</span>
-   <span class="signature">[`iterMap( iterator, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/map]</span><span class="delimiter">: </span><span class="description">create an iterator which invokes a function for each iterated value.</span>
-   <span class="signature">[`iterMapN( iter0, ...iterator, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/mapn]</span><span class="delimiter">: </span><span class="description">create an iterator which transforms iterated values from two or more iterators by applying the iterated values as arguments to a provided function.</span>
-   <span class="signature">[`iterNoneBy( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/none-by]</span><span class="delimiter">: </span><span class="description">test whether every iterated value fails a test implemented by a predicate function.</span>
-   <span class="signature">[`iterNone( iterator )`][@micromint1npm/est-doloribus-officiis/none]</span><span class="delimiter">: </span><span class="description">test whether all iterated values are falsy.</span>
-   <span class="signature">[`iterNth( iterator, n )`][@micromint1npm/est-doloribus-officiis/nth]</span><span class="delimiter">: </span><span class="description">return the nth iterated value.</span>
-   <span class="signature">[`iterThunk( iterFcn[, ...args] )`][@micromint1npm/est-doloribus-officiis/pipeline-thunk]</span><span class="delimiter">: </span><span class="description">create an iterator "thunk".</span>
-   <span class="signature">[`iterPipeline( iterFcn0[, ...iterFcn] )`][@micromint1npm/est-doloribus-officiis/pipeline]</span><span class="delimiter">: </span><span class="description">create an iterator pipeline.</span>
-   <span class="signature">[`iterPop( iterator[, clbk[, thisArg]] )`][@micromint1npm/est-doloribus-officiis/pop]</span><span class="delimiter">: </span><span class="description">create an iterator which skips the last value of a provided iterator.</span>
-   <span class="signature">[`iterPush( iterator, ...items )`][@micromint1npm/est-doloribus-officiis/push]</span><span class="delimiter">: </span><span class="description">create an iterator which appends additional values to the end of a provided iterator.</span>
-   <span class="signature">[`iterReject( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/reject]</span><span class="delimiter">: </span><span class="description">create an iterator which rejects the values of another iterator according to a predicate function.</span>
-   <span class="signature">[`iterReplicateBy( iterator, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/replicate-by]</span><span class="delimiter">: </span><span class="description">create an iterator which replicates each iterated value according to a provided function.</span>
-   <span class="signature">[`iterReplicate( iterator, n )`][@micromint1npm/est-doloribus-officiis/replicate]</span><span class="delimiter">: </span><span class="description">create an iterator which replicates each iterated value a specified number of times.</span>
-   <span class="signature">[`iterShift( iterator[, clbk[, thisArg]] )`][@micromint1npm/est-doloribus-officiis/shift]</span><span class="delimiter">: </span><span class="description">create an iterator which skips the first value of a provided iterator.</span>
-   <span class="signature">[`iterSlice( iterator[, begin[, end]] )`][@micromint1npm/est-doloribus-officiis/slice]</span><span class="delimiter">: </span><span class="description">create an iterator which returns a subsequence of iterated values from a provided iterator.</span>
-   <span class="signature">[`iterSomeBy( iterator, n, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/some-by]</span><span class="delimiter">: </span><span class="description">test whether at least `n` iterated values pass a test implemented by a predicate function.</span>
-   <span class="signature">[`iterSome( iterator, n )`][@micromint1npm/est-doloribus-officiis/some]</span><span class="delimiter">: </span><span class="description">test whether at least `n` iterated values are truthy.</span>
-   <span class="signature">[`iterStep( start, increment[, N] )`][@micromint1npm/est-doloribus-officiis/step]</span><span class="delimiter">: </span><span class="description">create an iterator which returns a sequence of numbers according to a specified increment.</span>
-   <span class="signature">[`iterStridedBy( iterator, fcn[, offset[, eager]][, thisArg] )`][@micromint1npm/est-doloribus-officiis/strided-by]</span><span class="delimiter">: </span><span class="description">create an iterator which steps according to a provided callback function.</span>
-   <span class="signature">[`iterStrided( iterator, stride[, offset[, eager]] )`][@micromint1npm/est-doloribus-officiis/strided]</span><span class="delimiter">: </span><span class="description">create an iterator which steps by a specified amount.</span>
-   <span class="signature">[`iterator2arrayviewRight( iterator, dest[, begin[, end]][, mapFcn[, thisArg]] )`][@micromint1npm/est-doloribus-officiis/to-array-view-right]</span><span class="delimiter">: </span><span class="description">fill an array-like object view from right to left with values returned from an iterator.</span>
-   <span class="signature">[`iterator2arrayview( iterator, dest[, begin[, end]][, mapFcn[, thisArg]] )`][@micromint1npm/est-doloribus-officiis/to-array-view]</span><span class="delimiter">: </span><span class="description">fill an array-like object view with values returned from an iterator.</span>
-   <span class="signature">[`iterUnion( iter0, ...iterator )`][@micromint1npm/est-doloribus-officiis/union]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the union of two or more iterators.</span>
-   <span class="signature">[`iterUniqueByHash( iterator, hashFcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/unique-by-hash]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values according to a hash function.</span>
-   <span class="signature">[`iterUniqueBy( iterator, predicate[, thisArg] )`][@micromint1npm/est-doloribus-officiis/unique-by]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values according to a predicate function.</span>
-   <span class="signature">[`iterUnique( iterator )`][@micromint1npm/est-doloribus-officiis/unique]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values.</span>
-   <span class="signature">[`iterUnitspace( start[, stop] )`][@micromint1npm/est-doloribus-officiis/unitspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns numbers incremented by `1`.</span>
-   <span class="signature">[`iterUnshift( iterator, ...items )`][@micromint1npm/est-doloribus-officiis/unshift]</span><span class="delimiter">: </span><span class="description">create an iterator which prepends values to the beginning of a provided iterator.</span>
-   <span class="signature">[`whileEach( iterator, predicate, fcn[, thisArg] )`][@micromint1npm/est-doloribus-officiis/while-each]</span><span class="delimiter">: </span><span class="description">create an iterator which, while a test condition is true, invokes a function for each iterated value before returning the iterated value.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var uncapitalize = require( '@stdlib/string/uncapitalize' );
var replace = require( '@stdlib/string/replace' );
var contains = require( '@stdlib/assert/contains' );
var randu = require( '@stdlib/random/iter/randu' );
var ns = require( '@micromint1npm/est-doloribus-officiis' );

// Create a fluent interface for chaining together iterator operations...

// Retrieve all the iterator utility names:
var keys = objectKeys( ns );

// Define a list of utilities to exclude from the fluent API:
var exclude = [ 'iterFlow', 'iterPipeline', 'iterThunk' ];

// Map each utility name to a fluent interface method...
var methods = {};
var key;
var k;
var i;
for ( i = 0; i < keys.length; i++ ) {
    key = keys[ i ];
    if ( contains( exclude, key ) ) {
        continue;
    }
    k = uncapitalize( replace( key, /^iter/, '' ) );
    methods[ k ] = ns[ key ];
}

// Create a fluent interface:
var FluentIterator = ns.iterFlow( methods );

// Create a new fluent interface iterator:
var it1 = new FluentIterator( randu() );

// Define a predicate function for filtering values:
function predicate( v ) {
    return ( v > 0.25 && v < 0.75 );
}

// Define a function which transforms iterated values:
function transform( v ) {
    return v * 10.0;
}

// Define a function to be invoked for each iterated value:
function log( v ) {
    console.log( v );
}

// Chain together a sequence of operations:
var it2 = it1.filter( predicate )
    .map( transform )
    .head( 10 )
    .forEach( log );

// Perform manual iteration...
var v;
while ( true ) {
    v = it2.next();
    if ( v.done ) {
        break;
    }
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@micromint1npm/est-doloribus-officiis.svg
[npm-url]: https://npmjs.org/package/@micromint1npm/est-doloribus-officiis

[test-image]: https://github.com/micromint1npm/est-doloribus-officiis/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/micromint1npm/est-doloribus-officiis/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/micromint1npm/est-doloribus-officiis/main.svg
[coverage-url]: https://codecov.io/github/micromint1npm/est-doloribus-officiis?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/micromint1npm/est-doloribus-officiis.svg
[dependencies-url]: https://david-dm.org/micromint1npm/est-doloribus-officiis/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/micromint1npm/est-doloribus-officiis/tree/deno
[deno-readme]: https://github.com/micromint1npm/est-doloribus-officiis/blob/deno/README.md
[umd-url]: https://github.com/micromint1npm/est-doloribus-officiis/tree/umd
[umd-readme]: https://github.com/micromint1npm/est-doloribus-officiis/blob/umd/README.md
[esm-url]: https://github.com/micromint1npm/est-doloribus-officiis/tree/esm
[esm-readme]: https://github.com/micromint1npm/est-doloribus-officiis/blob/esm/README.md
[branches-url]: https://github.com/micromint1npm/est-doloribus-officiis/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/micromint1npm/est-doloribus-officiis/main/LICENSE

<!-- <toc-links> -->

[@micromint1npm/est-doloribus-officiis/advance]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/advance

[@micromint1npm/est-doloribus-officiis/any-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/any-by

[@micromint1npm/est-doloribus-officiis/any]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/any

[@micromint1npm/est-doloribus-officiis/concat]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/concat

[@micromint1npm/est-doloribus-officiis/constant]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/constant

[@micromint1npm/est-doloribus-officiis/counter]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/counter

[@micromint1npm/est-doloribus-officiis/datespace]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/datespace

[@micromint1npm/est-doloribus-officiis/dedupe-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/dedupe-by

[@micromint1npm/est-doloribus-officiis/dedupe]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/dedupe

[@micromint1npm/est-doloribus-officiis/empty]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/empty

[@micromint1npm/est-doloribus-officiis/every-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/every-by

[@micromint1npm/est-doloribus-officiis/every]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/every

[@micromint1npm/est-doloribus-officiis/fill]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/fill

[@micromint1npm/est-doloribus-officiis/filter-map]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/filter-map

[@micromint1npm/est-doloribus-officiis/filter]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/filter

[@micromint1npm/est-doloribus-officiis/first]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/first

[@micromint1npm/est-doloribus-officiis/flow]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/flow

[@micromint1npm/est-doloribus-officiis/for-each]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/for-each

[@micromint1npm/est-doloribus-officiis/head]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/head

[@micromint1npm/est-doloribus-officiis/incrspace]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/incrspace

[@micromint1npm/est-doloribus-officiis/intersection-by-hash]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/intersection-by-hash

[@micromint1npm/est-doloribus-officiis/intersection]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/intersection

[@micromint1npm/est-doloribus-officiis/last]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/last

[@micromint1npm/est-doloribus-officiis/length]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/length

[@micromint1npm/est-doloribus-officiis/linspace]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/linspace

[@micromint1npm/est-doloribus-officiis/logspace]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/logspace

[@micromint1npm/est-doloribus-officiis/map]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/map

[@micromint1npm/est-doloribus-officiis/mapn]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/mapn

[@micromint1npm/est-doloribus-officiis/none-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/none-by

[@micromint1npm/est-doloribus-officiis/none]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/none

[@micromint1npm/est-doloribus-officiis/nth]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/nth

[@micromint1npm/est-doloribus-officiis/pipeline-thunk]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/pipeline-thunk

[@micromint1npm/est-doloribus-officiis/pipeline]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/pipeline

[@micromint1npm/est-doloribus-officiis/pop]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/pop

[@micromint1npm/est-doloribus-officiis/push]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/push

[@micromint1npm/est-doloribus-officiis/reject]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/reject

[@micromint1npm/est-doloribus-officiis/replicate-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/replicate-by

[@micromint1npm/est-doloribus-officiis/replicate]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/replicate

[@micromint1npm/est-doloribus-officiis/shift]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/shift

[@micromint1npm/est-doloribus-officiis/slice]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/slice

[@micromint1npm/est-doloribus-officiis/some-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/some-by

[@micromint1npm/est-doloribus-officiis/some]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/some

[@micromint1npm/est-doloribus-officiis/step]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/step

[@micromint1npm/est-doloribus-officiis/strided-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/strided-by

[@micromint1npm/est-doloribus-officiis/strided]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/strided

[@micromint1npm/est-doloribus-officiis/to-array-view-right]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/to-array-view-right

[@micromint1npm/est-doloribus-officiis/to-array-view]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/to-array-view

[@micromint1npm/est-doloribus-officiis/union]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/union

[@micromint1npm/est-doloribus-officiis/unique-by-hash]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/unique-by-hash

[@micromint1npm/est-doloribus-officiis/unique-by]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/unique-by

[@micromint1npm/est-doloribus-officiis/unique]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/unique

[@micromint1npm/est-doloribus-officiis/unitspace]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/unitspace

[@micromint1npm/est-doloribus-officiis/unshift]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/unshift

[@micromint1npm/est-doloribus-officiis/while-each]: https://github.com/micromint1npm/est-doloribus-officiis/tree/main/while-each

<!-- </toc-links> -->

</section>

<!-- /.links -->
