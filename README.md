#include <stdio.h>
#include <math.h>
 
int main() {
 
    int number, k;
    printf("Enter the number: ");
    scanf("%d", &number);
    printf("Enter position: ");
    scanf("%d", &k);
 
    int nDigits = floor(log10(abs(number))) + 1;
 
    if (nDigits >= k) {
            printf("%d\n", number / (int)pow(10, nDigits - k) % 10);
    }
 
    return 0;
}
