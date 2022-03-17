# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (actualAge){
  if (actualAge == 1){
    return {
      humanYears: actualAge,
      catYears: 15,
      dogYears: 15,
    }
  }

  if (actualAge == 2){
    return {
      humanYears: actualAge,
      catYears: 24,
      dogYears: 24,
    }
  }

  return {
    humanYears: actualAge,
    catYears: (actualAge - 2) * 4 + 24,
    dogYears: (actualAge - 2) * 5 + 24,
  }
}
```

| Input | Output     |
| ----- | ---------- |
| 3     | 3, 28, 29  |
| 6     | 6, 40, 44  |
| 12    | 12, 64, 74 |
| 1     | 1, 15, 15  |
| 2     | 2, 24, 24  |

<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program is a calculator for how old a person is in cat and dog years based on their current age. 
    The caculator is, for every 1 year of life for us, you subtract 2, multiply by 4 for cats or 5 for dogs and then add 24. 
    There are two variables that are not calculated though because of the 2 year subtraction, so if you input a 1 or a 2, 
    it just has a hard coded answer of 15 and 24 respectively.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
