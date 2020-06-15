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
 For 2D array ar[r][c] (2,5) compiler allocates r×c(2×5=10) continues celles in RAM, 2D array is stored in flat 1D array in memory as shown in below image<br>
![DS](/images/9_4_two_dimentional_array_in_RAM.PNG) <br>

### Common Operations on Array
 * [Declare , instantiation, initialization](#declare_instantiation_initialization)
 * Insert value
 * Travese
 * Accessing a cell
 * Searching a value
 * Deleting a value
#### Time and Space complexity of 1D Array
![DS](/images/9_11_time_and_space_complexity_1D_array.PNG) <br>
#### Declare instantiation initialization 
* Declare : compiler creates refference variable (int[] studentIdArray)
* Instantiation : allocates **n** no of cells and store fist index in referrence variavle variable (int[] studentIdArray=new int[n])
* Initialization :assign values to cells -> by default int array is filled with 0 <br>
![DS](/images/9_5_declare_and_initialize_array.PNG) <br> <br>
**Time complextiy of Declare , instantiation, initialization** <br>
 if we declare and intialize array in single step , time complexity is just **O(1)** , that is because instead of initializing with defuat value compiler is initializing value privided by us.<br>
 if we dont do in single step then during instantiation compiler initializes with 0 and during initialization it itrates and assign values to each cell wich is **O(n)** complexity<br>
![DS](/images/9_6_time_complexity_declare_and_initialize_array.PNG) <br><br>
#### Insert value
![DS](/images/9_7_time_complexity_insertvalue_array.PNG) <br>
#### Travese
![DS](/images/9_8_time_complexity_traverse_array.PNG) <br>
#### Accessing a cell
![DS](/images/9_9_time_complexity_accessing_cell_array.PNG) <br>
#### Searching a value 
![DS](/images/9_10_time_complexity_search_array.PNG) <br>
