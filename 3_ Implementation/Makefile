# Name of the project
PROJECT_NAME = Clinic Management System
# All source code files
SRC = clinic_management_system.c\
src/clinic.c
INC = inc
all.exe : $(SRC) 
	gcc $^ -I$(INC) -o $@

run : all.exe
	./all.exe

clean:
	del all.exe



