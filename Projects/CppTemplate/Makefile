# compiler
CC = g++

# compile flags
CFLAGS = -wall -g

# libs
LIBS = inc/template.hpp

# source files
SRCS = src/template.cpp src/main.cpp

# object files
OBJS = $(SRCS:.cpp=.o)

# target
TARGET = solution

all: $(TARGET)

# Generates the target executable
$(TARGET):$(OBJS)
	$(CC) -o $(TARGET) $(OBJS) $(LIBS)

# Generates the output files
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Removes object files and target
clean: