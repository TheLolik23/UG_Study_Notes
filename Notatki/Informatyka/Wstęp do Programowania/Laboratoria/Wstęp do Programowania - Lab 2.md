---
Date-Added: 2025-10-20T10:06:00
Category:
  - IT
MOC: "[[Wstęp do Programowania - Laboratoria]]"
type: basic-note
---
## Temat: Instrukcje Warunkowe, Operatory
- - -
1. Napisz program, który wczyta dwie liczby naturalne a i b oraz wyświetli informację o ich iloczynie, sumie oraz różnicy.
 ```C title:zad1.c
 #include <stdio.h>  
  
int main(void) {  
    int a,b;  
    printf("Podaj liczby a i b: ");  
    scanf("%d%d",&a,&b);  
    printf("Suma: %d \n",a+b);  
    printf("Różnica(a-b): %d \n",a-b);  
    printf("Iloczyn: %d \n",a*b);  
    return 0;  
}
```
2. Napisz program, który poprosi użytkownika o podanie dodatniej liczby zmiennoprzecinkowej a i wyświetli informację o kwadracie, sześcianie i pierwiastku z liczby a.
```C title:zad2.c
#include <math.h>  
#include <stdio.h>  
  
int main(void) {  
    float a;  
    printf("Podaj liczby a: ");  
    scanf("%f",&a);  
    if(a<0) {  
        printf("Liczba musi byc dodatnia\n");  
    }else {  
        printf("Kwadrat a: %f \n", a*a);  
        printf("Szescian a: %f \n", a*a*a);  
        printf("Pierwiastek a: %f \n", sqrt(a));  
    }  
    return 0;  
}
```
3.  Napisz program, który poprosi użytkownika o podanie wieku oraz wyświetli jedną z informacji jesteś pełnoletni lub będziesz pełnoletni za x lat, gdzie x jest wartością wyliczoną na podstawie wieku.
```C title:zad3.c
#include <stdio.h>  
  
int main(void) {  
    int a;  
    printf("Podaj wiek: ");  
    scanf("%d",&a);  
    if(a>=18) {  
        printf("Jesteś pelnoletni\n");  
    }else {  
        printf("Bedziesz pelnoletni za %d lat. \n",18-a );  
    }  
    return 0;  
}
```
4. Napisz program, który wczyta dwie liczby naturalne a i b oraz wyświetli informację o ich ilorazie albo informację, że nie można go obliczyć.
```C title:zad4.c
#include <stdio.h>  
  
int main(void) {  
    int a,b;  
    float iloraz;  
    printf("Podaj liczby a i b iloraz(a/b): ");  
    scanf("%d%d",&a,&b);  
    if(b==0) {  
        printf("Blad: Nie mozna obliczyc ilorazu (DZIELENIE PRZEZ ZERO)\n");  
    }else {  
        iloraz = (float)a /b;  
        printf("Iloraz a/b: %.4f  \n", iloraz);  
    }  
    return 0;  
}
```
4. Napisz program, który wczyta od użytkownika 3 liczby typu double a następnie wyświetli je w kolejności niemalejącej.
```C title:zad5.c
#include <stdio.h>  
int main(void) {  
    double a,b,c;  
    printf("Podaj liczby a, b, c: ");  
    scanf("%lf%lf%lf",&a,&b,&c);  
  
    //c najmniejsze  
    if (c<=a && c<=b) {  
        if (b<a) {  
            //cba  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", c,b,a);  
            return 0;  
  
        }else {  
            //cab  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", c,a,b);  
            return 0;  
  
        }  
    }  
    //b najmniejsze  
    if (b<=a && b<=c) {  
        if (a<c) {  
            //bac  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", b,a,c);  
            return 0;  
        }else {  
            //bca  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", b,c,a);  
            return 0;  
        }  
    }  
    //a najmniejsze  
    if (a<=b && a<=c) {  
        if (b<c) {  
        //abc  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", a,b,c);  
            return 0;  
        }else {  
        //acb  
            printf("Liczby w kolejnosci niemalejacej: %lf %lf %lf \n", a,c,b);  
            return 0;  
    }  
    }  
  
}
```
4.  Napisz program, który wczyta od użytkownika liczbę naturalną 0<=a<=9999 i wypisze jej cyfry w odwrotnej kolejności.
```C title:zad6.c
#include <stdio.h>  
int main(void) {  
   int a;  
    int b =0;  
    printf("Podaj liczbe a z przedzialu 0<=a<=9999: ");  
    scanf("%d",&a);  
    if(a>=0 && a<=9999) {  
        while (a != 0) {  
            int last = a % 10;  
            b = b * 10 + last;  
            a /= 10;  
        }  
        printf("%d\n",b);  
        return 0;  
    } else {  
        printf("Liczba %d jest z poza przedzialu!",a);  
        return 0;  
    }  
}
```
4. Napisz program, który poprosi o podanie miesiąca (liczba naturalna) oraz wyświetli jego nazwę słownie.
```C title:zad7.c
#include <stdio.h>  
int main(void) {  
    int miesiac;  
    printf("Podaj numer miesiaca: ");  
    scanf("%d", &miesiac);  
    if (miesiac>=1 && miesiac<=12) {  
        switch (miesiac) {  
            case 1:  
                printf("Styczen\n");  
                break;  
            case 2:  
                printf("Luty\n");  
                break;  
            case 3:  
                printf("Marzec\n");  
                break;  
            case 4:  
                printf("Kwiecien\n");  
                break;  
            case 5:  
                printf("Maj\n");  
                break;  
            case 6:  
                printf("Czerwiec\n");  
                break;  
            case 7:  
                printf("Lipiec\n");  
                break;  
            case 8:  
                printf("Sierpien\n");  
                break;  
            case 9:  
                printf("Wrzesien\n");  
                break;  
            case 10:  
                printf("Pazdziernik\n");  
                break;  
            case 11:  
                printf("Listopad\n");  
                break;  
            case 12:  
                printf("Grudzien\n");  
                break;  
        }  
    } else {  
        printf("Nie isteniej miesiac o podanej liczbie!\n");  
    }  
    return 0;  
}
```
4. Napisz program, który poprosi użytkownika o podanie dwóch parametrów a i b oraz obliczy miejsce/a zerowe funkcji f(x) = ax + b.
```C title:zad8.c
#include <stdio.h>  
int main(void) {  
float a,b;  
    printf("Podaj parametry a i b funkcji (f(x)=ax+b): ");  
    scanf("%f %f",&a,&b);  
    float x=-b /a;  
    printf("Miejsce zerowe funkcji o podanych parametrach %.2f\n",x);  
    return 0;  
}
```
4. Napisz program, który poprosi użytkownika o podanie trzech parametrów a, b i c oraz obliczy miejsce/a zerowe funkcji f(x) = ax^2 + bx + c.
```C title:zad9.c
#include <math.h>  
#include <stdio.h>  
int main(void) {  
    float a,b,c;  
    printf("Podaj parametry a i b funkcji (f(x)=ax^2+ bx +c): ");  
    scanf("%f %f %f",&a,&b,&c);  
    float delta = b*b - 4*a*c;  
    float x1,x2;  
  
    if(delta > 0){  
    x1 = (-b + sqrt(delta))/(2*a);  
    x2 = (-b - sqrt(delta))/(2*a);  
        printf("Miejsce zerowe funkcji o podanych parametrach %.2f %.2f\n",x1,x2);  
    } else {  
        printf("Delta jest ujemna. Brak miejsc zerowych w zbiorze liczb naturalnych");  
    }  
  
    return 0;  
}
```
4. Napisz program, który poprosi użytkownika o wpisanie jednego znaku i wypisze informację czy jest to litera alfabetu łacińskiego.
```C title:zad10.c
#include <stdio.h>  
int main(void) {  
    char c;  
    printf("Znak: ");  
    scanf("%c", &c);  
    if ( (c >= 'A' && c <= 'Z') || (c >= 'a' && c <= 'z') ){  
    printf("Podany znak znajduje sie w alfabecie lacinskim");  
    }  
    else {  
        printf("Podany znak nie znajduje sie w alfabecie lacinskim");  
    }  
    return 0;  
}
```
4. Napisz program, który poprosi użytkownika o podanie temperatury wyrażonej w stopniach Celsjusza i wyświetli informację o jej wartości wyrażonej w stopniach Fahrenheita.
```C title:zad11.c
  
#include <stdio.h>  
int main(void) {  
    float temperatura;  
    printf("Podaj temperaturę(w stopniach celcjusza): ");  
    scanf("%f", &temperatura);  
    printf("temperatura w stopniach Fahrenheita %.2f", (temperatura-30)/2); 
    return 0;  
}
```
4. Napisz program, który poprosi użytkownika o podanie temperatury wyrażonej w stopniach Fahrenheita i wyświetli informację o jej wartości wyrażonej w stopniach Celsjusza.
```C title:zad12.c
#include <stdio.h>  
int main(void) {  
    float temperatura;  
    printf("Podaj temperaturę(w stopniach Fahrenheita): ");  
    scanf("%f", &temperatura);  
    printf("temperatura w stopniach celcjusza %.2f", temperatura*2 + 30);  
  
    return 0;  
}
```
4. Napisz program, który dla podanego punktu (współrzędne x oraz y) sprawdzi czy znajduje się on w kwadracie (-10,-10)...(10,10).
```C title:zad13.c
  
#include <stdio.h>  
int main(void) {  
    float x,y;  
    printf("Podaj wspolrzedne x i y: ");  
    scanf("%f%f", &x,&y);  
    if (x<=10&&x>=-10&&y<=10&&y>=-10) {  
        printf("Punklt o wspolrzednych x: %f y:%f znajduje sie w kwadracie (-10,-10)...(10,10)",x,y);  
    } else {  
        printf("Punklt o wspolrzednych x: %f y:%f  nie znajduje sie w kwadracie (-10,-10)...(10,10)",x,y);  
    }  
  
    return 0;  
}
```
4. Napisz program, który wczyta od użytkownika znak i wyświetli jeden z komunikatów:

