all:  myProgram

myProgram: main.o employee.o address.o
	g++ -o myProgram main.o employee.o address.o

main.o: main.cpp
	g++ -c main.cpp

employee.o:
	g++ -c employee.cpp

address.o:
	g++ -c address.cpp

clear:
	rm -f main.o address.o employee.o myProgram
