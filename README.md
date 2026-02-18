# libfixmath
Fixed point arithmetic library from Wikipedia article https://en.wikipedia.org/wiki/Libfixmath. The library support Q15.16 fixed point number only.

## Credits
### Developer: Ben Brewer
### Stable release: r64 / February 2, 2012
### License: MIT
### Website: https://code.google.com/p/libfixmath
### Repository: https://code.google.com/p/libfixmath/source/default/source

## Authors description
Cross Platform Fixed Point Maths Library

This is a tried and tested cross platform fixed point maths library.

This library implements the math.h functions in fixed point (Q15.16) format, a subset of the currently supported functions are: * sin, cos, tan * asin, acos, atan, atan2 * sqrt, exp * mul, div * sadd, ssub, smul, sdiv (saturated arithmetic)

## Function Reference

### Conversion Functions

Conversion from integers and floating point values. These conversions retain the numeric value and perform rounding where necessary.

* fix16_from_int(a) Simply multiplies a by fix16_one = 65536
* fix16_to_int(a) Divides by fix16_one and rounds to nearest integer.
* fix16_from_float(a) Multiplies by fix16_one and rounds to nearest value.
* fix16_to_float(a) Divides by fix16_one. Rounding is according to the current floating point mode.
* fix16_from_dbl(a) Multiplies by fix16_one and rounds to nearest value.
* fix16_to_dbl(a) Divides by fix16_one. All fix16_t values fit into a double, so no rounding happens.
* fix16_from_str(buf) Converts from string to fix16_t.
* fix16_to_str(value, buf, decimals) Converts from fix16_t to string.
