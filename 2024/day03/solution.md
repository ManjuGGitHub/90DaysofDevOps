
# Basic Linux Commands - Day 3

Task 1: View the content of a file and display line numbers.
Steps to create file with any content and view the same file:
    step1: create file demo.txt with [hello everyone, welcome to #90daysofdevops challenge.....]
        cat > demo.txt #press ENTER, note: there are few other way to create demo.txt, you can use anyone ex: vim,nano
        hello everyone
        welcome to #90daysofdevops
        my name is Manju and connect me on LinkedIn: Manjunath Gudur
        #Press ctrl+d to save and exit
    step2: to view demo.txt content with line number
        cat -n demo.txt #refer task 1.png for hands on screenshots

![image](https://github.com/ManjuGGitHub/90DaysofDevOps/blob/master/2024/day03/image/task%201.png)

Task 2: Change the access permissions of files to make them readable, writable, and executable by the owner only.

file system has below details for every file/directory in Linux
-rwxr-xr-- 1 owner group 1 july 01 file_name

- represents its file
d represents its directory
l represents its link
rwx - owner of this file has read, write and execute permissions[any user/root]
r-x - group has read and execute permissions
r-- - othefr user only has read permission
1 - represents symbolic link
july 01 - date and time of file updated
file_name - file name will be at the end

Access modes/ Permissions
r - 4   - to add read permissions to file
w - 2   - to add write permissions to file
x - 1   - to add executable permissions to file

if you want to give read, write and execute permissions - 7 [ 4+2+1 ]
if you want to give only read and execute permissions - 5 [ 4+1 ]
if you want to give only read permissions - 4

if you want to give read,write and execute permission to owner and read,execute permission to group and only read permission to other user
give 754 permissions

To apply permissions you can use chmod command
    chmod 754 demo.txt

    I have created demo.txt for explaination
    -rw-rw-r-- 1 manju-devops devops_learner 38 Oct  7 11:49 demo.txt

    from the above:
    we can confirm that demo.txt is file by first letter i.e -
    we can see that owner[manju-devops] has read write permission and group[devops_learner] has read, write permissions and other user only has read permissions.

    To change the permission of the owner to have read write and execute permission, use below command
    chmod 754 demo.txt
    
    -rwx------ 1 manju-devops devops_learner 38 Oct  7 11:49 demo.txt

Task 3: Check the last 10 commands you have run.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%203.png)

Task 4: Remove a directory and all its contents.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%204.png)

Task 5: Create a `fruits.txt` file, add content (one fruit per line), and display the content.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%205.png)

Task 6: Add content in `devops.txt` (one in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava. Then, append "Pineapple" to the end of the file.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%206.png)
![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%2066.png)

Task 7: Show the first three fruits from the file in reverse order.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%207.png)

Task 8: Show the bottom three fruits from the file, and then sort them alphabetically.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%208.png)

Task 9: Create another file `Colors.txt`, add content (one color per line), and display the content.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%209.png)

Task 10: Add content in `Colors.txt` (one in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey. Then, prepend "Yellow" to the beginning of the file.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%2010.png)

Task 11: Find and display the lines that are common between `fruits.txt` and `Colors.txt`.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%2011.png)

Task 12: Count the number of lines, words, and characters in both `fruits.txt` and `Colors.txt`.

![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day03/image/task%2012.png)
