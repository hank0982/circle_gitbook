# If/Else Boolean

## If / Else

```javascript
if (condition1) {
    // block of code to be executed if condition1 is true
} else if (condition2) {
    // block of code to be executed if the condition1 is false and condition2 is true
} else {
    // block of code to be executed if the condition1 is false and condition2 is false
}
```

## Comparison Operator



| Operator | Description | Comparing | Returns |
| :--- | :--- | :--- | :--- |
| == | equal to | 8 == 8 | true |
|  |  | 8 == ''8" | true |
| === | equal value and equal type | 5 === 5 | true |
|  |  | 5 === "5" | false |
| != | not equal | 5 != 8 | true |
| !== | not equal value or not equal type | 5 !== 5 | false |
|  |  | 5 !== "5" | true |
|  |  | 5 !== 8 | true |
| &gt; | greater than | 5 &gt; 8 | false |
| &lt; | less than | 5 &lt; 8 | true |
| &gt;= | greater than or equal to | 5 &gt;= 8 | false |
| &lt;= | less than or equal to | 5 &lt;= 8 | true |

## Logical Operator



| Operator | Description | Example | Try it |
| :--- | :--- | :--- | :--- |
| && | and | \(5 &lt; 10 && 5 &gt; 1\)  | true |
| \|\| | or | \(2 == 5 \|\| 6 == 5\)  | false |
| ! | not | !\(x == y\)  | true |

### \(Optional\) Conditional \(Ternary\) Operator

```javascript
var voteable = (age < 18) ? "Too young":"Old enough";
```



