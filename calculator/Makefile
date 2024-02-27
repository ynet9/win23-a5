
CC = gcc
CFLAGS = -std=c11 -Wall
TARGET = calculator 
SOURCE = $(wildcard *.c)
OUTPUT = $(SOURCE:.c=.o)

all: $(TARGET)

$(TARGET): $(OUTPUT)
	$(CC) $(CFLAGS) $^ -o $@


%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

operations.o: operations.h
	$(CC) $(CFLAGS) -c operations.h -o operations.o

clean:
	rm *.o $(TARGET)
