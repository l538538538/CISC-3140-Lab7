# The makefile will display HelloWorld message with current time

all: hello

hello : file1.o M1.o file2.o

# This line will execute HelloWorld.java
file1.o:
        java HelloWorld

# This line will echo a message that the ShowDate.java is execute next
M1.o:
        echo "Now display current date"

# This line will execute ShowDate.java
file2.o:
        java ShowDate
