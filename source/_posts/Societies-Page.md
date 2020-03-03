---
title: Societies Page
date: 2020-03-03 17:17:29
tags:
---

# Societies

## Dedicated page

The societies page is now seperate from the user page, for a more aesthetically pleasing user interface and to compartmentalize the associated code.

## Invite links

Invite links are generated using an MD5 substring to hide the society IDs and to create a unique code incorporating the expiry date. Invite links are stored on the database and contain the expiry, uses and societyId. 
When a user visits an invite link, their societies are updated to include the society they are joing - if the invite code is valid.

### Invite expiry dates

Society managers can choose to have an expiry on their invite links to prevent people from finding and using their invite codes in the future. 

If a society no longer exists, all invite codes pointing to it will no longer work.

## Leaving societies

Leaving a society simply removes it from your array of societies on the database, and updates the user interface.

## Removing societies

Removing societies you manage deletes them from the database and all of their associated invite links.


# Demonstration

In this video I demonstrate adding a society, leaving, removing and using invite links.

{% owl youtube 6ZOwRk02nDs %}