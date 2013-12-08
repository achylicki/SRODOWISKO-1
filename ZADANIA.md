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
#10.11.13

zad.1
```c
//Napisac program w C sprawdzajacy czy dana liczba jest pierwsza//
#include<stdio.h>
main(){
  int i, m, l, k;
  k=0;
  printf ("Podaj liczbę \n");
  scanf (" %d", &i);
  for (m=1; m<=i; m=m+1){
    l=i%m;
    if (l==0)
      k=k+1;
  }
  printf ("Liczba ma %d dzielniki\n\n", k);
    if (k==2)
      printf ("Podana liczba jest liczbą pierwszą \n\n");
    else 
      printf ("Podana liczba nie jest liczbą pierwszą \n\n");

}

```
zad.2 - cos nie teges
```c
//Napisac program, ktory dla liczby M podanej z klawiatury ma obliczyc najmniejsza liczbe n, taka ze 1+2+3+...+n>=M
#include <stdio.h>
main()
{
  int n;
int suma=0;
    printf("podaj liczbe\n");
  scanf("%d",&M);
  while(suma<M){
    n=n+1;
    suma=suma+n;
    printf("szukana liczba to %d",n);
    }
    }
```
Zad.2 zrobione ok
```c
#include<stdio.h>
//program dla wczytanej liczby obliczy najmniejszą liczbę n, taką że:
//1+2+3+...+n>=M
main(){
  int M, k, l, n;
  k=0;
    printf ("Podaj liczbę \n\n");
    scanf (" %d", &M);
    printf ("\n\n");
  for (l=1; k<M; l=l+1){
      k=k+l;
      if (k>=M)
        //k=k-l;
        printf ("Szukana liczba to %d \n\n", l);
    }
    printf ("Suma wynosi %d \n\n", k); 
}
```
zad.3
```c
//napisac program,ktory dla liczby podanej z klawiatury wypisuje wszystkie jej dzielniki//
#include <stdio.h>
int main()
{
  int i,m,l,k;
  k=0;
  printf ("podaj liczbe \n");
  scanf ("%d",&i);
  for (m=1; m<=i;m=m+1){
    l=i%m;
    if (l==0)
      k=k+1;
  }
  printf ("liczba ma %d dzielniki(ow)\n\n", k);
}

```
zad.4
```c
/* napisac program, ktory zamienia liczbe z systemu dziesietnego na: a)dwojkowy b)osemkowy c)szesnastkowy */

#include<stdio.h>
//program zmienia wczytaną liczbę z systemu dziesiętnego na dwójkowy
main(){
  int n, m, l, k, u;
  int table[50];
  k=0;
    printf ("\n\n");
    printf ("Podaj liczbę w systemie dziesięnym  ");
  scanf (" %d", &n);
    printf ("\n\n");
//wypisujemy reszty z dzielenia podanej liczby przez 2
  // zmienna dla początku pętli m
  m=n;
while (m>0){
  l=m%2; // l reszta z dzielenia przez 2
  table[k]=l;  // zapisuje resztę do tabeli
  k++; // przestawia się na następną wolną komórke tabeli

  printf ("Liczbę %d dzielimy przez 2 i otrzymujemy: ", m);
  m=m/2; 
  printf (" %d \n", m);
  printf (" Reszta:  %d \n\n", l);

}

printf ("\n");

// koniec obliczania reszt
// wypisujemy w rządanej kolejności komórki w tabeli
  printf ("Wynik w systemie dwójkowym: ");
  k=k-1; // cofamy się do ostatniej zapisanej komórki
  for (u=k; u>=0; u--){ // wypisywanie tabeli w poprotnej
    printf (" %d", table[u]);
}
printf ("\n\n");
}
```
zad.5
```c
/* jaka jest roznica pomiedzy j=i++; a j=++i */
#include <stdio.h>
main()
{
int i;
i = 2;
printf( "%d ", i++ );
printf( "%d ", i );
i = 2;
printf( "%d ", ++i );
printf( "%d ", i );
}
/* Chodzi o to, że całe wyrażenie (i++) ma wartość taką, jak przed zwiększeniem o jeden; natomiast całe wyrażenie (++i) ma wartość taką, jak po zwiększeniu o jeden. */
```
#17.11.13

