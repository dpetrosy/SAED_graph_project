.PHONY: all re clean fclean debug gcov lcov clean_gcda clean_gcno clean_gcov clean_lcov fclean_glcov

FOLDER=src
SOURCES=$(wildcard $(FOLDER)/*.cpp)
OBJECTS=$(SOURCES:.cpp=.o)
CC=g++
INCS = -Iinclude
CXXFLAGS=-Wall -Wextra -Werror $(INCS)
CPPFLAGS=
STANDARD=-std=c++17
EXECUTABLE=graph.exe
RM=rm -rf
LCOVTEST=$(EXECUTABLE:.exe=.info)
BROWSER=google-chrome

all : $(EXECUTABLE)

$(EXECUTABLE) : $(OBJECTS)
	$(CC) $(OBJECTS) -o $@

%.o : %.cpp
	$(CC) $(STANDARD) $(CPPFLAGS) $(CXXFLAGS) -c -g $< -o $@

re : fclean all

clean :
	$(RM) $(OBJECTS)

fclean : clean
	$(RM) $(EXECUTABLE)

debug :
	gdb $(EXECUTABLE)

gcov :
	$(CC) $(STANDARD) $(CPPFLAGS) $(CXXFLAGS) $(SOURCES) --coverage -o $(EXECUTABLE)
	./$(EXECUTABLE)

lcov :
	lcov -t "program" -o $(LCOVTEST) -c -d .
	genhtml -o report $(LCOVTEST)
	$(BROWSER) report/index.html

clean_gcda :
	$(RM) *.gcda

clean_gcno :
	$(RM) *.gcno

clean_gcov : clean_gcda clean_gcno
	$(RM) $(LCOVTEST)
	$(RM) $(EXECUTABLE)

clean_lcov : 
	$(RM) report

fclean_glcov : clean_gcov clean_lcov
