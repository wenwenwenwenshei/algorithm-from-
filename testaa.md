### 二分查找

基础版

```
# 返回值：找到就返回key在该数组中对应的下标，找不到返回-1

# key 是要查找的数字,不是下标！nums是传入的数组
def binarysearch(nums,key):
    l = 0
    h = len(nums)-1 
    while l <= h:
     mid = (l+h)/2
    if nums[mid] == key:
        return mid
    
    elif key < nums[mid]:
        h = mid -1
        
    elif key > nums[mid]:
        l = mid + 1          
return -1
print binarysearch([1,2,3,4,5,6],0)   
```

