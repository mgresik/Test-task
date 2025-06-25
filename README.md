# Test-task
Тестовая задача перед интервью

Сборка:

mkdir build && cd build

cmake -DCMAKE_TOOLCHAIN_FILE=../toolchain.cmake -DCMAKE_BUILD_TYPE=Debug ..    ## или TYPE=Release

make  ## -j(количество ядер)

./test-string
