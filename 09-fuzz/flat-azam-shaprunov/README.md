# Bekhruz Azam Flat Buffers solution Node.js

_student_generated.js file should be in the same folder as solution.js_

    $ sha256sum data/students.bin
    0c016dc4ca1a8b24b34daa6c05472d16b401fd3c0c5417da18e9810b136704a6 data/students.bin
    $ node solution.js data/students.bin
    Reading binary student data from data/students.bin...
    3 students read...
    written to data/students.flat
    $ rm -f data/students.bin
    $ node solution.js data/students.flat
    Reading flatbuffers student data from data/students.flat...
    3 students read...
    written to data/students.bin
    $ sha256sum data/students.bin
    0c016dc4ca1a8b24b34daa6c05472d16b401fd3c0c5417da18e9810b136704a6 data/students.bin

# Shaprunov Fuzzing 

To check correctness run ```node fuzzer.js```, setupable TEST_COUNT variable.
Я гонял с корректными входными данными (по шаблону из https://github.com/decentralized-hse/practice/tree/main/04-formats) и все тесты были пройдены. 
Добавил только проверку на данные из .bin, что кол-во байт кратно 128. 

