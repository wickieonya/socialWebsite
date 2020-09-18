# Social Website
A social application built with django to allow users share images that they find on the Internet.

## Main features 
1. An authentication system for users to register, log in, edit profiles, and change or reset passwords.
2. A follow system to allow users to follow each other on the website.
3. A functionality to display shared images and implement a bookmarklet for users to share images from any website.
4. An activity stream that allows users to see the content uploaded by the people that they follow.

### Installation 
To install the app requirements.

`pip install -r requirements.txt`

#### Quirks
django models 
- use the `get_user_model()` method to retrieve the user
- use the `AUTH_USER_MODEL` setting to refer to it when defining a relationship with the user model, instead of referring to the `auth` user model directly.

#### Running Dev Server in HTTPS
Run the following command
`python manage.py runserver_plus --cert-file cert.crt`

