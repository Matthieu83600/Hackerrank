## Solution

```Javascript
/*
 * Complete the 'breakingRecords' function below.
 *
 * The function is expected to return an INTEGER_ARRAY.
 * The function accepts INTEGER_ARRAY scores as parameter.
 */

function breakingRecords(scores) {
    // Write your code here
    // Compteurs 
    let bestCount = 0;
    let worstCount = 0;
    // Correspond au meilleur et pire score
    let bestScore = scores[0];
    let worstScore = scores[0];
    
    for(let i = 0 ; i < scores.length ; i++) {
        if (scores[i] > bestScore) {
            bestScore = scores[i];
            bestCount += 1;
        } else if (scores[i] < worstScore) {
            worstScore = scores[i];
            worstCount += 1;
        }
    }
    
    return [bestCount, worstCount];

}
```