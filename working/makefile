# Note that compiling with VERBOSE will provide substantial debugging output,
#   and VERBOSE2 will give an enormous amount.
# Robert Grumbine 19 August 2003


#LINUX
CC=g++
CFLAGS=-Wall -DLINUX -O2 -DFLIP 
#-DVERBOSE -DVERBOSE2 
INCDIR=shorelines -Immablib/include

#Common -- accept from build script
#FAMILY=llgrid
#TARGET=global_ice
#RESOPS=2

# No changes below here -------------------------------------------
all : refill bathy paving

refill : refill.C geometry.C makefile
	$(CC) $(CFLAGS) $< -DFAMILY=$(FAMILY) -DTARGET=$(TARGET) -DRESOPS=$(RESOPS) -I$(INCDIR) -o $(@) mmablib/libombf_4.a

bathy : bathy.C
	$(CC) $(CFLAGS) $< -DTARGET=$(TARGET) -I$(INCDIR) -o $(@) mmablib/libombf_4.a

paving : paving.C geometry.C
	$(CC) $(CFLAGS) $< -DTARGET=$(TARGET) -I$(INCDIR) -DRESOPS=$(RESOPS) -o $(@) mmablib/libombf_4.a
