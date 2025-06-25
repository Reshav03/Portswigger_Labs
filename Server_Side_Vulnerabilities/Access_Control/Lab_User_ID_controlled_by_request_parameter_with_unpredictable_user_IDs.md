<H3>This lab has a horizontal privilege escalation vulnerability on the user account page, but identifies users with GUIDs.

To solve the lab, find the GUID for `carlos`, then submit his API key as the solution.
You can log in to your own account using the following credentials: `wiener:peter`</H3>

Lets first login by our own credentials

![Step1]()

We get this information

After login in check the posts made by carlos
Then click on carlos's username and see the changes in the URL

![Step2]()

Get his user-id and go to your login page and input his user ID in the URL

![Step3]()

And now you get his API Key.

Submit the API Key and Lab is solved
