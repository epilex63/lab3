# lab3

Task I
    В директории formatter_lib я создал такой CMakeLists.txt (1 скриншот)
    cmake_minimum_required устанавливает минимальную версию cmake
    project устанавливает имя сборки.
    set устанавливает минимальную версию g++ компилятора.
    add_library добавляет в сборку проекта блок файлов, которые будут использовааться в качестве библиотек для всех функций, упомянутых в этих файлах.
    Таким образом, статическая библиотека создана.

Task II
    В директории formatter_lib я сделал другой CMakeLists.txt (2 скриншот)
    С помощью target_include_directories включил директории formatter_lib для контакта с заголовочным файлом formatter.h
    С помощью target_link_libraries происходит линковка с библиотекой, в которой функции из заголовочного файла определены. 

Task III
    CMakeLists.txt для hello_world_application (3)
    При добавлении директории formatter_ex_lib также добавляется директория formatter_lib, так как в CMake файле formatter_ex_lib директории formatter_lib имеют модификатор PUBLIC.
    Создаю похожие CMake для solver_lib и solver_application (4 и 5)
    Так как файлы находятся в разных директориях, надо создать главный CMake который будет включать остальные. (6)
    В каждой директории с CMake исполняем команду cmake -H. -B_build, после чего в основном билде запускаем make
    Добавляем в solver.cpp <cmath> и меняем sqrtf на sqrt.
    Теперь можно запускать исполняемые файлы
