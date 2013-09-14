# Java

* versions: 1.5, 1.6 and 1.7
* Responsible: ricardo@technogi.com.mx
* Reviser: carlos@technogi.com.mx

## Comments

### Header

Every *.java, *.properties MUST have a header in the following format:

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

### Methods

In Java files, every public method must have its coment
```
  /**
   * <description of the method>
   * @param <param name> <param type> <description>
   * @return <return type> <description of what the method is returning>
   * @throws <Exception> <description> 
   */
```
   
## Naming Conventions

* Classes/Interfaces: Class names should be nouns, in mixed case with the first letter of each internal word capitalized. 
Class names should be simple and descriptive. Use whole words-avoid acronyms and try to avoid abbreviations.

```
    class TestUser{
    }

```
* Variables: Variable names should start with lower case and any subsequent word should be capitalized. Though $ and _ are 
 allowed to be used to start a variabe, it should be limited to framework standards. Variable names should be meaningful
 so that any developer knows what that variable represents.

``` 
    String firstName; 
```
  
* Methods: Method names should be verbs and should start with lowercase and any subsequent word should be capitalized.

``` 
    String doLogin( ){
    }
```

* Constants: Constant names should be uppercase and every word should be separated by underscores

```
    int TOP_LIMIT = 2809857;
```
  
  
## Format 

### Indentation
* Every code block should hace a single tab indentation more than the beginning of the code block

```
  class MyClass{
    String processCondition(boolean condition){
      if(condition){
        return "true";
      }
      else{
        return "false";
      }
    }
  }
```

### Brackets
* Brackets should start in the same line after the statement and should end in a separate line with the same indentation
of the beggining statement

```
  if('word'.equals('otherWord')){
    return true;
  }else{
    return false;
  }
```

### Line format
* Line size should be of a maximum of 80 - 90 characters so that it  is well handled by most IDEs.

* Whenever a line has to be broken, try to break it when chunks of code end (after a ',','(',')','{','}') or before a large
 statement. Subsequent lines should have 2 more tabs of indentation than the first line.

```
private static synchronized horkingLongMethodName(int anArg,
        Object anotherArg, String yetAnotherArg,
        Object andStillAnother) {
```

### Line spaces
* There should be a line space between method declarations and after the last variable declared for the code block

```
public class MyClass(){
  int variable1;
  int variable2;
  int variable3;
  
  void method1(){
    int method1Variable1 = 0;
    int method1Variable2 = 0;
    
    while(method1Variable1==methodVariable2){
      // Iteration code block
    }
  }
  
  void method2(){
    // Another method code block
  }

}
```

## Declarations

###Initialization
* Every variable shoud be declared in separate lines

### Placement
* Declare variables at the beginning of the code block you intend to use the variable

```
public class MyClass(){
  int n = 10;
  
  public int myMethod (){
    int counter = 0;
    
    for(int i=0; i<n;i++){
      counter++;
    }
    return counter;
  }
}
```
