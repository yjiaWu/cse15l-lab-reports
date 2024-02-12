# Part1: Bugs
**1. Failed test** <br>
the input is `int[] input1 = {1,2,3,4,5,6}`, and the test would faile with this input. <br>
```
@Test 
  public void testReversedFailed(){
    int[] input1 = {1,2,3,4,5,6};
    int[] expected = new int[]{6,5,4,3,2,1};
    assertArrayEquals(expected, ArrayExamples.reversed(input1));
  }
```
**2. Passed test which didn't find the code bug** <br>
the input is `int[] input1 = { }`. The test would show pass because the array is an empty array which would test out the bug of the original code. <br>
```
@Test
  public void testReversed() {
    int[] input1 = { };
    int[] expected = {};
    assertArrayEquals(expected, ArrayExamples.reversed(input1));
  }
```
**3. Symptom** <br>
For the test with input of empty array, the test shows it passed. However for the test with elements in the array, the message shows the outcome is different with the expected output. The expected output for the element at index 0 is 6 but the outcome is 0. Therefore we know that the code didn't reserve the array in a correct order. <br>
![image](Labreport3symptom.png) <br>

**4. Fixed Bugs** <br>
*Before*: <br>
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
Originally, we create the `newArray` aiming to pass the element in `arr` in a reserve order. However, the for loop assign `arr[i]`'s element with `newArray[arr.length - i - 1]`. Since we create the `newArray` with 0 as it's element, the array `arr` would be all 0 as its element after the for loop. Therefore, we didn't succesfully reserve the array. <br>

*After*: <br>
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
The above code fixed the bug. I switch the position of `newArray` with `arr` in the for loop. I put `newArray` in the left, and `arr` in the right. Now, the for loop would assign the element in `arr` into `newArray` in a reverse order correctly. <br>

# Part 2: Researching commands 







