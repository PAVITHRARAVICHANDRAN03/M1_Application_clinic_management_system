# Name of the project
PROJECT_NAME = Clinic Management System

# Output directory
BUILD = build

# All source code files
SRC = project_main.c\
src/clinic main.c
OBJ = clinic main.o
INC = inc
CFLAGS = I$(INC)
a.out:$(OBJ)
   gcc $ -I$(INC)-o $@
%.o:src%
   gcc $^ -I$(INC)-c
run : target
   ./all.out
clear:
   rm all.out *.o src/*.o
   
#Target_name

PROJ_NAME =	Bank
SRC	= clinic_main.c Clinic_Management_System.c

ifdef OS
	RM=del /q
   	FixPath=$(subst /,\,$1)
	EXEC =exe
else
	ifeq ($(shell uname),Linux)
		RM= rm -rf
		FixPath= $1
		EXEC =out
	endif
endif




build:
	gcc $(SRC) -o $(call FixPath,$(PROJ_NAME).$(EXEC))

run: build
	./$(call FixPath,$(PROJ_NAME).$(EXEC))

clean:
	$(RM) $(call FixPath,$(PROJ_NAME).$(EXEC))
