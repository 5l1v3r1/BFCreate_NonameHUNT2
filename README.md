# BFCreate_NonameHUNT2
 Библиотека для моего софта  

пример:  
python bloom-create.py -th 5 -split 40000000 -infile btc.txt -prefix btc -rescan

python bloom-create.py <количество потоков обработки> <по сколько строк разбить большой файл> <входной файл с адресами> <префикс> <создавать файл для рескана или нет>  

-th Количество потоков определяет сколько ядер будет задействовано для конвертации адресов в HASH160  
-split программа может разбить большой файл на несколько блюм фильтров. оптимально 40-50 миллионов.  
    Например у вас есть сборный файл на 99 млн. используя параметр в размере 40 млн. программа создаст 3 файла блюма  
-infile это входной файл с адресами  
-prefix в программе закреплены следующие значения (btc, alt, eth) думаю вы все поняли уже сами ))  
-rescan Создавать файл рескана или нет , это ваш выбор! применимы следующие значения (yes, no)  
    файл создается с расширением rescan. Будте внимательны файл получается немного больше размером чем оригенальный файл с адресами  
    он нужен для точного опрееления нахождения.  
