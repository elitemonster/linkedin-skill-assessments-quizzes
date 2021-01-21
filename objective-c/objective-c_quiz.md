## Objective-C

#### Q1. What is the value of s?
```
NSMutableString *s = [NSMutableString stringWithString: @"123"];
[s appendString: @"456"];
```
 - [x] 123456
 - [ ] 123
 - [ ] 456
 - [ ] This code contains an error.

#### Q2. What's the value of i after these statements?
```
NSString *str = nil;
NSInteger i = str.integerValue;
```
 - [x] nil
 - [ ] 0
 - [ ] -1
 - [ ] This code crashes.

#### Q3. What value is in str after this line in executed?
```
NSString str = "test" + " " + "more";
```
 - [x] This code contains an error
 - [ ] test
 - [ ] nil
 - [ ] test more

#### Q4. What does this code print?
```
    NSPredicate *p2 = [NSPredicate predicateWithBlock:^BOOL(NSString*  evaluatedObject, NSDictionary<NSString *,id> * _Nullable bindings) {
      return evaluatedObject.intValue % 2 == 0;
    }];
    NSArray *vals = @[@"1", @"2", @"3"];
    NSArray *n2 = [vals filteredArrayUsingPredicate:p2];
    NSLog(@"%@", n2.firstObject);
```
 - [x] 2
 - [ ] 1,2,3
 - [ ] 1,2
 - [ ] Nothing, since this code contains an error.

#### Q5. Property defaults include `**\_\_\_**`?
 - [x] atomic/strong
 - [ ] atomic/weak
 - [ ] nonatomic/weak
 - [ ] nonatomic/strong

#### Q6. What is the key difference between NSDictionary and NSMutableDictionary?
 - [x] NSMutableDictionary's values can change
 - [ ] NSMutableDictionary has not initializers.
 - [ ] NSDictionary can't be copied.
 - [ ] NSDictionary's values can change.

#### Q7. What is foo?
```
-(float)foo;
```
 - [x] A function with a return type of float.
 - [ ] This code contains an error.
 - [ ] A variable declaration of type float.
 - [ ] A property of type float.

#### Q8. What can you glean from this line?
```
#import "NSString+NameHelper.h"
```
 - [x] NameHelper is a category of NSString.
 - [ ] NameHelper is a subclass of NSString.
 - [ ] NSString implements the NameHelper protocol.
 - [ ] NSString has a helper class.

#### Q9. What's wrong with this code?
```
float x = 5.;
```
 - [x] Nothing is wrong with this code.
 - [ ] Declarations do not need semicolons.
 - [ ] x=5 is an invalid float.
 - [ ] Variables can't be declared and initialized in the same state.

#### Q10. How many times with this loop be executed?
```
for (int x=0; x<100; x++) {
  x = x + 1;
}
```
 - [x] 50
 - [ ] 99
 - [ ] 100
 - [ ] This code contains an error.

#### Q11. What is this code an example of?
```
[self addObserver: self forKeyPath: @"val" options:0 context: nil];
```
 - [ ] Key-Value Observing
 - [ ] Class Value Observing
 - [ ] Key-Data Observing
 - [ ] KeyPath Observing

#### Q12. What does ARC stand for?
 - [x] Automatic Reference Counting
 - [ ] Automatic Retain Checking
 - [ ] Async Retain Cycles
 - [ ] Automatic Release Code

#### Q13. What is printed for this code?
```
int val = 0;
val = 1.5;
printf("%d", val);
```
 - [x] 1
 - [ ] 2
 - [ ] 0
 - [ ] This code contains an error.

#### Q14. What best describes class inheritance in Objective-C?
 - [ ] single inheritance but multiple protocol implementation
 - [ ] Objective-C doesn't support inheritance
 - [ ] dual class inheritance
 - [ ] unlimited class inheritance and protocol adherence

#### Q15. How many keys does this NSDictionary have after this code is executed?
```
NSDictionary *dict = [[NSDictionary alloc] initWithObjectsAndKeys: @"b", @"e", @"a", @"r", nil];
```
 - [x] 2
 - [ ] 4
 - [ ] 5
 - [ ] This code contains an error.

#### Q16. What is wrong with this code?
```
NSMutableDictionary *dict1 = [NSMutableDictionary dictionaryWithCapacity:5];
[dict1 setValue:@"key" forKey:@"value"];
```
 - [x] The key and value items are mixed
 - [ ] Nothing is wrong with it
 - [ ] You can't set the capacity of a dictionary
 - [ ] NSMutableDictionary doesn't have a :setValue:forKey function.

