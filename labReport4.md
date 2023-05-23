# Lab Report 4: Vim - Doing it All from the Command Line (Week 7)
## Step 4 of 9: Log into ieng6

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/92460d68-f21b-4b69-968c-8b4b2c4836fa)

*Keypresses:* s,s,h,`<SPACE>,<CTRL-V>,<ENTER>`

The `<CTRL-V>` was used here in order for me to paste my username for ieng6 -- saving me time in having to type it all in. I also did not need to type in my password as I set up an SSH key for it beforehand.

## Step 5 of 9: Clone fork of repository

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/59d72cc3-bf26-46c4-94c4-075a37137139)

*Keypresses:* `<CTRL-V>,<ENTER>`

For this step, I simply pasted in the command to clone the repository.

## Step 6 of 9: Run the tests, demonstrating that they fail

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/862ce9b4-67f9-4f16-8a6e-fd9e7d73fdde)

*Keypresses:* c,d,`<SPACE>`,l,a,b,7,`<ENTER>,<up>,<up>,<up>,<up>,<up>,<up>,<up>,<up>,<ENTER>` 

For this step, I first changed the directory to that of lab7. Then, the bash command `bash test.sh` to run the tester was 5 positions up in the search history, so I simply used the up arrow keys to access it and run it.

## Step 7 of 9: Edit the code to fix the failing test

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/4c217b15-ab45-4683-a61f-53fcd3b06c38)

*Keypresses:* `<up>,<up>,<up>,<up>,<up>,<up>,<up>,<ENTER>`

Similar to the last step, to open the vim editor, I simply went back 7 positions in the search history to run the `vim ListExamples.java` command 

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/380d3973-ad1d-4e8a-9514-cbda557a04e2)

*Keypresses:* `<SHIFT-/>`,i,`<ENTER>`,e,r,2,:,w,q,`<ENTER>`
  
Then, I used the shortcuts found in the vim editor in order to quickly and efficiently jump to and solve the issue. More specifically, I jumped to the final while loop found in the code (the section in which the error was located) by moving to the latest instance of the letter 'i'. From here, I changed `index1` to `index2` in order for the code to iterate the right variable. 

## Step 8 of 9: Run the tests, demonstrating that they now succeed

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/f504acfb-b6ac-48b3-bf2d-654f44f6606c)

*Keypresses:* `<up>,<up>,<ENTER>`

For this step, I once again ran the tester -- this time only needing to move back 2 positions in the search history as I had just used it prior in step 6.

## Step 9 of 9: Commit and push the resulting change to your GitHub account

![image](https://github.com/Allegryan/cse15l-lab-reports/assets/130011927/b37ef047-a5bf-4d18-92da-a3a342e1fccb)

*Keypresses:* g,i,t,`<SPACE>`,p,u,s,h,`<ENTER>`

For this step, I attempted to commit and push the changes to GitHub, but, as I was having trouble doing it in lab as well, I was unable to successfully do so given I was unable to log my credentials and the SSH key shortcut was not working at the time of setting it up either.

