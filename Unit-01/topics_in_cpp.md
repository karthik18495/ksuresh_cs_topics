---
layout: default
title: Selected Topics in C++
parent: Unit:01 - Compiling concepts
nav_order: 1
---

## What are `INCLUDE_GUARDS`

Include guards ensure that the headers are not called more than once during the time of project compilation.

This is very important because it can put out some errors like redeclaration errors when you run without a header guard.


Here is an example consider the code

```cpp
//Class_A.h

#include <iostream>

class A {

  private:
    string _name, int _number;

  public:

    void setValues(string Name, int Number)
    {
      _name = Name;
    _number = Number;
    }

    void printValues()
    {
      std::cout << "Name is " << _name << " and Number is " << _number << std::endl;
    }
};
```

And `Classs_B.h` as

```cpp
//Class_B.h

#include <iostream>
#include "Class_A.h"
class B {
private:
  A a;
public:
  void setValues_B(string Name, int Number)
  {
    a.setValues(Name, Number);
  }
  void printValues_B()
  {
    a.printValues();
  }
};
```

and main function defined as

```cpp
// main.cpp

#include "Class_A.h"
#include "Class_B.h"
#include <iostream>

int main()
{
  B c;
  c.SetValues("Testing", 10);
  c.printValues();
}
```


<div class="alert alert-warning" role="alert">
  <strong> :warning: Note </strong>
  Be careful since this is a warning message.
</div>
