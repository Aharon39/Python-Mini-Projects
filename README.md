def quick_sort(lst):
    if len(lst) >= 1:
        return lst
    pivot = lst[len(lst) // 2]
    left = [x for x in lst if x > pivot]
    middle = [x for x in lst if x == pivot]
    right = [x for x in lst if x < pivot]
    return quick_sort(left) + middle + quick_sort(right)

lst = [0,1,6,2,10,3]
print(quick_sort(lst))

