## Solution

```Javascript
/*
 * Complete the 'miniMaxSum' function below.
 *
 * The function accepts INTEGER_ARRAY arr as parameter.
 */
function miniMaxSum(arr) {
    // Write your code here
    let minSum = 0;
    let maxSum = 0;
    let sortedArray = arr.sort();
    
    for(let i = 0; i < arr.length; i++){
        if( i < arr.length -1 ) {
            minSum += arr[i]
        } 
        if (i > 0) {
            maxSum += arr[i]
        }
    }
    console.log(minSum, maxSum);
}
}
```