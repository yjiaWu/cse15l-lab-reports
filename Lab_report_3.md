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



