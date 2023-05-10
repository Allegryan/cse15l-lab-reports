# **Lab Report 2 - Servers and Bugs (Week 3)** 
## **Part 1** 
The following is the code for creating a web server called StringServer:
![image](https://user-images.githubusercontent.com/130011927/234147093-08a00274-b35b-43d0-a847-3e72d2e3cf80.png)

**Screenshot 1 of using the "/add-message" request line:**
![image](https://user-images.githubusercontent.com/130011927/234147199-ee6f64ac-285c-49ce-9439-e7875602d5e5.png)
- The method(s) being used here is simply the `handleRequest()` method. 
- The only relevant (and really only) class field required is the "results" field. It initially starts as an empty string, and gets updated each time the "/add-message" request line is called with a value. In terms of arguments given to the method, the given `URI url` changes when a new url is typed in order to add a new message to the resulting string.
- From this specific request, the class field of results gets altered. It goes from

> "Hello\nHow are you\nGood! What about you?\n"

to

> "Hello\nHow are you\nGood! What about you?\nGreat! Thanks for asking\n"

**Screenshot 2 of using the "add-message" request line:**
![image](https://user-images.githubusercontent.com/130011927/234149741-d15431e1-35a2-4862-bb29-79efad44e79a.png)
- Once again, the only method being used here is simply the handleRequest() method
- Like the first example, the only relevant class field is the results field, which is added upon with each call of the "/add-message" request line. Again, the URI url changes with each new url that is typed.
- From this specific request, the results fields goes from 

> "Hello\nHow are you\nGood! What about you?\nGreat! Thanks for asking\n"

to

> "Hello\nHow are you\nGood! What about you?\nGreat! Thanks for asking\nOkay bye now...\n"

## **Part 2**
For this part, I'll be looking at the bug(s) from the `reverseInPlace()` method.

Failure-inducing input:
```
public void testReverseInPlace() {
    int[] input2 = {1, 2, 3, 4, 5, 6};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{6, 5, 4, 3, 2, 1}, input2);
	}
```

Input that *does not* induce a failure:
```
public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
    }
```

The symptom (showing the failure happening through the test):
![image](https://user-images.githubusercontent.com/130011927/234151696-0a481bba-eaf5-46ae-bfe8-0dbae6097f4e.png)

Fixing the bug(s) (Before and After):

**Before:**
```
static void reverseInPlace(int[] arr){
  for(int i = 0; i < arr.length; i += 1){
    arr[i] = arr[arr.length - i - 1];
  }
}
```

**After:**
```
static void reverseInPlace(int[] arr){
  for(int i = 0; i < arr.length / 2; i++){
    int temp = arr[i];
    arr[i] = arr[arr.lengthj - i - 1];
    arr[arr.length - i - 1] = temp;
  }
}
```

In order to fix `reverseInPlace`, I had to set the condition for the for loop to be the length of the integer array, arr, divided by 2. After that, I would swap the value at arr[i] with the value that is the same distance from the end of the array as arr[i] is from the beginning of the array. Prior to this change, the original code would go through the first half of the array and replace it with the second half of the array. This in concept is fine, but the loop would continue past the halfway point, so the values in the array after the halfway mark would not be replaced with values that came prior, as they should have.

## **Part 3**
For me, the most interesting thing I learned from the past two labs was the running/creation of different servers! Making use of servers, URLs, and websites was especially cool because, since they've become such an everyday part of our already habitual internet usage, being able to apply the concepts that I've learned about coding onto creating simple search engines and servers makes me super eager at the thought of new possibilities and ideas that I can think of now that I have the basic blueprint learned!
