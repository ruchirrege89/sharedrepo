Working with Git Repository from Multiple Computers.

In today's times, when accessibility to your work from anywhere is the key this git exercise helped me clear my concepts on how I can work on developing my codebase from any machine and anywhere.

Followed instructions from here - http://www.deanbodenham.com/learn/using-git-to-sync-different-computers.html

Summary:

Step 1 - Create a local repository on Machine A
  1 - create a folder where you want to store your code and 'cd' into the folder.
  2 - create a file in the folder (echo 'standing in line to see the show tonight' >> file1.txt)
  3 - git init
  4 - git add .
  5 - git commit -m 'Appropriate message'
  6 - Go to Github.com and login with your credentials
  7 - create a online repository (preferably with the same name as your local repository)
  8 - git remote add origin <<online repo URL>>
  9 - git push -u origin master

Step 2 - Clone the online repository on Machine B
  1 - 'cd' into the location you want the codebase to be in.
  2 - git clone <<<<online repo URL>>>>

Step 3
  3 - Make changes to the code base (echo "and there's a light on" >> file1.txt)
  4 - git add .
  5 - git commit -m "Appropriate message"
  6 - git push -u origin master

Step 4 - Pull modified repository again in Machine A
  1 - git pull origin master

You are all set! Steps 3 and 4 will keep repeating based on how often you use different machines.

Happy coding!
