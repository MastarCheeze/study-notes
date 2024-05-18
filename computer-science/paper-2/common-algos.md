# Common Algorithms

-   [Linear search](#linear-search)
-   [Bubble sort](#bubble-sort)
-   [Totalling](#totalling)
-   [Counting](#counting)
-   [Finding maximum/minimum](#finding-maximumminimum)
-   [Finding average](#finding-average)

## Linear search

```
Found <- FALSE
Index <- 0

WHILE Found = FALSE DO
    IF Array[Index] = SearchValue THEN
        Found <- TRUE
    ELSE
        Index <- Index + 1
    ENDIF
ENDWHILE
```

## Bubble sort

```
FOR I <- 1 TO N
    FOR J <- 0 TO N-1
        IF Array[J] > Array[J+1] THEN
            Temp <- Array[J]
            Array[J] <- Array[J+1]
            Array[J+1] <- Temp
        ENDIF
    NEXT J
NEXT I
```

Video: [Michael Sambol](https://youtu.be/xli_FI7CuzA?si=Z0B6BmNTOU4hIpx9)

## Totalling

## Counting

## Finding maximum/minimum

## Finding average
