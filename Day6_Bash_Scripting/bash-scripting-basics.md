# Linux Practical - Day 6 Bash Scripting Basics

## ✅ Objective
To learn basic Bash scripting for automation tasks in Linux.

---

## 1️⃣ Create a Simple Bash Script

Create file:

```bash
nano hello.sh

#!/bin/bash
echo "Hello DevOps World!"

Add:

#!/bin/bash
echo "Hello DevOps World!"


Run script:

bash hello.sh

2️⃣ Give Execute Permission
chmod +x hello.sh
./hello.sh

3️⃣ Variables in Bash
#!/bin/bash
name="Chandan"
echo "Welcome $name to DevOps!"

4️⃣ Taking User Input
#!/bin/bash
echo "Enter your name:"
read user
echo "Hello $user"

5️⃣ If-Else Condition
#!/bin/bash
echo "Enter a number:"
read num

if [ $num -gt 10 ]
then
  echo "Number is greater than 10"
else
  echo "Number is 10 or less"
fi

6️⃣ Loop Example
For loop:
#!/bin/bash
for i in 1 2 3 4 5
do
  echo "Iteration $i"
done

7️⃣ Useful Automation Script (Disk Usage)

Create script:

nano disk-check.sh


Add:

#!/bin/bash
echo "Disk Usage Report:"
df -h


Run:

chmod +x disk-check.sh
./disk-check.sh
