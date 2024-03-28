# Perform Bulk Microsoft Entra ID Operations in the Portal

**There are 3 objectives with this lab:**
* Bulk Create Users
* Bulk Delete Users
* Bulk Add Group Members


## Bulk Create Users

Alright so first things first, lets navigate to the Entra ID section of the portal

![Image](EntraID1.png)

Once I was in Entra ID, I found the `Users` blade on the left side. 

![Image](EntraID2.png)

Creating a user is pretty straightforward. I clicked on `New User` at the top of the page and put in the name for my users. We also have to give them a password and Azure conveniently will generate a password for you. 

![Image](EntraID3.png)

![Image](EntraID4.png)

We had to create two users so I created Ayanna Will and Edward Von <3. That completes the first objective.

![Image](EntraID5.png)

## Bulk Delete Users

For the next objective, we were tasked with modifying a user's properties and resetting their password. So I clicked on Ayanna Will's profile, clicked `Edit Properties` and changed her job description. 

![Image](EntraID6.png)

![Image](EntraID7.png)

After I saved the changes, I clicked on `Reset Password` at the top of page in order to reset her password. A pop up on the right side of the page will appear displaying the new temporary password.

![Image](EntraID8.png)

Objective completed!

## Bulk Add Group Members

The next objective is to revoke access to a user. I went to Edward Von's profile and then at the top of the page, I clicked `Revoke sessions` which will then log them out of their account. 

![Image](EntraID9.png)

That pretty much completes that revocation process. There's another step when you can disable the account I believe but not delete it. For now, the revoke sessions is enough. 

On to the last objective.


## Personal Notes

This was an easy lab and it only took 10 minutes. This is one of those things that may just be easier to finish in the Portal instead of automating it. 
