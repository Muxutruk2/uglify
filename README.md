# Uglify

This python script uglifies a C file by moving the charachters in char_list to the right (10 spaces to the right of the longest line)

## Installation

Clone the repo and cd into it

```bash
git clone https://github.com/Muxutruk2/uglify && cd uglify
```

Move the C file to the folder and run or make [input] and [output] absolute paths

```bash
python main.py -i [input] -o [output]
```

## Examples

input.c

```c
#include <stdio.h>
struct student {
    char name[50];
    int roll;
    float marks;
} s;

int main() {
    printf("Enter information:\n");
    printf("Enter name: ");
    fgets(s.name, sizeof(s.name), stdin);

    printf("Enter roll number: ");
    scanf("%d", &s.roll);
    printf("Enter marks: ");
    scanf("%f", &s.marks);

    printf("Displaying Information:\n");
    printf("Name: ");
    printf("%s", s.name);
    printf("Roll number: %d\n", s.roll);
    printf("Marks: %.1f\n", s.marks);

    return 0;
}
```

output.c

```c
#include <stdio.h>                                 
struct student                                    {
    char name[50]                                 ;
    int roll                                      ;
    float marks                                   ;
} s                                               ;

int main(                                       ) {
    printf("Enter information:\n"                );
    printf("Enter name: "                        );
    fgets(s.name, sizeof(s.name), stdin          );

    printf("Enter roll number: "                 );
    scanf("%d", &s.roll                          );
    printf("Enter marks: "                       );
    scanf("%f", &s.marks                         );

    printf("Displaying Information:\n"           );
    printf("Name: "                              );
    printf("%s", s.name                          );
    printf("Roll number: %d\n", s.roll           );
    printf("Marks: %.1f\n", s.marks              );

    return 0                                      ;
}
```
