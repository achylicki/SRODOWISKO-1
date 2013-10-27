#ROZWIAZANIA

ZADANIE 1 - odwracanie tablicy, elementy i ilosc znane

```c

int main() {
int i
int tabela[]={1,2,4,6,12};
for(i=4,i>=0,i=i+1) printf(" %i ", tabela[i]);
return 0;
}
```

ZADANIE 2 - potegi mniejsze od 2010, petla while oraz for

```c
#include<stdio.h>
main() {

  int i;
  int potega=1;
  int granica=2010;

  for(i=1;potega<granica;i=i+1){
    printf("Potega %d stopnia = %d \n",i-1,potega);
    potega=potega*2;
  }



  potega=1;
  i=1;
  for(potega=1;potega<granica;potega=potega*2){
    printf(" %i ",potega);
  } 

  potega=1;
  while(potega<granica){
    printf(" %i ", potega);
    potega=potega*2;
    i=i+1;}


  potega=1;
  i=1;
  while(potega<granica){
    printf("Potega %d stopnia = %d \n",i-1,potega);
    potega=potega*2;
    i=i+1;
  }


}
```
ZADANIE 3 - rowzne obliczanie oraz n-ta potega dwojki

```c
main(){
  int n=66;
  int i=0;
  int iloczyn=0;
  int n1, n2,n3;
  n1=5+3*8/2-3;
  n2=2%2+2*2-2/2;
  n3=2*4*(5+9/2);
  printf("N1: %d  N2: %d  N3:  %d \n",n1,n2,n3);
  printf("Podaj N: ");
  scanf("%d",&n);
  if(n>0)  for(i=1;i<=n;i=i+1){
    iloczyn=iloczyn+i*i;
  }
  else printf("LICZBA MUSI BYC WIEKSZA od 0");
  printf("Suma iloczynow: %d ",iloczyn);
}
```
ZADANIE 4- prosi o podanie elementow tablicy (max 50). Jezeli bedzie zero, wtedy konczymy i pokazujemy w odwrotnej kolejnosci.

```c
main(){
  int i=0,liczba=1;
  int tablica[50];
  while(liczba!=0){
    printf("Podaj element numer %d :", i);
    scanf("%d",&liczba);
    tablica[i]=liczba;
    printf("Element %i = %i\n",i,liczba);
    i++;
  }
  printf("WYPISUJE!\n");
  for(i=i-2;i>=0;i--) printf(" Element %i = %i\n",i,tablica[i]);
}
```

ZADANIE 5 - zamiana na system dwojkowy
```c
#include <stdio.h>
main(){
int liczba=8;
int i;
int wynik[20];
printf("Podaj liczbę w systemie 10: ");
scanf("%i",&liczba);
i=0;
while(liczba!=0)
{
	wynik[i]=liczba%2;
	printf(" RESZTA %i przez 2 = %i ",liczba,wynik[i]);
	liczba=liczba/2;
	printf(" PO PODZIELENIU LICZBA =  %i \n", liczba);
	i++;
}
printf("\nWYNIK:");
for(i=i-1;i>=0;i--) printf(" %i ",wynik[i]);


}

```
#Zajecia 3 niedziela

