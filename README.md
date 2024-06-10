# C-Program-to-Check-Prime-Number-By-Creating-a-Function-

#include <stdio.h> 
  
// Defining the function 
int primenumber(int number) 
{ 
    int i; 
    
    // Condition for checking the 
    // given number is prime or 
    // not 
    for (i = 2; i <= number / 2; i++)  
    { 
        if (number % i != 0) 
            continue; 
        else
            return 1; 
    } 
    return 0; 
} 
  
// Driver code 
int main() 
{ 
    int num = 7, res = 0; 
    
    // Calling the function 
    res = primenumber(num); 
    if (res == 0) 
        printf("%d is a prime number", num); 
    else
        printf("%d is not a prime number", num); 
}
