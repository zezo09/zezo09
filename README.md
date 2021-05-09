-#include<stdio.h>
#include<stdbool.h>
int num_digits(int num){
    int count = 0;
    while (num != 0) {
        num /= 10;
        ++count;
    }
    printf("Number of digits: %d", count);
}

int main() {
    int num = 0;
    printf("Enter an positive integer: ");
    scanf("%d", &num);
    num_digits(num);
}
