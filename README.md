# Notipy
This Python code looks for releases from the list of artists via spotipy library and sends e-mail notifications on the day of release, the next day (in case you forget to check it out), 3 days later (so that you REALLY don't forget) and 7 days later (so that you can have a weekiversaty party celebrating the new release from your favourite artist). Ok, more about that - I set up reminders that way because even though I love the convenience and the free-ism of the free tier of PythonAnywhere it comes with the downside of a kind of restricted access to the Gmail SMTP server - it works in the free tier but they add its IP's manually so it doesn't work for a day or two when Gmail SMTP changes their IP's hence this 'aggressive' reminding schedule.


The key 'album,single' for album_type grabs ALL types of releases from an artist. I chose so because I don't want to miss EP's and singles. Change it to 'album' if you want to get notifications about albums only.
You must create a spotify developer account (it takes like 5 minutes) to obtain and enter your credentials here.
This code uses Gmail SMTP to send e-mail notifications because it's the most convenient way to send e-mails via Python code for free. If you're not familiar with this solution - you must set up 2FA for your Gmail account and generate a 16 character password to give access to your account from other apps in security settings of your account. 
Run this code on a platform of your choosing as a daily task (the free tier of PythonAnywhere has one scheduled task so it works for me best).
Enjoy!
