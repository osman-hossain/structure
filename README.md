<!--comment line-->
_S_~~tru~~__c__`ture`  
---

<p> It's a programme of c contain structure related things.</p>

- [x] Initial
- [x] 
- [x]

<ol>
<li>starting</li>
<li>about</li>
</ol>

### initial

```c
#include<stdio.h>
struct person
{
    int age;
    float salary;
};
int main()
{
    struct person person1,person2;

    person1.age=50;
    person1.salary=80,000.50;

    printf("Person 1\n");
    printf("Age = %d\n",person1.age);
    printf("Salary = %.2f\n\n",person1.salary);

    person2.age=46;
    person2.salary=60,000.50;

    printf("Person 2\n");
    printf("Age = %d\n",person2.age);
    printf("Salary = %.2f\n",person2.salary);

    getch();

}
```  
---
<image src="./images/initial.png" width="500" title="initial"/>  

### Local && Global

- [x] Defferent Declaration
- [x] outside 

<p style="text-align:center; color :lightblue;">Inside main function of struct is local and outside can be use in other called global.</p> 

## Local
```c
#include<stdio.h>
int main()
{
    struct person
    {
        int age;
        float salary;
    };
    struct person person1,person2;

    person1.age=40;
    person1.salary=20000.60;

    printf("Person 1\n\n");
    printf("Age = %d\n",person1.age);
    printf("Salary = %.2f\n\n",person1.salary);

    person2.age=30;
    person2.salary=25000.50;

    printf("Person 2\n\n");
    printf("Age = %d\n",person2.age);
    printf("Salary = %.2f\n\n",person2.salary);

    getch();
}
```

<image src="./images/local.png" width="500" title="Local"/>

## Glaobal

```c
#include<stdio.h>
struct person
{
    int age;
    float salary;
};
struct person person1,person2;
int main()
{
    person1.age=35;
    person1.salary=40000.50;

    printf("Person 1\n\n");
    printf("Age = %d\n",person.age);
    printf("Salary = %.2f\n\n",person.salary);

    person2.age=26;
    person2.salary= 30000.50;

    printf("Person 2 \n\n");
    printf("Age = %d\n",person.age);
    printf("Salary = %.2f\n\n",person.salary);

    getch();
}
```
![Global](./images/global.png)

### Input information

```c
#include<stdio.h>
    struct person
    {
        int age;
        float salary;
    };
    struct person person1,person2;
int main()
{
    printf("Enter Person 1 Age : ");
    scanf("%d",&person1.age);

    printf("Enter Person 1 Salary : ");
    scanf("%f",&person1.salary);

    printf("Person 1\n\n");
    printf("Age = %d\n",person1.age);
    printf("Salary = %.2f\n\n",person1.salary);

    printf("Enter Person 2 Age : ");
    scanf("%d",&person2.age);
    printf("Enter Person 2 Salary : ");
    scanf("%f",&person2.salary);

    printf("Person 2\n\n");
    printf("Age = %d\n",person2.age);
    printf("Salary = %.2f\n\n",person2.salary);

    getch();
}
```  
<image src="./images/inputinformation.png" width="400" title="input-information"/>  

### practice

- [x] Directly initialised
- [x] Transfer one element to another

```c
#include<stdio.h>
struct person
{
    int age;
    float salary;
};
int main()
{
    struct person person1={20,35000.50};
    struct person person2,person3;

    person2.age=30;
    person2.salary=40000.40;

    person3=person2;

    printf("Person 1\n\n");
    printf("Age = %d\n",person1.age);
    printf("Salary = %.2f\n\n",person1.salary);

    printf("Person 2\n\n");
    printf("Age = %d\n",person2.age);
    printf("Salary = %.2f\n\n",person2.salary);

    printf("Person 3\n\n");
    printf("Age = %d\n",person3.age);
    printf("Salary = %.2f\n\n",person3.salary);

    getch();
}
```  
<image src="./images/diff.png" width="500" title="different-angle"/>  

### compare

```c
#include<stdio.h>
struct person
{
    int age;
    float salary;
};
int main()
{
    struct person person1={20,40000.50};
    struct person person2,person3;

    person2.age=30;
    person2.salary=40000.60;

    person3=person2;

    if(person1.age==person2.age && person1.salary==person2.salary)
    {
        printf("Person 1 is equal to person 2.\n");
    }
    else
    printf("Person 1 is not equal to person 2.\n");

    getch();
}
```
<image src="./images/notequal.png" width="500" title="not equal"/>  

```c
#include<stdio.h>
struct person
{
    int age;
    float salary;
};
int main()
{
    struct person person1={20,40000.50};
    struct person person2,person3;

    person2.age=30;
    person2.salary=40000.60;

    person3=person2;

    if(person2.age==person3.age && person2.salary==person3.salary)
    {
        printf("Person 2 is equal to person 3.\n");
    }
    else
    printf("Person 2 is not equal to person 3.\n");

    getch();
}
```  
![Equal](./images/equal.png)  
</br>
