CC = gcc
CFLAGS = -Wall -Wextra -std=c99
SRC = src/main.c
OBJ = $(SRC:.c=.o)
BIN = build/my_program

all: $(BIN)

$(BIN): $(OBJ)
	mkdir -p build
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -rf build
	rm -f $(OBJ)

.PHONY: all clean

#!/bin/bash

echo "Running the program..."
if [ ! -f build/my_program ]; then
    echo "Binary not found. Run 'make' to compile."
else
    ./build/my_program
fi

chmod +x script.sh

build/
*.o

# My Project: Bash, Make, Git, and GitHub

## Description
This is a simple project demonstrating the use of Bash scripts, Makefile automation, and version control with Git and GitHub.

## How to Run
1. Clone the repository:
   ```bash

 make

 ./script.sh


make clean



---


   ```bash
   git init
   git add .
   git commit -m "Initial commit"

git remote add origin https://github.com/your-username/my_project.git
git branch -M main
git push -u origin main


make
./script.sh
make clean

  

