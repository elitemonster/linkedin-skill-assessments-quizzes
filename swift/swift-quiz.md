## Swift

#### Q1. What is this code an example of?
```
let val = (Double)6
```
 - [x] an error
 - [ ] typecasting
 - [ ] assignment
 - [ ] initialization

#### Q2. What is the error in this code?
```
let x = 5
guard x == 5 { return }
```
 - [x] The guard is missing the else.
 - [ ] Nothing is wrong.
 - [ ] The guard is missing a then.
 - [ ] The comparison is wrong.

#### Q3. What is the raw/underlying type of this enum?
```
enum Direction {
  case north, south, east, west
}
```
 - [x] There is none.
 - [ ] String
 - [ ] Any
 - [ ] Int

#### Q4. Why is dispatchGroup used in certain situations?
 - [x] It allows multiple synchronous or asynchronous operations to run on different queues.
 - [ ] It allows track and control execution of multiple operations together.
 - [ ] It allows operations to wait for each other as desired.
 - [ ] all of these answers.

#### Q5. What is this code an example of?
```
let val = 5
print("value is: \(val)")
```
 - [x] string interpolation
 - [ ] string compilation
 - [ ] method chaining
 - [ ] string concatenation

#### Q6. What are the contents of vals after this code is executed?
```
var vals = [10, 2]
vals.sort { (s1, s2) -> Bool in
  s1 > s2
}
```
 - [x] [10, 2] 
 - [ ] [2, 10]
 - [ ] nil
 - [ ] This code contains an error

#### Q7. What does this code print?
```
typealias Thing = [String, Any]
var stuff: Thing
print(type(of: stuff))
```
 - [ ] Dictionary<String, Any> (To print this than code in question has to be `typealias Thing = [String: Any]`)
 - [ ] Dictionary
 - [x] ERROR (If code in question is really like that.)
 - [ ] Thing

#### Q8. What is the value of y?
```swift
let x = ["1", "2"].dropFirst()
let y = x[0]
```
 - [x] This code contains an error
 - [ ] 1
 - [ ] 2
 - [ ] nil

#### Q9. What is the value of test in this code?
```swift
var test = 1 == 1
```
 - [x] TRUE
 - [ ] YES
 - [ ] 1
 - [ ] This code contains an error

#### Q10. What is the value of y?
```swift
var x: Int?
let y = x ?? 5
```
 - [x] 5
 - [ ] 0
 - [ ] nil
 - [ ] This code contains an error

#### Q11. What is the type of this function?
```swift
func add(a: Int, b: Int) -> Int { return a+b }
```
 - [ ] Int
 - [x] (Int, Int) -> Int
 - [ ] Int<Optional>
 - [ ] Functions don't have types.

#### Q12. What is the correct was to call this function?
```swift
func myFunc(_ a: Int, b: Int) -> Int {
  return a + b
}
```
 - [x] myFunc(5, b: 6)
 - [ ] myFunc(5, 6)
 - [ ] myFunc(a: 5, b: 6)
 - [ ] myFunc(a, b)

#### Q13. The Codable protocol is \***\*\_\*\***?
 - [x] a combination of Encodable and Decodable
 - [ ] not a true protocol <<<<---Possibly correct as it's a typealias of Encodable and Decodable
 - [ ] required of all classes
 - [ ] automatically included in all classes

#### Q13. What is the type of value1 in this code?
```swift
let value1 = "\("test".count)"
```
 - [x] String
 - [ ] Int
 - [ ] null
 - [ ] test.count

#### Q14. When a function takes a closure as a parameter, when do you want to mark is as escaping?
 - [x] when it's executed after the function returns
 - [ ] when it's scope is undefined
 - [ ] when is's lazy loaded
 - [ ] all of these answers

#### Q15. What's wrong with this code?
```
class Person {
  var name: String
  var address: String
}
```
 - [x] Person has no initializers.
 - [ ] Person has no base class.
 - [ ] var name is not formatted corrrectly.
 - [ ] address is a keyword.

