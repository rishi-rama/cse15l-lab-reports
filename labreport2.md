# Lab Report #2
## Part 1
This screenshot shows my code for StringServer:
![image](https://user-images.githubusercontent.com/122561679/215654439-7de3693c-2ee4-4b63-af38-fcd66f9a9b5f.png)
This shows me adding the first string:
![image](https://user-images.githubusercontent.com/122561679/215655731-d7490cd0-a1ed-4726-b241-ebf9d3f03da9.png)
* The `storage` string begins as empty
* Then, the `handleRequest` method is called with the argument being the url, `http://localhost:4000/add-message?s=This%20is%20my%20first%20string!`
* After this, the relevant field changed is `input`, which becomes `This is my first string!`
* The value of `input` is appended to the `storage` string. Now the `storage string` is equal to
```

This is my first string!
```

![image](https://user-images.githubusercontent.com/122561679/215655785-03f410a7-ebe6-44e2-914c-fe819f9f41fe.png)
* The `storage` string begins as `This is my first string!`
* Then, the `handleRequest` method is called with the argument being the url, `http://localhost:4000/add-message?s=and%20now,%20I%27m%20adding%20a%20second%20one`
* After this, the relevant field changed is "input", which becomes "and now, I'm adding a second one"
* The value of `input` is appended to the `storage` string. Now the `storage` string is equal to
```

This is my first string!
and now, I'm adding a second one
```
## Part 2
**Failure-inducing input:**
* JUnit test:
```
@Test 
public void testReverseInPlace() {
    int[] input1 = {1,2,3};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{3,2,1}, input1);
}
```
* Failure-inducing input: {1,2,3}
* Expected output: {3,2,1}
* Actual output: {3,2,3}
* Screenshot:
![image](https://user-images.githubusercontent.com/122561679/215666846-1d08d522-ba4c-49fe-8be0-0e9f4fbed0ac.png)

**Non failure-inducing input:**
* JUnit test:
```
@Test 
public void testReverseInPlace() {
    int[] input1 = {1};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{1}, input1);
}
```
* Non failure-inducing input: {1}
* Expected output: {1}
* Actual output: {1}
* Screenshot:
![image](https://user-images.githubusercontent.com/122561679/215666716-8201a9ab-3fc1-4a7b-9e41-e1affbdb7561.png)

**Fixing Bug:**
reverseInPlace code before:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
}
```
reverseInPlace code after:
```
static void reverseInPlace(int[] arr) {
    int[] tempArr = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      tempArr[i] = arr[i];
    }
    for(int i = arr.length-1; i >= 0; i -= 1) {
      arr[i] = tempArr[arr.length - i -1];
      
    }
}
```
The problem with the prior buggy code is that it once it reaches the halfway point of arr[], it fails because it looks at the values of arr[] which it changed itself. In order to fix this, I created a temp array tempArr[] which is a copy of the non reversed arr[]. Then, using these original values the values of arr[] are appropriately ordered.
