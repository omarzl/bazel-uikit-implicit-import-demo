This project demonstrates how to implicitly import UIKit in Swift modules using a Clang module + Umbrella header
---

### How to run it?

Execute the `build.sh` script

As you can notice the classes `SomeClass` and `OtherClass` are instantiating an `UIViewController` which is part of the UIKit framework and it is being implicitly imported using the `MyLib.modulemap` and the `MyLib-umbrella.h`
