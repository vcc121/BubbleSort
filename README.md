# BubbleSort
Take sample code
constant MAX = 9

define main function:
    create array values with [7, 3, 9, 4, 6, 1, 2, 8, 5]
    
    print "Before:"
    call printValues(values)

    create x = 3
    create y = 5
    print x and y
    call swap(x, y)
    print x and y after swap

    call sort(values)

    print "After:"
    call printValues(values)
    return 0

define printValues function:
    print "["
    for i from 0 to MAX - 1:
        print array[i]
        if i is not MAX - 1:
            print a space
    print "]"

define swap function(a, b):
    store a in temp
    set a to b
    set b to temp

define sort function:
constant MAX is max length of array
function sort (array):
    create integer variables i and j
    for i from zero to MAX - 1:
        for j from zero to MAX - 1:
            if array[j] > array[j+1]:
                swap array[j] with array[j+1]
                printArray(array)
