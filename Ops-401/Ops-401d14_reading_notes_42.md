# Readings: Pass the Hash with Mimikatz
Below you will find reading materials and additional resources that support today’s topic and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

## Reading
[What is Mimikatz?](https://www.varonis.com/blog/what-is-mimikatz/)

### Name the six credential-gathering techniques which Mimikatz is able to perform and explain how two of them work.
Mimikatz is capable of performing the following six credential-gathering techniques:
1. Pass-the-hash
2. Pass-the-ticket
3. Overpass-the-hash (pass-the-key)
4. Kerberoast golden tickets
5. Kerberoast silver tickets
6. Pass-the-cache

**Pass-the-hash** technique allows an attacker to use a captured NTLM hash to authenticate to a target computer without needing to know the actual password. It exploits the way Windows used to store password data, essentially using the hash as a master key.

**Pass-the-ticket** is a method where attackers use a Kerberos ticket to gain access to a computer or network resource. Mimikatz can manipulate or create tickets, enabling an attacker to impersonate a legitimate user, bypassing the need for a password.

### What are four ways we can defend against Mimikatz attacks. Explain how two of the mitigations can stop Mimikatz.
Four ways to defend against Mimikatz attacks include:
1. Restricting admin privileges
2. Disabling password-caching
3. Turning off debug privileges
4. Configuring additional local security authority (LSA) protection

**Restricting admin privileges** limits the number of users with administrative access, reducing the chance of an attacker gaining the necessary permissions that Mimikatz requires to extract credentials from the system.

**Disabling password-caching** prevents the storage of password hashes in the system registry, which Mimikatz targets to retrieve authentication credentials. By setting the cache to zero, it removes the stored hashes that Mimikatz would otherwise exploit.

