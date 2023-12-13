# Insertion Sort Procedure

This repository contains a Pascal-like pseudocode implementation of the Insertion Sort algorithm.

## Procedure

```pascal
PROCEDURE InsertionSort(arr: array)
VAR
    n: INTEGER
    i, j, key: INTEGER
BEGIN
    n := length(arr)
    for i := 1 to n - 1 DO
        key := arr[i]
        j := i - 1

        while (j >= 0) and (key < arr[j]) do
            arr[j + 1] := arr[j]
            j := j - 1
        end while

        arr[j + 1] := key
    end for
END
```
