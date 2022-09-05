# Selection Sort

<img src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20220203094305/Selection-Sort-Flowhchart.png" alt="Selection Sort">

Let's consider the arr = [64, 25, 12, 22, 11]

### First Phase
For the first position in the sorted array, the whole array is traversed from index 0 to 4 sequentially. The first position where 64 is stored presently, after traversing whole array it is clear that 11 is the lowest value.

```
64      25      12      22      11
```

Thus, replace 64 with 11. After one iteration 11, which happens to be the least value in the array, tends to appear in the first position of the sorted list.

```
11      25      12      22   64
```

### Second Phase 
For the second position, where 25 is present, again traverse the rest of the array in a sequential manner.

```
11      25      12      22      64
```

After traversing, we found that 12 is the second lowest value in the array and it should appear at the second place in the array, thus swap these values.
```
11      12      25      22      64
```

### Third Phase 
Now, for third place, where 25 is present again traverse the rest of the array and find the third least value present in the array.
```
11      12      25      22      64
```

While traversing, 22 came out to be the third least value and it should appear at the third place in the array, thus swap 22 with element present at third position.
```
11      12      22      25      64
```

### Fourth Phase 
Similarly, for fourth position traverse the rest of the array and find the fourth least element in the array As 25 is the 4th lowest value hence, it will place at the fourth position.

```
11      12      22      25      64
```

### Fifth Phase 
At last the largest value present in the array automatically get placed at the last position in the arrayThe resulted array is the sorted array.
```
11      12      22      25      64
```

## Approach 
- Initialize minimum value(min_idx) to location 0.
- Traverse the array to find the minimum element in the array.
- While traversing if any element smaller than **min_idx** is found then swap both the values.
- Then, increment min_idx to point to next element.
- Repeat until array is sorted.