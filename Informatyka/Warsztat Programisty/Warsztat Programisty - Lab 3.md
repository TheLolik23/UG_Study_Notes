---
Date-Added: 2025-10-21T12:24:00
Category:
  - IT
MOC: "[[Warsztat Programisty - Laboratoria]]"
type: basic-note
---
## Temat:
- - -
Pierwszy skrypt:
```bash
touch plik1.txt
mv plik1.txt ./Laboratorium1
ls -l #-rw-------+ 1 sswiderski domain users 0 Oct 21 12:24 plik1.txt

touch plik2.txt
chmod o+r plik2.txt

nano pierwszy.sh
chmod u+x pierwszy.sh
./pierwszy.sh
#TempDir  cwiczenia  nowyPlik.txt  pierwszy.sh  plik1.txt  plik2.txt  wyklad  zadania

nano drugi.sh
chmod u+x drugi.sh #gives permission to user -> u to execute ->x file. u+x
```

```bash title:pierwszsy.sh
mkdir TempDir
ls -a
```

```bash title:drugi.sh
!/ bin / bash 
mkdir TempDir 
ls -a
```
Zmienne środowiskowe:
```bash
echo $SHELL #bin/bash
```
Przykładowe zmienne środowiskowe:
- SHELL - używana powłoka
- PATH – lista lokalizacji, w których powłoka poszukuje programów do uruchomienia  
- USER – nazwa użytkownika 
- HOME – katalog domowy użytkownika
- EDITOR – domyślny edytor tekstu 
- LD LIBRARY PATH – lista lokalizacji w których system poszukuje bibliotek
```bash
ls
echo $? #output: 0 - komenda wykonana bezbłędnie
rm jakisnieistniejacyplik.cos
echo $? #Output: 1 - błąd podczas wykonywania
```

>Dzięki zmiennej środowiskowej PATH możemy łatwo sprawić, że nasz skrypt będzie można uruchamiać, wpisując jedynie jego nazwę, bez podawania pełnej ścieżki. Wykonaj polecenie PATH="$PATH:sciezkabezwzglednadoskryptu" oraz uruchom skrypt przez podanie wyłącznie jego nazwy. UWAGA: Po zamknięciu terminala zmiana zmiennej PATH jest tracona i przywracany jest jej pierwotny stan.

```C title:program.c
int main () { 
return 7; 
}
```

```bash
nano program.c

gcc program.c 

./a.out 

echo $? #output: 7

```

```bash
nano program.c #changes: return -1;

gcc program.c 

./a.out 

echo $? #output: 255

```

```bash
nano program.c #changes: return 257;

gcc program.c 

./a.out 

echo $? #output: 1

```

```bash
echo $USER #o: sswiderski
echo $HOME #o:home/sswiderski
echo $EDITOR
```
Zadanie z tablicy:
```c title:hello.c
#include <stdio.h>
int main(void){



printf("Hello World\n");

return 0;

}
```

```bash title:skrypt.sh
gcc hello.c -o hello

./hello

echo $?

chmod 707 hello #

ls -l
```

### Permissions

The following permissions grant the corresponding operations on files and directories:

#### Read (r)

- For files: grants the ability to read the file’s contents (not its name or metadata, which are determined by the permissions of its parent directory).
- For directories: grants the ability to read the directory entry names of its contained files and directories, but not to access their metadata ([inode](https://en.wikipedia.org/wiki/Inode "Inode")) and therefore their content, which is determined by the directory _execute_ permission.

#### Write (w)

- For files: grants the ability to modify the file contents.
- For directories: grants the ability to modify entries in the directory, which allows creating, deleting, and renaming its files or directories.
    - Doing so also requires the _execute_ permission in order to access the metadata ([inode](https://en.wikipedia.org/wiki/Inode "Inode")) of all its containing files and directories. Therefore, without _execute_ permission the _write_ permission is effectively meaningless.

#### Execute (x)

- For files: grants the ability to execute a file. This permission must be set for executable programs to allow running them.
    - Doing so also requires the _read_ permission.
- For directories: grants the ability to read the metadata of its containing files and directories if their names are known, but not to read their names. A directory without _execute_ permission effectively blocks reading and writing the content of its contained files and directories.
    - A directory with _execute_ permission but without _read_ permission effectively makes it a name guessing game to access the contents of its files and directories.
##### Reddit chmod Tip:
>No you will need to run the command using the change permission program `chmod` like so:

```
chmod 755 filename
```

###### Explained:

- change the permission to:
```
    - user: 7 => r(4), w(2), x(1)
    - group: 5 => r(4), -, x(1)
    - others: r(4), -, x(1)
```