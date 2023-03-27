#include <stdio.h>
#include <stdlib.h>

int main(){
 
    double a, b;
    double sum = 0;
    char o;
    printf("Enter operator\n");
    scanf("%c", &o);
    printf("Enter first operand\n");
    scanf("%lf", &a);
    printf("Enter second operand\n");
    scanf("%lf", &b);

    if (o == '+'){
        sum = a + b;
        printf("The result is %lf\n", sum);
    } else if (o == '-'){
        sum = a - b;
        printf("The result is %lf\n", sum);
    } else if (o == '*'){
        sum = a*b;
        printf("The result is %lf\n", sum);
    } else if (o == '/'){
        if (b != 0){
        sum = a / b;
            printf("The result is %lf\n", sum); 
        }
        else printf("Error");
    }

    getchar();

    return 0;

}