-  wczytany znak jest małą literą,
    
-  wczytany znak nie jest literą ani cyfrą.
    
-  wczytany znak jest cyfrą,
    
-  wczytany znak jest wielką literą,
    
```C title:zad14.c
#include <stdio.h>  
int main(void) {  
    char c;  
    printf("Znak: ");  
    scanf("%c", &c);  
    if ( c >= 'A' && c <= 'Z'  ){  
        printf("Podany znak jest duza litera");  
    }  
    else {  
        if ( c >= 'a' && c <= 'z'  ){  
            printf("Podany znak jest mala litera");  
        } else {  
            if (c >= '0' && c <= '9') {  
                printf("Podany znak jest cyfra");  
            } else {  
                printf("Podany znak nie jest litera ani cyfra");  
            }  
        }  
    }  
    return 0;  
}
```
15. Napisz program, który poprosi o podanie roku i wypisze informacje, czy ten rok jest przestępny?
```C title:zad15.c
#include <stdio.h>  
int main(void) {  
int rok;  
    printf("Podaj rok: ");  
    scanf("%d", &rok);  
//rok przestepny podzielny 4 lub jest podzielny przez 100 i 400  
    if (rok%4 ==0 && rok%100 !=0||rok%400==0 ) {  
        printf("It is a leap year.\n");  
    } else {  
        printf("It is not a leap year.\n");  
    }  
    return 0;  
}
```
15. Napisz program, który dla podanej przez użytkownika liczby całkowitej wyświetli informację czy jest to cyfra, a jeżeli jest to dodatkowo wyświetli jej wartość słownie.
```C title:zad16.c
#include <stdio.h>  
int main(void) {  
int a;  
    printf("Podaj cyfre dodatnia a: ");  
    scanf("%d", &a);  
        switch (a) {  
            case 0:  
                printf("Zero\n");  
                break;  
                case 1:  
                printf("Jeden\n");  
                break;  
                case 2:  
                printf("Dwa\n");  
                break;  
                case 3:  
                printf("Trzy\n");  
                break;  
                case 4:  
                printf("Cztery\n");  
                break;  
                case 5:  
                printf("Piec\n");  
                break;  
                case 6:  
                printf("Szesc\n");  
                break;  
                case 7:  
                printf("Siedem\n");  
                break;  
                case 8:  
                printf("Osiem\n");  
                break;  
                case 9:  
                printf("Dziewiec\n");  
                break;  
    default: printf("Nie jest to cyfra\n");  
  
  
  
        }  
    return 0;  
}
```
15. Napisz program, który dla podanego przez użytkownika znaku wyświetli:
 - jeżeli wprowadzony znak jest literą, to wyświetli znak znajdujący się na klawiaturze po prawej stronie od danego lub
