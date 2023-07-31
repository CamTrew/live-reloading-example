# Live Reloading Example

This repository provides an example of how to implement live reloading in a Go application using CompileDaemon.

## Overview

Live reloading is a development technique that automatically rebuilds and restarts the application whenever changes are made to the source code. It helps developers save time and get instant feedback on their code changes without the need for manual rebuilds and restarts.

In this example, we demonstrate how to use CompileDaemon, a tool for live reloading in Go applications. CompileDaemon monitors the source code for changes and triggers automatic rebuilds and restarts, allowing you to see the effects of your code changes in real-time.

## Prerequisites

To run this example, you need to have the following prerequisites installed:

- Go (version 1.16 or higher)
- Docker

## Getting Started

Follow these steps to run the example:

1. Clone this repository:

```
$ git clone https://github.com/thegodev/live-reloading-example.git
```
   
2. Change to the project directory:

```
$ cd live-reloading-example
```

3. Make sure you have Docker installed and run docker-compose:
   
```
$ docker-compose up
```   
   
This will start the container and mount the current directory inside the container. Any changes made to the code will trigger the live reloading.

5. Open a web browser and go to `http://localhost:8000/hello`. You should see the response below: 
```
{"message":"hello"}
```
6. Make changes to the source code (e.g., modify the message in `main.go`).

   As soon as you save the changes, CompileDaemon will detect the modifications and automatically rebuild and restart the application. The updated message will be reflected in the browser without manual intervention.

7. Repeat step 6 to see the live reloading in action. Enjoy coding with real-time feedback!