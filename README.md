# JavaScript Algorithms
## 1. Bubble Sort

![Bubble Sort](img/bubble_sort.gif) 

```javascript
function bubbleSort(arrayForSort) {
    var n = arrayForSort.length;
    for (var i = 0; i < n - 1; i++) {
        for (var j = 0; j < n - 1; j++) {
            if (arrayForSort[j] > arrayForSort[j + 1]) {
                var temp = arrayForSort[j];
                arrayForSort[j] = arrayForSort[j + 1];
                arrayForSort[j + 1] = temp;
            }
        }
    }
    return arrayForSort;
}
```

## 2. Selection Sort

![Selection Sort](img/selection_sort.gif)

```javascript
function selectionSort(arrayForSort) {
    var n = arrayForSort.length;
    for (var i = 0; i < n; i++) {
        var min = i;
        for (var j = i; j < n; j++) {
            if (arrayForSort[j] < arrayForSort[min]) {
                min = j;
            }
        }
        var temp = arrayForSort[min];
        arrayForSort[min] = arrayForSort[i];
        arrayForSort[i] = temp;
    }
    return arrayForSort;
}
```