- informację, że podany znak nie jest literą
```C title:zad17.c
#include <stdio.h>  
  
int main() {  
    char znak;  
    printf("Podaj znak (mala litera lub znak specjalny): ");  
    scanf("%c", &znak);  
if (znak>='A' && znak<='Z') {  
    printf("Podana litera musi byc mała");  
}else {  
    switch(znak) {  
        case 'a': printf("s\n"); break;  
        case 'b': printf("n\n"); break;  
        case 'c': printf("v\n"); break;  
        case 'd': printf("f\n"); break;  
        case 'e': printf("r\n"); break;  
        case 'f': printf("g\n"); break;  
        case 'g': printf("h\n"); break;  
        case 'h': printf("j\n"); break;  
        case 'i': printf("o\n"); break;  
        case 'j': printf("k\n"); break;  
        case 'k': printf("l\n"); break;  
        case 'l': printf(";\n"); break;  
        case 'm': printf(",\n"); break;  
        case 'n': printf("m\n"); break;  
        case 'o': printf("p\n"); break;  
        case 'p': printf("[\n"); break;  
        case 'q': printf("w\n"); break;  
        case 'r': printf("t\n"); break;  
        case 's': printf("d\n"); break;  
        case 't': printf("y\n"); break;  
        case 'u': printf("i\n"); break;  
        case 'v': printf("b\n"); break;  
        case 'w': printf("e\n"); break;  
        case 'x': printf("c\n"); break;  
        case 'y': printf("u\n"); break;  
        case 'z': printf("x\n"); break;  
        default: printf("Podany znak nie jest litera\n");  
    }  
}  
  
    return 0;  
}
```




