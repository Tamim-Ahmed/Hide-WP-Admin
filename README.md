# Hide-WP-Admin

The code below hides the user with username XXXXXX from the list of users on your client’s WordPress site (Users >> All Users). Of course, you need to change both instances of XXXXXX to the username of your choosing.
Copy this code into your theme’s functions.php file. You can find your theme’s functions.php file in folder /wp-content/themes/your(sub)theme/ on your site’s server.

{CODE = Hide-administrator.php}

The code snippet still shows your account when you are logged in, but hides it from other users. You can check by creating other accounts.

# Change-the-number-of-administrators-on-the-site

The code above hides the selected admin account itself from the list of users. However, the number of users (All) and the number of admins (administrator) in the left corner above the user list will still include this account. This might tick off certain site owners.

Luckily, it’s not too difficult to solve this. Though I’ve seen numerous solutions that just got rid of the counts altogether, this code takes both numbers and subtract 1. Place this code in the functions.php below the code snippet above.

{CODE = Remove-admin-roles-number.php}