#### Q17. What is printed from this code?
```
NSData *data = [@"print" dataUsingEncoding:NSASCIIStringEncoding];
NSLog(@"%@", [[NSString alloc] initWithData:data encoding:NSASCIIStringEncoding]);
```
 - [x] print
 - [ ] This code is invalid
 - [ ] Nothing is printed from this code.
 - [ ] nil

#### Q18. What is different about this function?
```
+(void)doSomething;
```
 - [x] It is static
 - [ ] It is abstract.
 - [ ] It is inline.
 - [ ] This code contains an error.

#### Q19. Structs can have `**\_\_\_**`?
 - [x] functions
 - [ ] initializers
 - [ ] fields
 - [ ] all of these answers

#### Q20. What is wrong with this code?
```
@interface MyClass : NSObject
    @property (strong, nonatomic, readonly) NSString *name;
  @end
```
 - [x] There is nothing wrong with this code.
 - [ ] There is not read-only directive.
 - [ ] MyClass doesn't implement NSObject.
 - [ ] Properties are declared in the implementation.

#### Q21. What is wrong with this code?
```
NSArray *vals = @[@"1", @"2", @"3"];
NSPredicate *pred = [NSPredicate predicateWithFormat:@"SELF.intValue > 1"];
NSArray *newValues = [vals filteredArrayUsingPredicate:pred];
```
 - [x] 2,3
 - [ ] nil
 - [ ] 2,"3"
 - [ ] This code contains an error.

#### Q22. What is an enums base type for the code below?
```
typedef enum { Foo1, Foo2} Foo;
```
 - [x] There is no base type.
 - [ ] NSObject
 - [ ] int
 - [ ] NSNumber

#### Q23. If you want to store a small amount of information (e.g., user settings), whats the best, built-in way to go?
 - [x] UserDefaults
 - [ ] plist file
 - [ ] CoreData
 - [ ] TextFile

#### Q24. What are categories used for?
 - [x] to extend other classes
 - [ ] to manage access control
 - [ ] to coordinate objects
 - [ ] to group classes

#### Q25. What is this Objective-C code checking?
```
if ([keyPath isInstanceOf:[NSString class]]) {
}
```
 - [x] This code contains an error
 - [ ] if keyPath is an instance of NSString
 - [ ] if keyPath's baseclass is the same as NSString's baseclass
 - [ ] if keyPath implements the same methods as NSString

#### Q26. What is this a declaration of?
```
int(^foo)(int);
```
 - [ ] an Extension
 - [ ] a Generic
 - [ ] a block of code
 - [ ] an abstract class

#### Q27. For observing changes to a property, which of these two statements cause the related method to be called and why?
```
1. _val = 1;
2. self.val= 100;
```
 - [ ] Statement 2, since it calls the auto-created setter on the property.
 - [ ] Statement 1, since it uses the property directly.
 - [ ] Statement 2, since it specifies the class instance to use.
 - [ ] Statement 1, since it calls the auto-created setter on the property.

#### Q28. What is wrong with this code?
```
float x = 2.0;
int(^foo)(int) = ^(int n1) {
  return (int)(n1*x);
};
foo(5);
```
 - [ ] Ints and floats can't be multiplied.
 - [ ] The parameter isn't declared correctly.
 - [ ] x is not in the right scope.
 - [ ] Nothing is wrong with this code.

#### Q29. What's the difference between an array and a set?
 - [ ] Arrays are ordered, non-unique values.
 - [ ] Arrays are stored sorted.
 - [ ] Sets are ordered, unique values.
 - [ ] Sets can contain nils.

#### Q30. Dot notation can be used for `**\_\_\_**`?
 - [ ] nothing, as they're never used in Objective-C
 - [ ] function calls only
 - [ ] property getter/setter
 - [ ] parameter delimiters

#### Q31. What is the value of newVals after this code is executed?

    NSArray *vals = @[@"1", @"2", @"3"];
    NSPredicate *pred = [NSPredicate predicateWithFormat:@"SELF.intValue > 1"];
    NSArray \*newVals = [vals filteredArrayUsingPredicate:pred];

 - [x] 2,3
 - [ ] nil
 - [ ] This code contains an error
 - [ ] 2,"3"

#### Q32. How would this funciton be called?
`-(int)foo:(int)a b:(int)c;`
 - [ ] self.foo(5, b:10);
 - [ ] This code contains an error.
 - [ ] [self foo:5:10:20];
 - [ ] [self foo:5 b:10];

#### Q33. What is the type of the error return value stored in json?

    NSERROR *error;
    NSData *data;
    id json = [NSJSONSerialization JSONObjectWithData:data opetions:NSJSONReadingAllowFragments error:&error];

 - [ ] NSString
 - [ ] NSArray
 - [ ] id
 - [ ] NSDictionary
