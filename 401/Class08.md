# Review, Research, and Discussion

## When is Basic Authorization used vs. Bearer Authorization?
The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret.The Bearer authentication scheme is dedicated to the authentication using a token.
<br/>
<br/>


## What does the JSON Web Token package do?
It is a standard used to create access tokens for an application. It works this way: the server generates a token that certifies the user identity, and sends it to the client.

## What considerations should we make when creating and storing a SECRET?
Use encryption to store secrets within .git repositories
* Use “Secrets as a service” solutions
* It should be stored securely
* It should be random, not guessable
* It should be a String
<br/>
<br/>


## Document the following Vocabulary Terms

encryption : It is the method by which information is converted into secret code that hides the information’s true meaning.

token : It is a piece of data that has no meaning or use on its own, but combined with the correct tokenization system, becomes a vital player in securing your application.

bearer : authentication (also called token authentication) is an HTTP authentication scheme that involves security tokens called bearer tokens.

secret : a string that used to encrypt the token when we create it and identify it when its come back to our server. JSON Web Token: It is a standard used to create access tokens for an application.

JSON Web Token : is an Internet proposed standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims.
<br/>
<br/>


## Preview

Which 3 things had you heard about previously and now have better clarity on?

- bearer authorization use in real life.



Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
implement or see how it works?

- learning about fixing bugs.

## RBAC
is the idea of assigning system access to users based on their role in an organization. It’s important to remember that not every employee needs a starring role.

It’s nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs.

- Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations.
<br/>
<br/>


## Benefits of RBAC:
With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.
<br/>
<br/>


## 5 steps to RBAC:
1. Inventory your systems: Figure out what resources you have for which you need to control access, if you don’t already have them listed. Examples would include an email system, customer database, contact management system, major folders on a file server, etc.

2. Analyze your workforce and create roles: You need to group your workforce members into roles with common access needs. Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible.

3. Assign people to roles: Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly.

4. Never make one-off changes: Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary.

5. Audit: Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role.


<br/>
<br/>

## References:
1. [RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
2. [5 steps to RBAC](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html)
3. [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)