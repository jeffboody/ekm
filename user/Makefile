TARGET   = ekm
CLASSES  =
SOURCE   = $(TARGET).c $(CLASSES:%=%.c)
OBJECTS  = $(TARGET).o $(CLASSES:%=%.o)
HFILES   = $(CLASSES:%=%.h)
OPT      = -O2 -Wall
CFLAGS   = $(OPT) -I.
LDFLAGS  =
CCC      = gcc

all: $(TARGET)

$(TARGET): $(OBJECTS)
	$(CCC) $(OPT) $(OBJECTS) -o $@ $(LDFLAGS)

clean:
	rm -f $(OBJECTS) *~ \#*\# $(TARGET)

$(OBJECTS): $(HFILES)
