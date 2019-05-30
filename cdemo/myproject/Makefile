TARGET = student.c
LIBS = -lm
CC = gcc
CFLAGS = -g Wall =I.typedef 

.PHONY: clean all default

default: $(TARGET)
all: default

HEARDS = $(wildcard*.h)
OBJECTS = $(patsubst %.c, %.o, $(wildcard *.c))

%.o: %.c $(HEADERS)
        $(CC) $(CFLAGS) -c $< -o $@

$(TARGET): $(OBJECTS)
        $(CC) $^ $(LIBS) -o $@

clean:
      -rm -f *.o
      -rm -f $(TARGET)
