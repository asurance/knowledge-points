---
title: flex
date: 2021-01-26 22:05:52
tags:
---

# flex

## display
* flex
* inline-flex

## flex-direction

* **row**
* column
* row-reverse
* column
  
## flex-wrap

* **nowrap**
* wrap
* wrap-reverse

## flex-flow

<'[flex-direction](#flex-direction)'> || <'[flex-wrap](#flex-wrap)'>

## justify-content
* **flex-start**
* flex-end
* center
* space-between
* space-around

## align-items
* **stretch**
* flex-start
* flex-end
* center
* baseline

## align-content
* **stretch**
* flex-start
* flex-end
* center
* space-between
* space-around

## flex-grow
* **0**
* number

## flex-shrink
* **1**
* number

## flex-basis
* **auto**
* content
* number

## flex
<'[flex-grow](#flex-grow)'> <'[flex-shrink](#flex-shrink)'>? || <'[flex-basis](#flex-basis)'>
* **initial** -> '0 1 auto'
* auto -> '1 1 auto'
* none -> '0 0 auto'
  
## align-self
* **auto**
* flex-start
* flex-end
* center
* baseline
* stretch

## order
* **0**
* number