zad.1
```c
/*Wczyta liczbe calkowita i wypisze czy jest wieksza od 5*/

#include <stdio.h>
main()
{
  int liczba;
 printf ("podaj liczbe");
 scanf ("%d",&liczba);
 printf ("%d",liczba);
 if(liczba>5)
   printf ("liczba %d  wieksza niz 5\n",liczba);
  else
    printf ("liczba %d jest mniejsza lub rowna 5\n",liczba);
}
```
zad.2
```c
/*Wczyta liczbe calkowita i wypisze czy jest dodatnia,ujemna czy rowna 0*/

#include <stdio.h>
main()
{
  int liczba;
 printf ("podaj liczbe \n");
 scanf ("%d", &liczba);
 printf ("%d\n",liczba);
 if(liczba>0)
   printf ("liczba %d dodatnia \n",liczba);
 else if (liczba<0)
   printf ("liczba %d jest ujemna \n",liczba); 
 else
   printf ("liczba %d rowna 0 \n",liczba);
 return 0;
}
```
zad.3
```c
/*Wczyta liczbe calkowita i wypisze czy jest parzysta czy nieparzysta*/

#include <stdio.h>
main()
{
  int n;
  printf ("podaj liczbe \n");
scanf ("%d", &n);
printf ("%d\n", n);

if(n%2==0)
printf ("liczba %d jest parzysta \n",n);
else
printf ("liczba %d jest nieparzysta \n",n);
return 0;
}
```
zad.4
```c
/*Wczyta 2 liczby całkowite i wypisze ktora z nich jest wieksza JESZCZE ZLE

#include <stdio.h>
main()
{
  int n,n2;
  prinf ("podaj liczbe \n");
  scanf ("%d", &n);
  printf ("podaj druga liczbe \n");
  scanf ("%d", &n2);

  if(n=n)
    printf ("liczby %d  sa rowne \n",n,n2);
    else
      printf ("liczby %d sa rozne od siebie \n",n,n2);
}

```
zad 4
```c
/*Sprawdzi czy liczby sa sobie rowne.*/
  int liczba,liczba2;
  printf("Podaj liczbe \n");
  scanf("%d",&liczba);
  printf ("Podaj druga liczbe \n");
  scanf("%d",&liczba2);

  if(liczba==liczba2) {
    printf("Liczba %d jest rowna liczbie %d\n",liczba,liczba2);
  }
  else {
    printf("Liczba %d nie jest rowna liczbie %d\n", liczba,liczba2);
  }
  return 0;
```
zad.5
```c
 /*Program, ktory wczyta 2 liczby calkowite i wypisze ktora z nich jest wieksza */


  int liczba,liczba2;
  printf("Podaj liczbe \n");
  scanf("%d",&liczba);
  printf ("Podaj druga liczbe \n");
  scanf("%d",&liczba2);

  if(liczba>liczba2) {
    printf("Liczba %d jest wieksza od liczby %d\n",liczba,liczba2);
  }

  else if(liczba==liczba2){
    printf("Liczba %d jest rowna liczbie %d\n",liczba,liczba2);
  }

  else {
    printf("Liczba %d jest mniejsza od liczby %d\n", liczba,liczba2);
  }
  return 0;
  ```
  zad.6 (to samo co 8)
  ```c
  /*Napisac program, ktory wczytuje liczbe calkowita n wieksze rowne 0, a nastepnie n liczb rzeczywistych 
(double %lf) i drukuje te liczby w trzech kolumnach w taki sposob, zeby zachowac krycie (
tzn. kropka dziesietna zawsze byla w tych samych kolumnach) np. gdy uzytkownik 
poda 7 0.12 -31.5 2.5 -59.01 26.4 -12.0 8.3 */

  int n;
  int i;
  printf("Podaj n:\n");
  scanf("%i",&n);
  //deklaracja tablicy
  double tab [n];
  //petla wczytujaca dane do tablicy, petla czyli for
  for (i=0;i<n;i++)
    scanf("%lf",&tab[i]);
  //petla wypisujaca dane z tablicy
  for(i=0;i<n;i++){
    printf("%2.5lf |",tab[i]);
  if(i%3==2)
    printf("\n");
  }
  /*Mozna zakladac. ze liczby naleza do przedzialu (-100,100), zeby wydrukowal l.rzeczywista na 
  polu o dl. 6 znakow z 2 cyframi po kropce nalezy w komendzie printf uzyc formatu "%6.2lf". 
  komenda ./zad6 > plik_z_danymi wpiszemy wartosci w pliku, a 
  komenda ./zad6 <plik_z_danymi otwieramy program przy wykorzystaniu danych z pliku*/
```
zad 8
```c
#include <stdio.h>
main()
{
 int n;
 int i;
  printf ("podaj n\n");
  scanf ("%i", &n);
  //deklaracja tablicy
  double tab[n];
  //petla wczytujaca dane do tablicy
  for (i=0;i<n;i++)
    scanf ("%lf", &tab[i]);
  //petla wypisujaca dane z tablicy
  for (i=0;i<n;i++){
    printf("%2.5lf\n",tab[i]);
  if(i%3==2)
    printf("\n");
  }
}
```
#ZADANIA Z KARTKI - ZADANIA Z JEZYKA C (pętle i tabele - zadania elementarne)

zle zad.1
```c
#include <stdio.h>
int main()
{
int tab[]={1,3,7,8,9};
 int i;

 for (i=0;i<=4;i++){
   printf("%d", &tab[i]);
 }
}
```
zad1 poprawione
```c
#include<stdio.h>
int main (){
  int tab[]={1,3,7,8,9};
  int a;
    for (a=0; a<=4; a=a++)
    printf (" %i ", tab[a]);

  return 0;
}   
```
zle zad 5
```c
#include <stdio.h>
int main(){
int tab[5];
int i;

//wczytywanie danych do tabeli
for (i=0;i<=4;i++);
scanf("%i", &tab[i]);
//wypisywanie danych z tabeli
for (i=0;i<=4;i++){
  printf("i",tab[i]);
 }
if(n<=o)
  printf("%lf");
 }
}
```
zad 5 poprawione - trzeba do tego stworzyc plik z danymi
```c
#include<stdio.h>
int main (){
  int tab[5];
int a;
  for (a=0; a<=4; a++)
  scanf ("%i", &tab[a]);
      for (a=4; a>=0; a=a-1)
    printf (" %i", tab[a]);

  return 0;
}
```
zad 8
```c
#include<stdio.h>
int main (){
  int tab[5];
int a;
//scanowanie do tabeli
  for (a=0; a<=4; a++)
  scanf ("%i", &tab[a]);
//wyświetlenie wyników w tabeli
  for (a=0; a<=4; a++)
  printf (" %i ", tab[a]);
  printf (" \n\n");
//zamiana komórek miejscami
  tab[0]=tab[4];
   for (a=0; a<=4; a=a++)
    printf (" %i ", tab[a]);
  printf (" \n\n");
return 0;
}
```
zad 10
```c
#include<stdio.h>
int main (){
  int tab[5];
  int tabela[5];
int a;
//scanowanie do tabeli
  for (a=0; a<=4; a++)
  scanf ("%i", &tab[a]);
//wyświetlenie wyników w tabeli
  for (a=0; a<=4; a++)
  printf (" %i ", tab[a]);
  printf (" \n\n");
//dwukrotnie powiększenie wartości w tabeli pierwszej
     for (a=0; a<=4; a=a++)
    printf (" %i ", 2*tab[a]);
  printf (" \n\n");
return 0;
}
```
