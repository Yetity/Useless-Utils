# Useless Math Package

I mean.. Do you really need this soon to be multi mathemetically functioning package? (if that even makes sense)

## Installation

```bash
npm i @yetnt/ump
```

> _It's suggested you don't install from github itself as I'm consistently commiting to the project you'll need to update everyday and because some code breaks because i'm editing it so just get it from npm :+1:_

```js
const Ump = require("@yetnt/ump");
Ump.PrimeFactorize();
```

or

```js
const { PrimeFactorize } = require("@yetnt/ump");
PrimeFactorize();
```

## Features

So far this package can do a lot

### Prime Factorization

```js
const { PrimeFactorize } = require("@yetnt/ump");

PrimeFactorize(50); // [2, 5, 5]
PrimeFactorize(5000); // [2, 2, 2, 5, 5, 5, 5]
PrimeFactorize(93928893); // [3, 17, 103, 17881]
PrimeFactorize(3); // [3]
```

### Ratio(s)

#### Divide `x` in the ratio of `y`:`z`

```js
const { DinRatio } = require("@yetnt/ump");

DinRatio(500, 3, 2); // [300, 200]
DinRatio(456.93, 12, 5); // [ 322.5388235294118, 134.39117647058825 ]
DinRatio(456.93, 12, 5, true); // ['322.54', '134.39']
```

#### Direct Proportion (equivalent ratios)

```js
const { PropRatio } = require("@yetnt/ump");

PropRatio(2, 4, 6, true); // 12
/* 
x : y
z : ?

in this case:
2 : 4
6 : ?
*/

PropRatio(2, 6, 12); // 4
/*
x : y
? : z

in this case
2 : 6
? : 12
*/
```

### Conversion

#### Distance

```js
const { Convert, Distance } = require("@yetnt/ump");

Convert.Distance(12, Distance.Millimeter, Distance.Centimeter); // 1.2
Convert.Distance(1, Distance.Inch, Distance.Centimeter); // 2.54
Convert.Distance(98, Distance.NauticalMile, Distance.Nanometer); // 1852000000000
```

#### Area

```js
const { Convert, Area } = require("@yetnt/ump");

Convert.Area(34, Area.SquareCentimetre, Area.SquareInch); // 5.27001054002108
Convert.Area(34, "cm2", "inch2"); // 5.27001054002108
Convert.Area(490, Area.Hectare, Area.SquareFoot); // 52743183.75079384
```

#### Volume

```js
const { Convert, Volume } = require("@yetnt/ump");

Convert.Volume(34, Volume.CubicCentimeter, Volume.CubicInch); // 2.0748027411805627
Convert.Volume(34, "cm3", "inch3"); // 2.0748027411805627
Convert.Volume(490, Volume.Quart, Volume.Liter); // 463.71297
```

#### Temperature

```js
const { Convert } = require("@yetnt/ump");

Convert.Temp(1, "K", "C"); // 1 Kelvin to Celsius = -272.15
Convert.Temp(1, "Fahrenheit", "kelvin"); // 1 Fahrenheit to kelvin = 255.92777777777775
Convert.Temp(1, "c", "f"); // 1 Celsius to Fahrenheit = 33.8
```

#### Data

```js
const { Convert, Data } = require("@yetnt/ump");

Convert.Data(15, Data.Kibibyte, Data.Tebibyte); // 1.396983862272e-8
Convert.Data(20, Data.Gigabyte, Data.Kilobyte); // 20000000
Convert.Data(1, Data.Terabyte, Data.Bit); //8000000000000
```

## Releases

[Github](https://github.com/Yetity/ump/releases) \
**[Latest](https://github.com/Yetity/ump/releases/latest)**

> -   **[4.0.0](https://github.com/Yetity/ump/releases/tag/v4.0.0)**
> -   **[3.0.0](https://github.com/Yetity/ump/releases/tag/v3.0.0)**
> -   **[2.0.0](https://github.com/Yetity/ump/releases/tag/v2.0.0)**
> -   **[1.0.0](https://github.com/Yetity/ump/releases/tag/v1.0.0)**

## Links

-   [Github](https://github.com/Yetity/ump)
-   [NPM](https://npmjs.com/package/@yetnt/ump)

## Contributors

#### Main/Owner/Creator of package

-   YetNT
    -   [Discord](https://discordapp.com/users/671549251024584725)
    -   [Github](https://github.com/Yetity)
    -   [NPM](https://npmjs.com/~yetnt)

#### others

-   202291
    -   _Improved PrimeFactorize, by removing feature that does not work._
    -   _Removed Imperal V Metric terms in favour of Enums_
