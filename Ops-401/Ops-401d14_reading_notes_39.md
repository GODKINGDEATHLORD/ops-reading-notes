# [Understanding SQL Injection, Identification and Prevention](https://www.varonis.com/blog/sql-injection-identification-and-prevention-part-1)

1. What is SQL injection?

    SQL injection is a type of attack that exploits flaws in a web application's interaction with its database through the use of SQL commands. An attacker can manipulate these flaws to execute unauthorized SQL commands, which can lead to unauthorized data access or operations.

2. Can you give an example of how a hacker could use SQL injection to gain unauthorized access?

    An example of a SQL injection attack could be altering an `id` value in a URL from a benign number to a malicious SQL command. For instance, changing `/show_me_the_cheese?id=1` to `/show_me_the_cheese?id=(UPDATE products SET price = 0.1 WHERE ID = 1)` could potentially alter database records if the system is vulnerable.

3. What are some ways to prevent SQL injection attacks on a web server?

    To prevent SQL injection attacks, web servers can implement user input sanitization to filter out harmful SQL patterns, use parameterized queries to ensure the form of the SQL command is correct before execution, and apply web application firewalls like ModSecurity for Apache or Naxsi for Nginx to block malicious requests.