#### Q16. What is the value of names after this code is executed?
```
let names = ["Bear", "Joe", "Clark"]
names.map { (s) -> String in
  return s.uppercased()
}
```
 - [ ] ["BEAR", "JOE", "CLARK"]
 - [ ] ["B", "J", "C"]
 - [x] ["Bear", "Joe", "Clark"]
 - [ ] This code contains an error.

#### Q17. What describes this line of code?
```
let val = 5
```
 - [x] a constant named val of type Int
 - [ ] a variable named val of type item
 - [ ] a constant named val of type Number
 - [ ] a variable named val of type Int

#### Q18. What is the error in this code?
```
extension String {
  var firstLetter: Character = "c" {
    didSet {
      print("new value")
    }
  }
}
```
 - [x] Extensions can't add properties. // although extensions technically can't contain stored properties
 - [ ] Nothing is wrong with it.
 - [ ] didSet takes a parameter.
 - [ ] c is not a character.

#### Q19. didSet and willSet are examples of `\***\*\_\*\***`?
 - [x] property observers
 - [ ] key properties
 - [ ] all of these answers
 - [ ] newOld value calls

#### Q20. What is wrong with this code?
```
self.callback = {
  self.attempts += 1
  self.downloadFailed()
}
```
 - [x] Use of self inside the closure causes retain cycle.
 - [ ] You cannot assign a value to closure in this manner.
 - [ ] You need to define the type of closure explicitly.
 - [ ] There is nothing wrong with this code.

#### Q21. How many values does vals have after this code is executed?
```
var vals = Set<String> = ["4", "5", "6"]
vals.insert("5")
```
 - [x] three
 - [ ] four
 - [ ] eight
 - [ ] This code contains an error.

#### Q22. How can you avoid a strong reference cycle in a closure?
 - [x] Use a capture list to set class instances of weak or unowned.
 - [ ] You can't, there will always be a danger of strong reference cycles inside a closure.
 - [ ] Initialize the closure as read-only.
 - [ ] Declare the closure variable as lazy.

#### Q23. How can you avoid a strong reference cycle in a closure?
 - [x] an instance of any class
 - [ ] all of these answers
 - [ ] an instance of an optional type
 - [ ] an instance of function type

#### Q24. What is wrong with this code?
```
if let s = String.init("some string") {
  print(s)
}
```
 - [x] This String initializer does not return an optional.
 - [ ] String does not have an initializer that can take a String.
 - [ ] = is not a comparison.
 - [ ] Nothing is wrong with this code.

#### Q25. Which code snippet correctly creates a typealias closure?
 - [x] typealias CustomClosure: () -> ()
 - [ ] typealias CustomClosure { () -> () }
 - [ ] typealias CustomClosure -> () -> ()
 - [ ] typealias CustomClosure -> () {}

#### Q26. How do you reference class members from within a class?
 - [x] self
 - [ ] instance
 - [ ] class
 - [ ] this

#### Q27. All value types in Swift are \***\*\_\*\*** under the hood?
 - [x] structs
 - [ ] classes
 - [ ] optionals
 - [ ] generics

#### Q28. What is the correct was to ass a value to this array?
```
var strings = [1, 2, 3]
```
 - [x] all of these answers
 - [ ] strings.append(4)
 - [ ] strings.insert(5, at: 1)
 - [ ] strings += [5]

#### Q29. How many times will this loop be executed?
```
for i in 0...100 {
	print(i)
}
```
 - [ ] 0
 - [x] 101
 - [ ] 99
 - [ ] 100

#### Q30. What can AnyObject represent?
 - [x] an instance of any class
 - [ ] an instance of an optional type
 - [ ] an instance of a function type
 - [ ] all of these answers

#### Q31. What does this code print?
```
typealias Thing = [String:Any]
var stuff : Thing
print(type(of:stuff))
```
 - [ ] Dictionary
 - [ ] ERROR
 - [ ] Thing
 - [x] Dictionary<String, Any>

#### Q32. What is the value of test in this code?
```
var test = 1 == 1
```
 - [x] TRUE
 - [ ] 1
 - [ ] This code contains an error.
 - [ ] YES

