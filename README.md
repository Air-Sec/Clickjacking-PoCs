This is a Clickjacking PoC that demonstrates steps to a user as a fake advert to get 75% off by following instructions.
One of the instructions contains a hidden draggable HTML element with the email oliver.wen@airit.co.uk, that can be used to replace the existing user's email address.

The purpose of this is to allow an attacker bypass CSRF protections and use the new email address to compromise the victim user's account by requesting a password reset that gets sent to the attacker.
Once the attacker resets the password, he now has full control of the user's account and has at the same time prevented the target user from logging into their own account.
