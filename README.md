# Simple Chat Bot (Go)

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Hyperskill](https://img.shields.io/badge/Hyperskill-JetBrains_Academy-purple?style=flat-square)
![Status](https://img.shields.io/badge/Status-Learning_Project-blue?style=flat-square)

A simple interactive command-line chatbot written in **Go**, developed as part of the [Hyperskill — Simple Chat Bot (Go)](https://hyperskill.org/projects/206) project by JetBrains Academy.

## Overview

This project is a beginner-friendly console application designed to practice the fundamentals of Go programming.

The chatbot communicates with users through the terminal, asks questions, performs a mathematical trick to guess their age, counts numbers, and runs a small programming quiz.

The project focuses on understanding how to structure a program, process user input, and implement basic application logic.

## Features

The project is divided into five stages:

| Stage | Description |
|---|---|
| 1. Introduction | The chatbot introduces itself |
| 2. User Interaction | Asks for the user's name and responds |
| 3. Age Guessing | Calculates the user's age using mathematical remainders |
| 4. Counting | Counts from zero to a user-specified number |
| 5. Quiz | Asks a multiple-choice question and checks the answer |

## Technologies

- **Go (Golang)** — Programming language
- **Go Standard Library** — Console input and output
- **Git** — Version control
- **GitHub** — Source code hosting

## Getting Started

### Prerequisites

Install [Go](https://go.dev/dl/) and verify your installation:

```bash
go version
```

### Installation

Clone the repository:

```bash
git clone https://github.com/lowqrst/simple-chat-bot-go.git
```

Navigate to the project directory:

```bash
cd simple-chat-bot-go
```

### Run

If the project contains a `main.go` file:

```bash
go run main.go
```

Or, if the project is configured as a Go module:

```bash
go run .
```

## Example Interaction

```text
Hello! My name is Aid.
I was created in 2023.
Please, remind me of your name.
> Alex

What a great name you have, Alex!
Let me guess your age.
Enter remainders of dividing your age by 3, 5 and 7.
> 1 4 5

Your age is 19; that's a good time to start programming!

Now I will prove to you that I can count to any number you want.
> 5

0!
1!
2!
3!
4!
5!

Let's test your programming knowledge.
Why do we use methods?

1. To repeat a statement multiple times.
2. To decompose a program into several small subroutines.
3. To determine the execution time of a program.
4. To interrupt the execution of a program.

> 2
Completed, have a nice day!
```

## How Age Guessing Works

The chatbot uses a mathematical technique based on the **Chinese Remainder Theorem**.

The user enters the remainders obtained when dividing their age by 3, 5, and 7.

The program calculates:

```go
age := (remainder3*70 + remainder5*21 + remainder7*15) % 105
```

This formula reconstructs the age modulo 105.

For ages between 0 and 104, the result uniquely determines the user's age.

## Learning Outcomes

Through this project, I practiced:

- Variables, constants, and data types
- Console input and output using `fmt`
- Conditional statements (`if`, `else`)
- Loops (`for`)
- Functions and code organization
- Arithmetic operations
- Basic user input processing
- Building interactive CLI applications

## Project Structure

A minimal implementation can use the following structure:

```text
simple-chat-bot-go/
├── main.go
├── go.mod
└── README.md
```

The actual structure may vary depending on the implementation.

## Future Improvements

Potential extensions include:

- Additional quiz questions
- Randomized questions
- Input validation
- Score tracking
- Improved command-line interaction
- Unit tests

## Acknowledgments

This project is based on the **Simple Chat Bot (Go)** educational project developed by JetBrains Academy and available on Hyperskill.

Project link: https://hyperskill.org/projects/206

## Author

**Nursultan Tleukhanov**

Cybersecurity Student at Astana IT University

Aspiring Go Backend Developer

GitHub: [@lowqrst](https://github.com/lowqrst)
