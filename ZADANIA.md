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
