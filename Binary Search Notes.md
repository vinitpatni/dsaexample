- Floor in sorted array
 <pre markdown="2">
   largest value in the array which is smaller or equal to given value
  for example :- 1 3 5 8 12 15 17 (5 is floor for 7), (8 is floor for 8) (12 is floor for 14)
    int ans = -1;
    while (left <= right) {
      int mid = (left + right) / 2;
      if (arr[mid] <= target) {
           ans = arr[mid];
           left = mid + 1;
      } else {
           right = mid - 1;
      }
    }
 </pre>
- Ceiling in sorted array
 <pre markdown="2">
   Smalles value in the array which is greater than or equal to given value
  for example :- 1 3 5 8 12 15 17 (8 is ceiling for 7), (8 is ceiling for 8) (15 is celing for 14)
    int ans = -1;
    while (left <= right) {
      int mid = (left + right) / 2;
      if (arr[mid] >= target) {
           ans = arr[mid];
           right = mid - 1;
      } else {
           left = mid + 1;
      }
    }
 </pre>        
- Lower Bound

Lower Bound is applicable for sorted array only. For a number 'target' lower bound is defined as the lowest index 'i' in the array for which is x[i] >= target

For example lets consider the array :- [1,1,1,2,2,2,3,3,7,9,9,10]

Lower Bound of 2 = 3 (3 is index)
Lower Bound of 1 = 0 (0 is index)
Lower Bound of 4 = 8 (8 is index)
Lower Bound of 10 = 11 (11 is index)
Lower Bound of 13 = 12 (size of array)

- Upper Bound Trick 
Upper Bound is applicable for sorted array only. For a number 'target' upper bound is defined as the lowest index 'i' in the array for which is x[i] > target

For example lets consider the array :- [1,1,1,2,2,2,3,3,7,9,9,10]

Upper Bound of 2 = 6 (6 is index)
Upper Bound of 1 = 3 (3 is index)
Upper Bound of 4 = 8 (8 is index)
Upper Bound of 10 = 12 (size of array)
Upper Bound of 13 = 12 (size of array)

Floor and Celing on TreeMap in java
TreeMap map = new TreeMap();
map.floorKey() and map.ceilingKey()
