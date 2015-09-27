---
title       : Calculating area of Nozzle
subtitle    : 
author      : Harikrishnan Murali
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Nozzle

* A nozzle is often a pipe or tube of varying cross sectional area, and it can be used to direct or modify the flow of a fluid (liquid or gas). 

* Nozzles are frequently used to control the rate of flow, speed, direction, mass, shape, and/or the pressure of the stream that emerges from them. 

* In nozzle velocity of fluid increases on the expense of its pressure energy.


--- .class #id 

## Geometry

* The nozzle in question here is a supersonic diverging nozzle. 

* It converts a low speed fluid flow into a flow faster than the speed of sound.

![alt text] (http://www.potto.org/gasDynamics/img217.png)


---

## Necessity of the App

* The nozzle geometry results in the formation a region where there is an abrupt conversion of fluid velocity.

* This is called a shockwave.

* This region is of utmost importance to fluid dynamicists. 

* The area of the nozzle's cross section is the first step towards calculating the location of the shock.

---

## How it works

* It uses the formula 

$$A(x)=1.398 + 0.347\tanh(0.8x-4)$$

where $A(x)$ is the area at a particular distance $x$.


```r
##If x=1, then
x=1
A=1.398 +0.347*tanh(0.8*x-4)
print(A)
```

```
## [1] 1.052151
```

---