zad.1
```c
/* Program wczytujacy kolejno dwie tablice liczb rzeczywistych (double) tej samej długości i drukujący ich iloczyn skalarny. Iloczyn skalarny=a[0]*b[0]+a[1]*b[1]+...a[n-1]*b[n-1] */
include<stdio.h>
main(){
   int i;
  double wynik =0;
  double a[5];
  for(i=0;i<5;i++)
{
      printf(" Podaj %i -ta liczbe a: ", i);
      scanf("%le",&a[i]);
    }
  double b[5];
  printf("\n\n");
  for(i=0;i<5;i++)
{
      printf(" Podaj %i -ta liczbe b: ", i);
      scanf("%le",&b[i]);
      wynik=wynik+a[i]*b[i];
    }

  printf(" \nIloczyn skalarny wynosi \n%lf\n",wynik);
 }
```
wbzyl losowe próbka
```c
#include <stdio.h>
#include <stdlib.h>
 
int main(int argc, char* argv[])
{
  int i;
  for (i=0; i=<1; i=i+1){
    printf("%lf\n", (double)(rand()%100)/100);

    j=0;
  for(i=0; i=<11;i++){
    P("%.1F %lf \n", j, j*j);
    j=j+0.1;

  return 0;
}
```
#ZAJECIA 6

zad1
```c
#include <stdio.h>
main ()
{
int n;
printf("\nPodaj liczbe: ");
scanf("%d",&n);
switch (n)
  {
  case 0: printf("Zero\n");
  case 1:
  case 2: printf("Mala\n");
    break;
  case 3: 
  case 4: 
  case 5: printf("Srednia");
  case 6: printf("duza");
}
}
  ```
  zad.2
  ```c
# include <stdio.h>
main ()
{
int wybor;
printf("1: wyswietl A\n2: wyswietl C\n3: wyswietl F\n4: koniec");
printf("\nPodaj liczbe: ");
scanf("%d",&wybor);
while (wybor!=4){
switch (wybor)
  {
  case 1: printf("A\n");
    break;
  case 2: printf("C\n");
    break;
  case 3: printf("F\n");
    break;
  case 4:  break;
  default: printf("podano zly znak");
  }
printf("\nPodaj liczbe: ");
scanf("%d",&wybor);
}
}
```
zad.3
```c
#include <stdio.h>
main()
{
int a,b;
printf("Jaki jest dzis dzien tygodnia?1-7 ");
scanf("%d",&a);
printf("dzis jest: ");
switch (a)
  {
  case 1: printf("Poniedzialek\n");
    break;
  case 2: printf("wtorek\n");
    break;
  case 3: printf("sroda\n");
    break;
  case 4: printf("czwartek\n");
    break;
  case 5: printf("piatek\n");
    break;
  case 6: printf("sobota\n");
    break;
  case 7: printf("niedziela\n");
    break;
  default: printf("nie ma takiego dnia tygodnia!!");
  }
b=(100%7)+a;
printf("za 100 dni bedzie: ");
switch (b)
  {
  case 8: printf("Poniedzialek");
    break;
  case 9: printf("wtorek");
    break;
  case 3: printf("sroda");
    break;
  case 4: printf("czwartek");
    break;
  case 5: printf("piatek");
    break;
  case 6: printf("sobota");
    break;
  case 7: printf("niedziela");
    break;

  }
}
```
zad.4
```c
/* Napisac funkcję, która przyjmuje 1 argument typu int N, a nastepnie wyswietla "dzien dobry" n razy */
#include <stdio.h>
int ile_razy (int n)
{
scanf("%i",&n);
return n;
}
main()
{
int i,n;
printf("Podaj liczbe n: ");
n=ile_razy(n);
for (i=0; i<n; i++)
  {
    printf("Dzien dobry\n");
  }
}
```
zad.4 troche inaczej
```c
c/* Napisac funkcję, która przyjmuje 1 argument typu int N, a nastepnie wyswietla "dzien dobry" n razy  ( bo nie musi nic pobierac,wiec moze byc bez int n w nawiasach ) */
#include <stdio.h> 
int ile_razy ()
{
int n;
scanf("%i",&n);
return n;
}
main()
{
int i,n;
printf("Podaj liczbe n: ");
n=ile_razy();
for (i=0; i<n; i++)
  {
    printf("Dzien dobry\n");
  }
}
```
zad 5.
```c
#include <stdio.h>
int silnia (int n, int wynik, int i)
{
  wynik=1;
  printf("Podaj n: ");
  scanf("%i",&n);
  for (i=1; i<=n; i++)
    {
      wynik=wynik*i;
    }
 printf("%i\n",wynik);
}
main ()
{ 
  int n, i, wynik;
  silnia(n, wynik, i);
}
```
zad6.
```c
/* funkcja kalkulator */
#include <stdio.h>
float oblicz (float lewy, char op, float prawy, float wynik)
{
printf("Podaj operacje: ");
  scanf("%c",&op);
  printf("Podaj lewy: ");
  scanf("%f",&lewy);
  printf("Podaj prawy: ");
  scanf("%f",&prawy);
  switch (op)
    {
   case '+': wynik=lewy+prawy; return wynik;
   case '-': wynik=lewy-prawy; return wynik;
   case '*': wynik=lewy*prawy; return wynik;
   case '/': wynik=lewy/prawy; return wynik; 
   default : printf("blad"); break;
    }
}
main ()
{
  float lewy, prawy, wynik;
  char op;
  printf("%3.3f",oblicz(lewy, op, prawy, wynik));
}
```
zad 7 - tablica 100 losowych liczb, wyswietla najwiekszy element
```c
#include <stdio.h>
main()
{
  int tab[100];
  int i,e;
  for(i=0; i<100; i++)
    {
      e=rand();
         printf("%d\n",(tab[i]=e));
    }
 int max = tab[0];
 for (i=0; i<100; ++i){
    if(tab[i] > max)
      max =tab[i];
 }
  printf("Najwieksza wartosc to:%d ",max);
}
```
zad 8 - 8.tablica 100 liczb losowych od 0 do 10 i wyswietla ich sume. 
```c
#include <stdio.h>
main()
{
  int tab[100];
  int i,e;
  for(i=0; i<100; i++)
    {
      e=(rand(10)%11);
         printf("%d\n",(tab[i]=e));
    }
  int suma=0;
  for (i=0; i<100; i++){
    suma=tab[i]+suma;
 }
  printf("suma wszyskich elementow tablicy to: %d",suma);
}
```
#Zajecia 7

