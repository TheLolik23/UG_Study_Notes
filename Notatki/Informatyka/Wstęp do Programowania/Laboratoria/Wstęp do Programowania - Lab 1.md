---
date: 2025-10-13
tags:
  - JęzykC
moc: "[[Wstęp do Programowania - Laboratoria]]"
type: Class Note
---

# Laboratoria 13-10-2025

## Temat: Hello World - C

---

1. Uruchom pierwszy program zgodnie z opisem 01_first.pdf.

    ```C title:zad0.c
    #include <stdio.h>
    
    int main(){
        printf("Hello World!\n");
        
        return 0;
    }
    ```

2. Napisz program, który wyświetla Twoją wizytówkę (użyj różnych specyfikatorów w łańcuchu konfiguracyjnym printf - \n, \t, itp).

    ```C title:zad2.c
    #include <stdio.h>
    
    int main(){
        printf("Stanisław Świderski \t - \t Technik Programista \nNauczyciel w: \n\tZespół szkół łączności w Gdańsku");
        
        return 0;
    }
    ```

3. Na początku programu zadeklaruj zamienne w następujący sposób:

    ```C
    char *name1 = "Adrian";  
    int age1 = 20;  
    double height1 = 1.83;  
    char *name2 = "Ania";  
    int age2 = 9;  
    double height2 = 1.4;  
    ```
    
    Napisz program, który korzystając z tych zmiennych będzie wyświetlał tabelę:
    
    ```text
    |Adrian              |                  20|      1.83|
    |Ania                |                   9|      1.40|
    ```
    
    Pierwsza i druga kolumna powinna mieć szerokość 20 znaków. Trzecia kolumna powinna mieć szerokość 10 znaków i wyświetlać liczbę z dokładnością do dwóch miejsc po przecinku.
    
    ```C title:zad3.c
    #include <stdio.h>
    
    int main(){
        char *name1 = "Adrian";  
        int age1 = 20;  
        double height1 = 1.83;  
        char *name2 = "Ania";  
        int age2 = 9;  
        double height2 = 1.4;
        int main(void){
        printf("|%-20s|%20d|%10.2f|\n", name1, age1, height1);
        printf("|%-20s|%20d|%10.2f|", name2, age2, height2);
    }
    ```

4. Napisz program, który wczyta trzy liczby naturalne a następnie wyświetli je w odwrotnej kolejności.

    ```C title:zad4.c
    # include <stdio.h>
    
    int main(void){
        int l1;
        int l2;
        int l3;
        scanf("%d", &l1);
        scanf("%d", &l2);
        scanf("%d", &l3);
        printf("%5d %5d %5d",l3,l2,l1);
    }
    ```
