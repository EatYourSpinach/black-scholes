black-scholes
=============

Option pricing using the Black-Scholes formula.

**blackScholes(s, k, t, v, r, callPut)**
- **s** - Current price of the underlying
- **k** - Strike price
- **t** - Time to experiation in years
- **v** - Volatility as a decimal
- **r** - Anual risk-free interest rate as a decimal
- **callPut** - The type of option to be priced - "call" or "put"

Usage:
```
var bs = require("black-scholes");

console.log(bs.blackScholes(30, 34, .25, .2, .08, "call")); // 0.23834902311961947
console.log(bs.blackScholes(30, 34, .25, .2, .08, "put")); // 3.5651039155492974
```