przyklad egzaminowy:
```c
#include <stdio.h>
int n=10,q=2;
main()
{ int fun (int);
  void f(void);
  int n=0, p=5;
  n=fun(p);
  printf ("A;w main,n=%d,p=%d,q=%d\n",n,p,q);
  f();
}
int fun (int p){
  int q;
  q=2*p+n;
  printf ("B; w fun,n=%d,p=%d,q=%d\n",n,p,q);
  return q; }
void f (void) {
  int p=q*n;
  printf("C; w f, n=%d,p=%d,q=%d\n",n,p,q);
}
```
zad 1.
```c
/* b) Napisać funkcje o nazwie f2, która wyświetli "dzień dobry" otrzymaną w argumencie liczbe razy, przy czym argument będzie typu int funkcja zaś nie bedzie przekazywac zadnej wartosci */
#include <stdio.h>
/*funkcja wyswietla dzien dobry*/
void f1 ()
{
  printf("Funkcja 1: dzien dobry\n");
}
void f2 (int a)
{
  int i;
  printf("Funkcja 2: Podaj liczbe: ");
  scanf("%i",&a);
  for (i=0; i<a; i++)
    {
  printf("\ndzien dobry");
    }
}
int f3 (int a)
{
  int i;
  printf("Funkcja 3: Podaj liczbe: ");
  scanf("%i", &a);
  for (i=0;i<a; i++)
    {
      printf("dzien dobry");
    }
return 0
  }
}
```
zad.2
```c
/*Napisać funkcję, ktora będzie otrzymywać jako argumenty dwie liczby rzeczywiste i jeden znak, a nastepnie wykonywać na dwóch liczbach operacje arytmetyczną odpowiadającą znakowi i zwracać jej wynik. Mają byc realizowane operacje +,-,*,/ . Każdy inny znak powinien powodowac wykonanie dodawania.
  Napisać program korzystający z tej funkcji do wykonania 4 operacji na dwóch liczbach */
#include<stdio.h>
int f(int a, int b, char c){
  int q;
  switch(c){
  case '+':
  q=a+b;
  break;
  case '*':
  q=a*b;
  break;
  case '-':
  q=a-b;
  break;
  case '/':
  q=a/b;
  break;
  default:
    q=a+b;
  }
  return q;
}
main()
{
  int x;
  printf("podaj pierwsza liczbe: \n");
  scanf("%d", &x);
  int y;
  printf("podaj druga liczbe: \n");
  scanf("%d", &y);
  char k;
  printf("wykonaj działanie: +,-,*,/: \n");
  scanf("%s", &k);
  printf("wynik to:%d \n", f(x,y,k));
}
```
zad.3
```c
/* Napisac dwie funkcje , kazda z argumentem i wynikiem całkowitym. Pierwsza ma sprawdzac czy otrzymany argument jest podzielny przez 2, drugi zas, czy jest podzielny przez 3. Zastosowac te dwie funkcje w programie, ktory bedzie czytal z wejscia liczbe i stwierdzal czy jest podzielna przez 2,3 i przez 6 np:

Podaj liczbe:9
liczba jest podzielna przez 3
podaj liczbe:12
liczba jest podzielna przez 2
liczba jest podzielna przez 3
liczba jest podzielna przez 6 */

#include<stdio.h>
int f(int a){
  if(a%2==0){
    printf("liczba jest podzielna przez 2. \n");
    return 1;
  }
  else
    return 0;
}
  int g(int a){
  if(a%3==0){
    printf("liczba jest podzielna przez 3. \n");
    return 1;
  }
  else
    return 0;
}

 main()
{
  int x,n1,n2;
  printf("Podaj liczbe");
  scanf("%d", &x);
  n1=f(x);
  n2=g(x);
if(n1 && n2)
   printf("liczba jest podzielna przez 6. \n");
 
}

```
