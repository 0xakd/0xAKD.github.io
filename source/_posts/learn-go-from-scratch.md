---
title: Learn Go from Scratch
tags:
  - golang
  - basics
categories:
  - software
date: 2024-07-03 22:03:35
---


![cover image](../images/learn-go-from-scratch/image.png)
## How to Download and install go in your device 
## Downloading Go
- Go to the official website of Go i.e. https://go.dev/
- Click download
- Select your Operating System and download the latest version

### Installing Go on Different Operating Systems
 - **Windows**
    - Open the MSI file you downloaded and follow the prompts to install Go. By default, the installer will install Go to Program Files or Program Files (x86). You can change the location as needed. After installing, you will need to close and reopen any open command prompts so that changes to the environment made by the installer are reflected at the command prompt.
    - Verify that you've installed Go.
    - In Windows, click the Start menu.
    - In the menu's search box, type cmd, then press the Enter key.
    - In the Command Prompt window that appears, type the following command:

```bash
$ go version
```
Confirm that the command prints the installed version of Go.


 - **Linux**
Remove any previous Go installation by deleting the /usr/local/go folder (if it exists), then extract the archive you just downloaded into /usr/local, creating a fresh Go tree in /usr/local/go:

```bash
$ rm -rf /usr/local/go && tar -C /usr/local -xzf go1.22.4.linux-amd64.tar.gz
```
- (You may need to run the command as root or through sudo). Do not untar the archive into an existing /usr/local/go tree. This is known to produce broken Go installations.

- Add /usr/local/go/bin to the PATH environment variable. You can do this by adding the following line to your $HOME/.profile or /etc/profile (for a system-wide installation):

```bash
$ export PATH=$PATH:/usr/local/go/bin
```
- Note: Changes made to a profile file may not apply until the next time you log into your computer. To apply the changes immediately, just run the shell commands directly or execute them from the profile using a command such as source $HOME/.profile.

- Verify that you've installed Go by opening a command prompt and typing the following command:

```bash
$ go version
```

Confirm that the command prints the installed version of Go.

**Mac**

- Open the package file you downloaded and follow the prompts to install Go.

- The package installs the Go distribution to /usr/local/go. The package should put the /usr/local/go/bin directory in your PATH environment variable. You may need to restart any open Terminal sessions for the change to take effect.

- Verify that you've installed Go by opening a command prompt and typing the following command:
```bash
$ go version
```
Confirm that the command prints the installed version of Go.


### Setting Up VS Code for Golang

**Download and install vs code in your device:**
- For Windows -> Microsoft Store
- For Linux -> Snap Store
- For Mac -> App Store
- Or else you can download it from its website: https://code.visualstudio.com/

**Installing Go extention for VS code**

- Go to Extensions section in vs code
- Search: "Go"
- install the 1st extension named "Go" by go.dev



## Getting Started with GO

**Creating Path for GO**:

- Make a new folder anywhere in your directory and name it "GO_LANG".
- Drag & Drop that folder in your VS code
- Create another new folder in that that folder and name it " helloworld ".
- Create a file under that "helloworld" folder and name it " main.go .

**How to run your Go code in vs code??**
- Right Click on the folder which you are using.
- Choose "Open integrated terminal"
- Go to the Terminal and Type: "go run <filename.go>" and press enter.

### Go Mod

The go mod command is a fundamental part of the Go Modules system. It is used to **create or initialize a Go module**, which is a way to manage dependencies and versioning in your Go projects.

Follow the steps to initialize go mod:

1. Right click on the folder your are in and open integrated terminal.

2. Type "go mod init <filename>" and hit enter.

***You have to mod every new folder you will make***

### Basic Structure of Go
```go
package main
import "fmt"

//the main function
func main(){
    //your code 
}
```

### Printing "Hello World" in Go.

```go 
package main

import "fmt"

func main() {
	fmt.Println("Hello World")
}
```

- The "fmt" package :- Stands for Format package. It offers a variety of functions to manipulate the format of input and output.

