
# FullCycle Docker Challenge with Go

The goal is to create a image that prints a simple message like "Hello, World!" in Golang.
The thing is that the image should have no more than 2 MB.




## How I Did It

First I look for the smallest Golang image possible. So, the base image I used was golang:alpine.
With that, I prepared the builder environment to use it at the second build stage where I start from scratch base image and executed the go file that what already compiled at the first stage.
After that, I just put the ENTRYPOINT to run the already compiled go script.

