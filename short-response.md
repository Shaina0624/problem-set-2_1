# Problem Set 2.1
## Types, Values, and Operators

1. What is a _unary operator_? Give an example of one.
It is when one uses one operator for an operaant. For instance, i++.
Examples of unary operators include: + , - , * , /.

2. What is a _binary operator_? Give an example of one.
It is when one uses two operators to compare operants. For instance, i <= num.
Examples of binary operators include: > , < , = , == , === , != , !==.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.
I see ternary operator as a type of if else function that includes a : and a ?.
Examples include: 
const age = 26;
const beverage = age >= 21 ? "Beer" : "Juice";
console.log(beverage); // "Beer"

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
A strict eqality is a === it has to have the same type of values. 
Example include "3" === "3"
A non-strict equality is a == and it doesn't need to have the same type of values.
Example: 3 == "3"

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
Primitive:
-Number : 23
-String : "23"
-Boolean: true
-NULL: null
-Undefined :undefined
-Symbol:
Non-Primitive:
-Object

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
string

7. What does the code below return?
  ```javascript
  typeof true;
  ```
boolean

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
number

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
NULL bc it has no value

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
Falsy:
-undefined
-null
-NaN
-0
-"" or ''
-false
Truthy: any value that is true and !== 0
1
true

11. Evaluate the following expressions using JavaScripts implicit coercion rules. For each example, in one sentence, explain what coercions were applied and why:
  * `8 * null`
- 8 is a number and null is NULL and bc of the * it will return 0 bc null is falsy
  * `"5" - 1`
- "5" is a string and 1 is a number and bc of the - it will return 4 bc js reads "5" as a number despite it being in a string
  * `"5" + 1`
- "5" is a string and 1 is a number and bc of the + it will return 6 bc js reads "5" as a number despite it being in a string
  * `true + false` true and false are both booleans and bc of the + it will return 1 bc when booleans are treated as numbers true will be 1 and false will be 0 and 0 + 1 = 1.
  * `"i am" + undefined`
- "i am" is a string and undefined is a Undefined and bc of the + it will return i amundefined bc undefined doesn't like to be treated as a number
  * `5 + undefined`
- 5 is a number and undefined is a Undefined and bc of the + it will return NaN bc undefined is not a number and doesn't like being treated as such.

12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
   false

   ```javascript
   (false || undefined);
   ```
   undefined
   
   ```javascript
   (undefined || false);
   ```
   false

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
   undefined

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
   undefined
   
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
   
   false

   ```javascript
   ((false || undefined) && (false && undefined));
   ```

  undefined

   ```javascript
   ('a' || (false && undefined) || '');
   ```

  'a'

   ```javascript
   ((false && undefined) || 'a' || '');
   ```

  'a'

   ```javascript
   ('a' && (false || undefined) && '');
   ```

  undefined

   ```javascript
   ((false || undefined) && 'a' && '');
   ```
  undefined
