rm -rf NAZWA_FOLDERU      #usuwa folder z całą zawartością
which NAZWA_POLECENIA     #pokazuje sciezke do pliku zrodlowego polecenia np. which bash

grep bash /etc/passwd     #pokazuje liste uzytkownikow korzystajacych z basha

if [ $1 == "string" ]     #porownuje stringi

$#                        #zwraca liczba parametrow
$@                        #zbior wszystkich parametrow np. echo $@ wyswietla wszystkie parametry

tab[int]=NUMBER/STRING    #ustawia zawartość komórki tablicy
tab[*]                    #zwraca wszystkie elementy tablicy

mkdir DIRNAME && cd $_    #tworzy katalog i wchodzi do niego

printf                    #dziala jak echo, ale nie dodaje znaku przeniesienia lini na koncu


grep -w WORD FILE         #wyszukuje tylko PEŁNE słowa WORD

echo `date`               #wyswietlanie aktualnej daty (zauważ odwrotne apostrofy)
echo `date +%s`           #wyswietla timestamp, przydatny np. do obliczenia czasu wykonywania skryptu


cat FILE_NAME             #wypisuje zawartość pliku na wyjście standardowe
cat file1 file2 > file12  #Łączy pliki file1 i file2 w jeden file12
-------------------------------------------------------------------------------------------------------

var=0                     #inicjalizacja licznika

for i in ${tablica[@]}    #iteruje po elementach tablicy              
  do
    echo ${#i}            #wyswietla ilość znaków w każdym elemencie tablicy
    var=$[$var+${#i}]     #zwiekszenie wartości licznika o dlugość elementu tablicy
  done


number=$[$RANDOM%1000]    #losowa liczba z zakresu 1-1000


-------------------------------------------------------------------------------------------------------



Operatory porównania:
http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-11.html

Zarządzanie argumentami:
http://wiki.bash-hackers.org/scripting/posparams

