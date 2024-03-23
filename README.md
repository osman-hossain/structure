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
