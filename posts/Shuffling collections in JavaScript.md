# Create a Collection Shuffling Function in JavaScript

*Utilize a custom function that can shuffle any given collection in JavaScript.*

JavaScript does not inherently have a built-in function to shuffle a collection, but you can easily create one using the
Fisher-Yates (or Knuth) shuffle algorithm. This algorithm works by selecting an element from the collection and swapping
it with the current element, iterating through the collection in this manner until every element has been shuffled.

## JavaScript Implementation

Here's a simple implementation of the Fisher-Yates shuffle for an array in JavaScript:

```javascript
function shuffleArray(array) {
    let currentIndex = array.length, temporaryValue, randomIndex;
    // While there remain elements to shuffle...
    while (0 !== currentIndex) {

        // Pick a remaining element...
        randomIndex = Math.floor(Math.random() * currentIndex);
        currentIndex -= 1;

        // And swap it with the current element.
        temporaryValue = array[currentIndex];
        array[currentIndex] = array[randomIndex];
        array[randomIndex] = temporaryValue;
    }
    return array;
}


```

This `shuffleArray` function will return a new array with the same elements as the original, but in a random order. It
uses JavaScript's built-in `Math.random()` function to generate the randomness needed for the shuffle. You can test this
code by running the following code:

```javascript
// Testing shuffleArray function
let arr = [1, 2, 3, 4, 5];
arr = shuffleArray(arr);
console.log(arr);
```

## TypeScript Implementation

In TypeScript, you'd maintain the same logic but explicitly define the type of data in your array:

```typescript
function shuffleArray(array: number[]): number[] {
    let currentIndex = array.length;
    let temporaryValue: number;
    let randomIndex: number;

    while (0 !== currentIndex) {
        randomIndex = Math.floor(Math.random() * currentIndex);
        currentIndex -= 1;

        temporaryValue = array[currentIndex];
        array[currentIndex] = array[randomIndex];
        array[randomIndex] = temporaryValue;
    }
    return array;
}
```
