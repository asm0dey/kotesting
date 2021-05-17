---
marp: true
title: "Testing with kotlin"
url: https://asm0dey.ru/p/devops-de
theme: gaia
size: 4K
class: default
paginate: true
footer: '[![](images/twitter_24.png)asm0di0](https://twitter.com/asm0di0)'
---

<style>
.hljs-variable { color: lightblue }
.hljs-string { color: lightgreen }
.hljs-params { color: #77c6d3 }
footer { color: white }
</style>
<!--
backgroundImage: "linear-gradient(to bottom, #000 0%, #1a2028 50%, #293845 100%)"
_class: lead
color: white
_paginate: false
_footer: ""
-->

# <!-- fit --> Kotest and his friends

Pasha Finkelshteyn, JetBrains


---

<!--
_class: lead
-->
## Who am I

- Developer Advocate
- Love testing
- Love learning new things
- :heart: Kotlin

---

<!--
_class: lead
-->
## What I'm talking about

- Plenty of instruments for testing
- Java has rich ecosystem
- "Proven over years" technologies

---
## What Kotlin brought into the JVM world

- DSL
- Extension methods
- Functions as 1st class citizens
---
<!--
_class: lead
-->
## <!-- fit --> And plenty of libraries!
---
<!--
_class: lead
-->
![bg brightness:0.7](https://source.unsplash.com/i--IN3cvEjg)
## <!-- fit --> But why?

---
<style scoped> p > img { display: block; margin: auto }</style>


## Current test structure

Like *this*
![width:920](images/discoworld.svg)

---
<!-- 
_class: lead
 -->
![bg brightness:0.6](images/world.jpg)
# Welcome to the Discoworld!

By Sir Terence David John Pratchett

---

<style scoped> p > img { display: block; margin: auto }</style>
## We wanna nice things!

![](images/beauty.svg)

---

<style scoped> p > img { display: block; margin: auto }</style>
## Parametrized tests. *TestNG*

![width:920](images/dataprovider.svg)

---

<style scoped> p > img { display: block; margin: auto }</style>
## Parametrized tests. *JUnit 5*

![width:920](images/junit5.svg)


---

## Still to noisy

- Annotations
- Arrays.asList *(Looks better in newer Java)*
- Strings where we will make mistakes
- Separate methods

---
<!-- _class: lead -->
<style scoped>img { filter: invert(94%) }</style>

## Tests should be easy to read

![](images/crowd.svg)

---
<!-- 
_footer: ""
_class: lead
 -->

![bg left:45% fit brightness:110%](images/sir.jpg)

# Sage of
# <!-- fit --> enterprise security

---

## We need to store passwords. How?

* Plain
* MD5(plain)
* MD5(plain+salt)
* MD5(md5(plain)+salt)

---

## We need to store passwords. How?

- Plain
- MD5(plain)
- MD5(plain+salt)
- MD5(md5(plain)+salt)

Rapid! 
**200 GH/s** @ 8x Nvidia GTX 1080 Founders Edition with *Hashcat*

---
## What should we do now??

### Cry

#### Or use bcrypt/scrypt


Hash starts with `$2a$10`

`$2a` — bcrypt version
`$10` — number of salting rounds

The are **very** slow (100/1000 per second)

---
<!-- _class: lead -->
# <!-- fit --> Kotest
## It's demo time!
---

## What should we remember

kotest solves problems od

- Structure
- Parametrized testing
- Property-based testing

---

<!-- _class: lead -->

## <!-- fit --> Thank you! Time for Q&A!

Pasha Finkelshteyn, JetBrains

[![](images/twitter_24.png)asm0di0](https://twitter.com/asm0di0)
