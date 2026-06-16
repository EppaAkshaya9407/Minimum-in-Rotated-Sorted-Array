# Minimum-in-Rotated-Sorted-Array
nums=list(map(int,input("Enter array elements: ").split()))
left=0
right=len(nums)-1
while left<right:
    mid=(left+right)//2
    if nums[mid]>nums[right]:
        left=mid+1
    else:
        right=mid
print("Minimum element:",nums[left])
