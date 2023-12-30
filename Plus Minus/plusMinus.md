## Solution

```Javascript
/*
 * Complete the 'plusMinus' function below.
 *
 * The function accepts INTEGER_ARRAY arr as parameter.
 */
function plusMinus(arr) {
    // Write your code here
    let positive = 0;
    let negative = 0;
    let zero = 0;
    let sizeArray = arr.length;
    arr.forEach((num) => {
        if (num > 0) {
            positive++;
        } else if (num < 0) {
            negative++;
        } else {
            zero++;
        }
    })
     console.log((positive/sizeArray).toFixed(6) + "\n" + (negative/sizeArray).toFixed(6) + "\n" + (zero/sizeArray).toFixed(6));
}
```