# Coding_practice
##All my answer questions of my coding problems 

#01. Given two arrays of A and B respectively of sizes N1 and N2, the task is to calculate the product of the maximum element of the first array and minimum element of the second array.

```cpp
long long find_multiplication(int a[], int b[], int n, int m)
    {
        // Complete the function
        int max = INT_MIN;
        int min = INT_MAX;
        for(int i = 0; i< n; i++){
            if(max < a[i]){
                max = a[i];
            }
        }
        for(int i = 0; i< m; i++){
            if(min > b[i]){
                min = b[i];
            }
        }
        return max*min;
    }
```
