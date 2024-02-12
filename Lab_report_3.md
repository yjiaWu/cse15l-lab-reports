# Part1_Bugs
1. Failed test <br>
the input is `int[] input1 = {1,2,3,4,5,6}`, and the test would faile with this input. <br>
```
@Test 
  public void testReversedFailed(){
    int[] input1 = {1,2,3,4,5,6};
    int[] expected = new int[]{6,5,4,3,2,1};
    assertArrayEquals(expected, ArrayExamples.reversed(input1));
  }
```
2. Passed test which didn't find the code bug <br>
the input is `int[] input1 = { }`. The test would show pass because the array is an empty array which would test out the bug of the original code. <br>
```
@Test
  public void testReversed() {
    int[] input1 = { };
    int[] expected = {};
    assertArrayEquals(expected, ArrayExamples.reversed(input1));
  }
```
3. Symptom <br>
For the test with input of empty array, the test shows it passed. However for the test with elements in the array, the message shows the outcome is different with the expected output. The expected output for the element at index 0 is 6 but the outcome is 0. <br>




