# Lab Report 5: Debugging and Reflection (Week 9/10)

## Part One: Debugging

### Student:
**Title:** Error while testing reverseInPlace method

**Category:** Debugging 

Hi all, I was working on the Array portion of Lab 3 and I ran into the following when trying to test my `reverseInPlace()` method:

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/cdc48f87-42ec-4528-b961-232aefa2b232)

When running the bash script for the testing, it doesn't really seem to give me much information in regards to the error itself, such as what my array looks like or even just what index the error is occuring at...
If someone could help me out with trying to fix this, that would be great -- thanks!!

### TA Response: 

Hey, sorry for the wait! In order for me to help you out better, do you mind providing a screenshot of the error message that occurs when running the JUnit tester through VS Code itself? In case you forgot, you can 
do this by hitting the "Testing" icon on the far left, which looks like so:

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/daa2ed71-20c5-4733-b7e0-c00da2be852e)

Alongside a screenshot of the tester error, could you also provide a screenshot of the code and/or method that you are testing? I should be able to better pinpoint any potential errors made, if so!

Until then, all the best---

### Student:

Hi, thanks for taking on my request! The specific error message that I get is as follows:

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/6f113243-b2f2-4dd5-bf5f-efac9096b9af)

And here is the code that I'm having the problem in:

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/dc27051f-13a4-491f-8b12-60f9c686b3d0)

(Specifically the problem seems to be happening in the `reverseInPlace` method...)

Thanks again!

### TA Response:

The problem with your code is that it seems as if your array is not being fully reversed... Judging from the error message you received, your array manages to reverse at least the first index with the last. 
As for your implementation specifically, it looks like the way in which you handle the creation of the reversed array is the primary issue. 

With your current implementation, you are taking the given array, `arr` and swapping
the first and last values as intended. However, when your method reaches the value index 2, for example, what happens to the value that it is supposed to swap with? You've set the value at index 0 to the
value at the end of the array, but when you reach the end of the array and must change the value to the value that _was_ at index 0, it won't be there anymore.

The key to fixing this issue lies in finding a way to reverse the values of `arr` without losing the values in the middle of swapping. That way, you can actually swap them with their corresponding counterparts on the other half of
the array. 

I've given you what I believe to be enough to lead to a solution, but if anything is confusing or you need a bit more clarification, don't hesitate to ask! Until then, good luck with solving the issue!

### Student:

Okay I believe I figured it out, but I wanted to post this in case other students run into the same kind of issue that I did --

I realized from your replies that I needed to create a temporary variable, `temp`, to "hold" the value that I'm swapping. Then, after changing lets say the first value into the last, I can utilize a complete "swap"
by replacing the corresponding value in the back half of the array with the value held in `temp`. To do this though, I needed to adjust the `for` loop so that I only iterate through half of the array.
In case what I'm saying is a little bit confusing, I have a screenshot of a basic implementation of it:

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/1f5ca0ab-1890-43ba-a850-b074a23df62c)

Hope this helps you guys out for the assignment as well!

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/3de0b87f-8e96-4fe3-82da-6b6d4765f4ac)

## Part Two: Reflection

During this second half of the quarter, I personally think that the coolest thing that I learned came at the very end of the Week 9 Lab, after my groupmates and I finished going through the lab itself, just talking amongst ourselves and our tutor over the different uses and applications of coding and CS in general. I learned a lot about the prospects of applying for tutor positions, forming resumes and portfolios, and future CS classes during our brief yet informative discussion! In particular, talking about future classes such as CSE30 and CSE100 got me very curious and eager to see how my experience in those classes will go! It really kinda opened my eyes to the peculiarity of learning new coding languages and broadening my horizons and experiences through it! Basically, one of the best parts of 15L was being able to talk more with my peers and really getting a feel of the kind of community and discussions that can develop from this subject!





