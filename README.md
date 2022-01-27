# Markdown : les bases  
Source : https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## Les exemples de code : spécifier un langage particulier
Par exemple, pour du javascript :
```js
// Rajouter ```js pour du code javascript
function sumTwoSmallestNumbers(numbers) {  
  return numbers.sort((a,b)=>a-b).slice(0,2).reduce((prev,curr)=>prev+curr);
}
``` 

## Les listes : rajouter 4 espaces pour que le bloc de code suive l'indentation des bullet-list
Par exemple :
- Array sort https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort  
  - Tri par défaut : basé sur les caractères
    ```js
    return [3, 87, 45, 12, 7].sort();
    // Result = [ 12, 3, 45, 7, 87 ]
    ```
  - Tri par ordre croissant numérique
    ```js
    return [3, 87, 45, 12, 7].sort((a,b)=>a-b);
    // Result = [ 3, 7, 12, 45, 87 ]
    ```
  - Tri par ordre décroissant numérique
    ```js
    return [3, 87, 45, 12, 7].sort((a,b)=>b-a);
    // Result = [ 87, 45, 12, 7, 3 ]
    ```

- Array slice : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
```js
return [3, 87, 45, 12, 7].slice(0,1);
// Result = [ 3 ]

