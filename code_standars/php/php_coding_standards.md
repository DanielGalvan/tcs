# PHP

* versions: 5.x
* Responsible: daniel.galvan@technogi.com.mx
* Reviser: ricardo.hernandez@technogi.com.mx

# Basic Coding Standard

Standard coding elements that are required to ensure a high level of technical interoperability between shared PHP code.

1. Overview
-----------

- Files MUST use only `<?php` tags.
- Files MUST use only UTF-8 without BOM for PHP code.
- Files MUST have a documentation header.
- Class names MUST be declared in `StudlyCaps`.
- Classes MUST have a documentation header.
- Class constants MUST be declared in all upper case with underscore separators.
- Method names MUST be declared in `camelCase`.
- Methods MUST have a documentation header.
- Coding Style.

2. Files
--------

### 2.1. PHP Tags

PHP code MUST use the long `<?php ?>` tags ; it MUST NOT use the other tag variations.

### 2.2. Character Encoding

PHP code MUST use only UTF-8 without BOM.

### 2.3. File Header

Every *.php file MUST have a header in the following format:

```
  /**
   * Copyright: <Project Copyright>
   * 
   * <Project Name>
   * <Module> - <Component>
   * @author <author>
   * @version <version>
   * @description <description>
   * 
   * Contributors:
   *  [<email>]
   */
```


3. Classes
----------

Each class is in a file by itself.

### 3.1. Class Names

Class names MUST be declared in `StudlyCaps`.

For example:

```
<?php
class Foo
{
  // code here
}
```

### 3.2. Class Header

Every php class MUST have a header in the following format:

```
  /**
   * Copyright: <Project Copyright>
   * 
   * <Project Name>
   * <Module> - <Component>
   * @name <class name>
   * @author <author>
   * @version <version>
   * @property <property type> <property name> <description>
   *
   * @description <description>
   * 
   * Contributors:
   *  [<email>]
   */
```

4. Class Constants, Properties, and Methods
-------------------------------------------

The term "class" refers to all classes, interfaces, and traits.

### 4.1. Constants

Constant names should be uppercase and every word should be separated by underscores

For example:

```php
<?php
class Foo
{
    const VERSION = '1.0';
    const DATE_APPROVED = '2013-09-20';
}
```

### 4.2. Properties

Property names MUST be declared in `camelCase()`.

### 4.3. Methods

Method names MUST be declared in `camelCase()`.

Every method must have a documentation header in the following format:

```
  /**
   * <description of the method>
   *
   * @param <param type> <param name> <description>
   * @return <return type> <description of what the method is returning>
   * @throws <Exception> <description> 
   */
```

5. Coding Style
---------------

### 5.1. Files

All PHP files MUST use the Unix LF (linefeed) line ending.

All PHP files MUST end with a single blank line.

The closing ?> tag MUST be omitted from files containing only PHP.

### 5.2. Lines

The soft limit on line length MUST be 120 characters; lines SHOULD be 80 characters or less.

### 5.3. Indenting

Code MUST use an indent of 4 spaces, and MUST NOT use tabs for indenting.

### 5.4. Keywords and True/False/Null

The PHP constants true, false, and null MUST be in lower case.

### 5.5. Properties

Visibility MUST be declared on all properties.

The var keyword MUST NOT be used to declare a property.

There MUST NOT be more than one property declared per statement.

Property names SHOULD NOT be prefixed with a single underscore to indicate protected or private visibility.

### 5.6. Methods

Visibility MUST be declared on all methods.

Method names SHOULD NOT be prefixed with a single underscore to indicate protected or private visibility.

Method names MUST NOT be declared with a space after the method name. The opening brace MUST go on its own line, and the closing brace MUST go on the next line following the body.
There MUST NOT be a space after the opening parenthesis, and there MUST NOT be a space before the closing parenthesis.

### 5.7. Method Arguments

In the argument list, there MUST NOT be a space before each comma, and there MUST be one space after each comma.

Method arguments with default values MUST go at the end of the argument list.

### 5.8. Control Structures

The general style rules for control structures are as follows:

- There MUST be one space after the control structure keyword
- There MUST NOT be a space after the opening parenthesis
- There MUST NOT be a space before the closing parenthesis
- There MUST be one space between the closing parenthesis and the opening brace
- The structure body MUST be indented once
- The closing brace MUST be on the next line after the body
- The body of each structure MUST be enclosed by braces.

### 5.8.1. `if`, `elseif`, `else`

An `if` structure looks like the following. Note the placement of parentheses,
spaces, and braces; and that `else` and `elseif` are on the same line as the
closing brace from the earlier body.

```php
<?php
if ($expr1) {
    // if body
} elseif ($expr2) {
    // elseif body
} else {
    // else body;
}
```
The keyword `elseif` SHOULD be used instead of `else if` so that all control
keywords look like single words.


### 5.8.2 `for`

A `for` statement looks like the following. Note the placement of parentheses,
spaces, and braces.

```php
<?php
for ($i = 0; $i < 10; $i++) {
    // for body
}
```