#### Q33. What is the value of y?
```
var x : Int?
let y = x ?? 5
```
 - [ ] 0
 - [ ] nil
 - [ ] This code contains an error.
 - [x] 5

#### Q34. What is the value of y?
```
let x = ["1","2"].dropFirst()
let y = x[0]
```
 - [ ] 1
 - [ ] nil
 - [x] This code contains an error.
 - [ ] 2

#### Q35. What is the value of t after this code is executed?
```
let names = ["Larry","Sven","Bear"]
let t = names.enumerated().first().offset
```
 - [x] This code is invalid.
 - [ ] 0
 - [ ] 1
 - [ ] Larry

#### Q36. What is the value of test after this code executes?
```
let vt = (name: "ABC", val: 5)
let test = vt.0
```
 - [x] ABC
 - [ ] 0
 - [ ] 5
 - [ ] name

#### Q37. What is the base class in this code?
```
class LSN : MMM {
}
```
 - [x] MMM
 - [ ] LSN
 - [ ] There is no base class.
 - [ ] This code is invalid.

#### Q38. What does this code print to the console?
```
var userLocation: String = "Home" {
  willSet(newValue) {
  print("About to set userLocation to \(newValue)...")
  }

  didSet {
  if userLocation != oldValue {
  print("userLocation updated with new value!")
  } else {
  print("userLocation already set to that value...")
  }
  }
 }

 userLocation = "Work"
```
 - [ ] About to set userLocation to Work… userLocation updated to new value!
 - [ ] About to set userLocation to Work… userLocation already set to that value…
 - [ ] About to set userLocation to Home… userLocation updated to new value!
 - [ ] ERROR

#### Q39. What must a convenience initializer call?
 - [ ] a base class convenience initializer
 - [ ] either a designated or another convenience initializer
 - [x] a designated initializer
 - [ ] none of these answers

#### Q40. Which object allows you access to specify that a block of code runs in a background thread?
 - [ ] `DispatchQueue.visible`
 - [x] `DispatchQueue.global`
 - [ ] `errorExample` need to be labeled as `throws`.
 - [ ] `DispatchQueue.background`

#### Q41. What is the inferred type of x?
```
let x = ["a", "b", "c"]
```
 - [ ] `String[]`
 - [x] `Array<String>`
 - [ ] `Set<String>`
 - [ ] `Array<Character>`

#### Q42. What is the value of `oThings` after this code is executed?
```
let nThings: [Any] = [1, "2", "three"]
let oThings = nThings.reduce("") { "\($0)\($1)" }
```
 - [ ] `11212three`
 - [ ] `115`
 - [x] `12three`
 - [ ] Nothing, this code is invalid.

#### Q43. How would you call a function that throws errors and also returns a value?
 - [ ] `!try`
 - [x] `try?`
 - [ ] `try!`
 - [ ] `?try`

#### Q44. What is wrong with this code?
```
protocol TUI {
	func add(x1 : Int, x2 : Int) -> Int {
		return x1 + x2
	}
}
```
 - [ ] Protocol functions cannot have return types.
 - [x] Protocol functions cannot have implementations.
 - [ ] Nothing is wrong with it.
 - [ ] `add` is a reserved keyword.

#### Q45. In this code, what are `wheels` and `doors` examples of?
```
class Car {
	var wheels: Int = 4
	let doors = 4
}
```
 - [ ] class members
 - [ ] This code is invalid.
 - [ ] class fields
 - [x] class properties

#### Q46. What is the value of `t` after this code is executed?
```
let names = ["Larry", "Sven", "Bear"]
let t = names.enumerated().first().offset
```
 - [x] This code does not compile.
 - [ ] `0`
 - [ ] `1`
 - [ ] `Larry`

#### Q47. How do you designate a failable initializer?
 - [ ] `init?`
 - [ ] `deinit`
 - [x] `init`
 - [ ] You can't.

#### Q48. What is printed when this code is executed?
```
let dbl = Double.init("5a")
print(dbl ?? ".asString()")
```
 - [ ] `five`
 - [ ] `5a`
 - [x] `.asString()`
 - [ ] `5`
