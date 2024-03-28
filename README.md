# Perform Bulk Microsoft Entra ID Operations in the Portal

**There are 3 objectives with this lab:**
* Bulk Create Users
* Bulk Delete Users
* Bulk Add Group Members


## Bulk Create Users

The first objective requires us to create 3 users using the `Bulk` option in Entra ID. So first things first, lets navigate to the Entra ID section of the portal

![Image](EntraIDBulk1.png)

Next, we'll look on the left to the Users blade. Lets click that to get one step closer to our Bulk operations.  

![Image](EntraIDBulk2.png)

Once here, I looked at the top of the screen and saw the `Bulk operations` tab where we're presented with multiple options: Create, Invite, and Delete. We're going to choose the `create` option. 

![Image](EntraIDBulk3.png)

Once you're pressed `Bulk create`, yoou'll be given an Excel file where you need to add your user information into. 

![Image](EntraIDBulk4.png)

Make sure you give each user a first and last name, an email address with the proper domain (I mistakenly gave everyone `@contoso.com`), and a temporary password. If you don't give the information precisely, the Azure portal won't accept the file (as we'll see shortly). 

![Image](EntraIDBulk5.png)

When you're done, save it and upload it to the Azure. It will say `File uploaded successfully` and then Azure will deploy it. 

I ended up getting a failed deploy and it was saying I didn't have the proper domain for the email addresses. 

![Image](EntraIDBulk6.png)

I went back into the Entra ID section and looked at the users. I noticed the domain the other users had (`@radlabs2p.onmiscrosoft.com`) so I knew I had to change the domain for the users I created. 

![Image](EntraIDBulk7.png)

I went back and changed the domain name for the three users. 

![Image](EntraIDBulk8.png)

Once I reuploaded the updated Excel spreadsheet, I received a `Succeeded` notification.

![Image](EntraIDBulk9.png)

Afterwards, I checked the users to see if they were populated in the table and they were there!

![Image](EntraIDBulk10.png)

Objective completed. On to the deletion objective.

## Bulk Delete Users

For the next objective, we were tasked with bulk deleting users. Similar to the bulk create, we navigated back to users and `Bulk operations`. We then downloaded the `Bulk delete` spreadsheet.

![Image](EntraIDBulk11.png)

I put the email address of the three users I created into the spreadsheet and then uploaded it to Azure. You should also receive a `Succeeded` message here as well. 

![Image](EntraIDBulk12.png)

After the operation was deployed, you can check the `Users` tab to see if the users were deleted. In my case, the users were no longer in the table. 

![Image](EntraIDBulk13.png)

Objective completed! Last but not least, the final objective. 

## Bulk Add Group Members

The next objective is to revoke access to a user. I went to Edward Von's profile and then at the top of the page, I clicked `Revoke sessions` which will then log them out of their account. 

![Image](EntraID9.png)

That pretty much completes that revocation process. There's another step when you can disable the account I believe but not delete it. For now, the revoke sessions is enough. 

On to the last objective.


## Personal Notes

This was an easy lab and it only took 10 minutes. This is one of those things that may just be easier to finish in the Portal instead of automating it. 
