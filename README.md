
# **Ruby**

#### [Learn Ruby The Hard Way](https://learnrubythehardway.org/book/)

## Variables
Variables are data elements that may or may not be changed
##### Assign
 - Assign is when you give a variable an initial value

##### Example:
```sh
cars = 1000
dogs = true
```

##### Use
- Use is when you put the assigned variables to work

##### Example:
```sh
puts "If there are #{cars} number of cars, then dogs are #{dogs}"
```

##### Types
- Types include integer (a whole number), double (a decimal number), boolean (determining if it is true or false), and string (include words, phrases, and sentences)

##### Example:
```sh
pencils = 6
puts pencils #would display 6

paper = 4.5
puts paper #would display 4.5

isVisible = true
puts isVisible #would display true
```

## Conditionals
Conditionals are actions that are performed based on user input. It could be a true-false statement or an if-then statement

##### Expressions
- Expressions are combinations of values, constants, variables, and operators to produce a result

##### Example:
```sh
x = 4
y = 6
y > x #Would return as true

x = 2
y = 3
z = 6
x + y >= z #Would return false
```

##### Branching
- Branching is when the program goes outside of the normal execution and executes a certain code based on certain conditions

##### Example:
```sh
x = 4
y = 8

if x < y
  puts "Yay"
else
  puts "Awee"
endif
```

## Methods
Methods are made up of data and behavior and another code can call it and use it

##### Returning
- Most of the end results are then returned to a test code to check if the method is valid

##### Example:
```sh
# This would be the method
def has_teen?(a, b, c)
	if a > 12 && a < 20
		return true
	end
	if b > 12 && b < 20
		return true
	end
	if c > 12 && c < 20
		return true
	end
	return false
end

# This would be the test
describe 'has_teen?' do
  it 'has a teen' do
    has_teen?(14, 12, 22).must_equal(true)
    has_teen?(16, 30, 9).must_equal(true)
  end
  it 'does not have a teen' do
    has_teen?(20, 11, 6).must_equal(false)
  end
end

describe 'not_string' do
  it 'does not start with not' do
    not_string("hello").must_equal("nothello")
  end
  it 'does start with not' do
    not_string("nothi").must_equal("nothi")
  end
end
```
