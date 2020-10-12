# Exercise #1 - findNeedles
By: Daniel Nicholson

---

## findNeedles

```public static void findNeedles(String haystack, String[] needles)```

Counts the number of times that each element in the `needles` string array appears within the `haystack` string and prints the results. The `needles` string array can contain five or fewer elements. If `needles` has more than five elements, the method only prints an error message. A regular expression splits the `haystack` string to remove all spaces, single and double quotation marks, tabs, line feeds, word boundaries, form feeds, and carriage returns. The print results include each element from `needles` that matches with another in `haystack` and a count for each match.

|  Parameters |  |
|---|---|
| needles | **String (Array)**: The search string. This array cannot contain more than five elements. |
| haystack  | **String**: The string being searched.  |

---

## Code suggestions 

The `for` loop is creating the `haystack` array for each element in the `needles` string array. Creating the `haystack` array just once may provide some performance gains.
