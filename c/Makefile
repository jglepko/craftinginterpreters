CC = gcc

CFLAGS = -g -Wall

SRCS = src/main.c src/chunk.c src/debug.c src/memory.c src/value.c src/vm.c src/compiler.c src/scanner.c src/object.c src/table.c 

OBJS = $(SRCS:.c=.o)

HDRS = src/chunk.h src/common.h src/debug.h src/memory.h src/value.h src/vm.h src/compiler.h src/scanner.h src/object.h src/table.h

TARGET = clox

all: $(TARGET)

$(TARGET): $(OBJS) $(HDRS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

$(OBJS): $(HDRS) $(SRCS)

clean:
	$(RM) -f $(TARGET) *.o *~
