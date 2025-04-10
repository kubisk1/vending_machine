cmake_minimum_required(VERSION 3.10)
project(vending_machine C)

# Włącz ostrzeżenia i ustaw standard C
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall")

# Dodaj katalog z nagłówkami
include_directories(inc)

# Zbierz wszystkie pliki .c z src/
file(GLOB SOURCES "src/*.c")

# Twórz plik wykonywalny
add_executable(vending_machine ${SOURCES})
