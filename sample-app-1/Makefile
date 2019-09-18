EXTRA_CFLAGS+=-fstack-protector-strong -fPIE -fPIC -Wformat -Wformat-security
EXTRA_CFLAGS+=-O2 -D_FORTIFY_SOURCE=2
CFLAGS=-Wall $(EXTRA_CFLAGS)
LDFLAGS=-z noexecstack -z relro -z now -pie
PROGS=sample-app-1

all: $(PROGS)

sample-app-1: sample-app-1.o

clean:
	$(RM) *~ $(addsuffix .o,$(PROGS)) $(PROGS)
