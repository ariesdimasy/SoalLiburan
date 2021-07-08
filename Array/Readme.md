# Array

<details>
<summary> Soal 001</summary>

```js
/*
    ==================
    WordToArrayReverse
    ==================

    [INSTRUCTION]
    buatlah sebuah program yang mengconvert string menjadi array, yang di reverse
    posisinya berdasarkan per kata

    [RULE]
    - dilarang menggunakan function bawaan javascript kecuali split

    [EXAMPLE]

    wordToArrayReverse("Hello my name is Dimas")
    output:["Dimas","is","name","my","Hello"]

    wordToArrayReverse("Lorem ipsum sit dolor amet")
    output:["amet","dolor","sit","ipsum","Lorem"]

\*/

function wordToArrayReverse(str) {
  // your code here
}

wordToArrayReverse("Hello my name is Dimas");
//["Dimas","is","name","my","Hello"]

wordToArrayReverse("Lorem ipsum sit dolor amet");
//["amet","dolor","sit","ipsum","Lorem"]
```

</details>

<details>
<summary> Soal 002</summary>

```js
/*
    ======================
    String to Multidimensi
    ======================

    [INSTRUKSI]
    diberikan sebuah string yang jumlah characternya bisa di akar pangkat
    (4, 9, 16, 25 , ... ) 
    ubahlah karakter - karakter itu menjadi array multidimensi
    dimana hasil akar pangkat jumlah karakternya menjadi row dan col

    [EXAMPLE]

    stringToMultidimensi("0120194124213712")
    jumlah char : 16 
    row dan col = akat 16 
    row dan col = 4
    output: 
    [
         1 2 3 4 
        [0,1,2,0], 1 
        [1,9,4,1], 2 
        [2,4,2,1], 3
        [3,7,1,2]  4
    ]

 */

function stringToMultidimensi(str) {
  // your code here
}

stringToMultidimensi("0120194124213712");
/*
    [
        [0,1,2,0],
        [1,9,4,1],
        [2,4,2,1],
        [3,7,1,2]
    ]
 */

stringToMultidimensi("01201941242137127");
/*
    // char count invalid
 */
```

</details>

<details>
<summary> Soal 003</summary>

```js
/*
    ========================
    Multidimensi into String
    ========================

    [INSTRUKSI]
    diberikan sebuah array multidimensi, tugas kalian adalah mengconvert
    dari array multidimensi menjadi string 

    [RULE]
    - array harus multidimensi , bila tidak multidimensi output : "input is invalid"

    [EXAMPLE]
    multidimensiIntoString([
        [4,3,2,1,5],
        [4,2,7,9,3],
        [7,4,3,7,3],
        [4,6,3,6,8],
        [3,2,5,6,4]
    ])  
    output: 4321542793743734636832564

    multidimensiIntoString([1,2,3,4])
    output: input is invalid

*/

function multidimensiIntoString(arr) {
  // your code here
}

multidimensiIntoString([
  [4, 3, 2, 1, 5],
  [4, 2, 7, 9, 3],
  [7, 4, 3, 7, 3],
  [4, 6, 3, 6, 8],
  [3, 2, 5, 6, 4],
]);
// 4321542793743734636832564

multidimensiIntoString([1, 2, 3, 4]);
// input is invalid
```

</details>

<details>
<summary> Soal 004</summary>

```js
/* 
    ===================
    Two Array Operation
    ===================

    Buatlah sebuah Program yang dapat mengoperasikan bilangan - bilangan yang ada
    didalam 2 buah array sesuai dengan masing - masing indexnya.

    [INSTRUCTION]
    diberikan 2 buah array yang akan dioperasikan 
    - jika bilangan tersebut berada pada index yang genap, maka tambahkan (+)
    bilangan pada index array yang ke satu dengan index array yang ke dua 
    - jika bilangan tersebut berada pada index yang ganjil, maka kurangkan (-)
    bilangan pada index array yang ke satu dengan index array yang ke dua 
    - jika panjang ke dua array tidak sama , 
    maka masukkan saja bilangan - bilangan tersebut ke dalam hasilnya 

    [EXAMPLE]
    twoArrayOperation([1,2,3],[1,2,3])
    array1 : [1, 2, 3]
              +  -  +
    array2 : [1, 2, 3]
    result : [2, 0, 6]

    twoArrayOperation([12,34,11,23,12],[11,78,45,20,42])
    array1 : [12, 34, 11, 23, 12]
               +   -   +   -   +
    array2 : [11, 78, 45, 20, 34]
    result : [23,-44, 56, 3, 46]

    twoArrayOperation([-4, 5, 57, 33, -90, 0],[4, 2, 54, 24])
    array1 : [-4, 5, 57, 33, -90, 0]
              +   -   +   -    +
    array2 : [4,  2, 54, 24,  34]
    result : [0,  3, 111, 9, -56, 0]

*/

function twoArrayOperation(arr1, arr2) {
  // your code here
}

console.log(twoArrayOperation([-4, 5, 57, 33, -90, 0], [4, 2, 54, 24, 34])); // [ 0, 3, 111, 9, -56, 0]
console.log(twoArrayOperation([12, 34, 11, 23, 12], [11, 78, 45, 20, 42])); // [ 23, -44, 56, 3, 54 ]
console.log(twoArrayOperation([1, 2, 3], [1, 2, 3])); // [ 2, 0, 6 ]
```

</details>

<details>
<summary> Soal 005</summary>

```js
/*
    =======================
    Alphabet Multidimension
    =======================

    Buatlah sebuah function yang berfungsi mengenerate Alphabet Multidimension. 
    yang artinya di dalam array multidimension terdapat alphabet yang isinya 
    berurutan. dimana Array multidimension nya memiliki row dan col yang sama
    
    [EXAMPLE]
    alphabetMultidimension(6)

    maka output nya adalah : 

    [
        [A,B,C,D,E,F],
        [G,H,I,J,K,L],
        [M,N,O,P,Q,R],
        [S,T,U,V,W,X],
        [Y,Z,A,B,C,D], <--- perhatikan, jika sudah sampai z maka , kembali lagi ke A
        [E,F,G,H,I,J]
    ]
*/

function alphabetMultidimension(num) {
  // code
}

console.log(alphabetMultidimension(6));
/*
output:
[
    [A,B,C,D,E,F],
    [G,H,I,J,K,L],
    [M,N,O,P,Q,R],
    [S,T,U,V,W,X],
    [Y,Z,A,B,C,D],
    [E,F,G,H,I,J]
]
*/
```

</details>