- The "fmt" package contains many functions under it. Some of the most commonly used functions of the "fmt" package are :-

    1. Sprintf - uses verbs like %s (string), %d(int), %f(float), %t(bool), etc. to interpolate values into a string and returns it as a single string.

    2. Printf - formats the input in the same way as Sprintf before printing it

    3. Println -simply prints the arguments it receives.


## Data types in Go.

There are mainly 4 data types :- string, integer, float, boolean. They are further divided into several categories:-

### Integers

- int = ranges from negative ∞ to positive ∞
- int8 = ranges from -128 to 127
- int16 = ranges from -32768 to 32767
- int32 = ranges from -2147483648 to 2147483647
- int64 = ranges -9223372036854775808 to 9223372036854775807
- uint8 = ranges from 0 to 255
- uint16 = ranges from 0 to 65535
- uint32 = ranges from 0 to 4294967295
- uint64 = ranges from 0 to 18446744073709551615

### Float
- float32 = all 32-bit floating point numbers.
- float64 = all 64-bit floating point numbers.

### Strings

- string = used for storing characters, letters, symbols, etc...

### Boolean

- bool = Stores either true or false value.


## Packages in Golang

**Package** - A package in Go is a collection of source files in the same directory that are compiled together. Packages are used to organize code and promote code reuse. Each Go program is made up of packages, and the program starts running in the main package.

### Key Points about packages in Golang. :-
1. **Package Declaration** :- Every Go source file starts with a package declaration. This defines the package to which the file belongs.

syntax:

```go
package package_name
```
2. **Importing Packages**:- To use functions, types, or variables from another packages, we need to import that package.

syntax:
```go
import "package_name"
```

## Variables
```go 
package main

import "fmt"

const Logintoken string = "zvbnm" //Public constant

func main() {

	//String values
	var variable1 string = "hello world"
	//Integer values
	var variable2 int = 530
	//Float values
	var variable3 float32 = 322.123144645776575675675756
	var variable4 float64 = 322.123144645776575675675756
	
    //default values and some alias
	var variable5 float64
	var variable6 string
	var variable7 int

	//no var delaration style
    variable8 := 1234 
    
    //Multiple variable declaration
    var variable9, variable10, variable11 string = "Shiv", "Shankar", "Bhole"
}
```

- "var" keyword is used to declare a variable.
- ":=" is used for direct declaration of a variable.
- Default Values don't store garbage values.<br>for eg. :- default string variables will return null value. default int/float variables will return 0.

### Printing Strings with variables
```go
package main
import "fmt"

func main() {
    var name string = "Ganesh"
    var age int = 18
    fmt.Println("She is",name ,"of age", age)
}
```

### To Print the Data Type of a Given Value
```go
package main
import "fmt"

func main() {
    abc = 324.5425
    fmt.Printf("this variable is of type: %T\n")
}
```

- "%T" is used for identifying the data type

### Arithmetic Operations

```go
package main 
func main() {
    sum := 5 + 4
    sub := 6 - 2
    mul := 3 * 2
    div := 10 / 2
    mod := 53 % 5
    greater := 4 > 3 // returns boolean value i.e. True or false.
    lesser := 5 < 7 // returns boolean value i.e. True or false.
    equalto := 6 == 7 // returns boolean value i.e. True or false.
    notequal := 5 != 4 // returns boolean value i.e. True or false.
    greaterequal := 8 >= 4 // returns boolean value i.e. True or false.
    lesserequal := 6 <= 9 // returns boolean value i.e. True or false.
}
```

## User Input
```go
package main

import (
    "bufio"
    "fmt"
    "os"
)
 func main() {
    reader = bufio.NewReader(os.Stdin) //Stdin stands for Standard input.
    fmt.Println("<Input statement for user>")
    
    input, _ := reader.ReadString("\n") // ", _" is called comma ok syntax. 
    fmt.Println("Your input is, ", input)
}
```

**Bufio or Buffered I/O package** :- allows input and output with a buffer.

**os package** :- It allows you to access to operating system functionalities.

**variable name.ReadString("\n")** :- it reads the user input data in string form until the user enters the value given inside the brackets i.e. "\n" (new line) .
