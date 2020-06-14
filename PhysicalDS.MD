# Physical Datastrucures
  **Array*
  **Linked List**
## Array
  Array is a data structure consisting of a colloction of similar elements,each identified by array inded.An array is stored such that the position of each element can be computed from its index cell by a methamatical formula.

### Types of Array
![DS](/images/9_1_array_types.PNG) <br>
![DS](/images/9_2_array_types.PNG) <br>

### How Arrays Stored in RAM
**One Dimentional Array** <br>
  Arr[col]<br>
  Arr[5] = {10,20,30,40,50}<br>
  When declare array with size 5(n), compiler allocates 5(n) continues cells in the RAM.Starting address can be anything but it will be n continues cells<br>
![DS](/images/9_3_one_dimentional_array_in_RAM.PNG) <br><br>
**Two Dimentional Array** <br>
 Arr[row][col]<br>
 Arr[2][5] = {{10,3,20,7,99},{63,15,33,55,44}}<br>
 For 2D array ar[r][c] (2,5) compiler allocates r*c(2*5=10) continues celles in RAM, 2D array is stored in flat 1D array in memory as shown in below image<br>
![DS](/images/9_4_two_dimentional_array_in_RAM.PNG) <br>
