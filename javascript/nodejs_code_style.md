# Javascript (Node.js)

* Versions: **0.8.x, 0.10.x**
* Responsible: carlos@technogi.com.mx
* Reviser: daniel@technogi.com.mx

## Introduction

This guide target [node.js](http://nodejs.org/), if you need documentation for browser based applications, please refer to the [javascript documentation (code_style.md)](http://example.com/ "cod_style.md") inline link.

Since there is no official documentation governing node.js applications...(http://nodeguide.com/style.html)


**Note:** node.js and available packages have their own styles. Those may differ from this one.

## Comments

### Header

Every javascript file MUST have a header in the following format:

```
  /**
   * Copyright: <Project Copyright>
   * 
   * <Project Name>
   * <Module> - <Component>
   * @version <version>
   * @description <description>
   * @author <author>
   * 
   * Contributors:
   *  [<email>]*
   */
```

### Functions

If a method is a part of an API or is exported as part of a module it must have the following header at the top of the function
```
  /**
   * <description of the method>
   * @param {callback} <param name> <description>
   * @return {function} <description of what the method is returning>
   * @api public 
   */
```
   

## Naming Conventions

### File names

## Code Format

### Indentation

* must use 2 spaces for every indentation
* avoid tab (configure your ide to use spaces insted of tabs)

### Brackets
