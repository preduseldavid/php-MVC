### Live Page running this repository
http://139.59.153.154

# PHP MVC (Model, View, Controller)

Just a simple user authentication solution inside a super-simple framework skeleton that works out-of-the-box
(and comes with an auto-installer), using the future-proof official bcrypt password hashing/salting implementation of 
PHP 5.5+, plus some nice features that will speed up the time from idea to first usable prototype application 
dramatically. Nothing more. This project has its focus on hardcore simplicity. Everything is as simple as possible, 
made for smaller projects, typical agency work and quick drafts. If you want to build massive corporate 
applications with all the features modern frameworks have, then have a look at [Laravel](http://laravel.com), 
[Symfony](http://symfony.com) or [Yii](http://www.yiiframework.com), but if you just want to quickly create something
that just works, then this script might be interesting for you.


### Features <a name="features"></a>
* built with the official PHP password hashing functions, fitting the most modern password hashing/salting web standards
* proper security features, like CSRF blocking (via form tokens), encryption of cookie contents etc.
* users can register, login, logout (with username, email, password)
* password-forget / reset
* remember-me (login via cookie)
* account verification via mail
* captcha
* failed-login-throttling
* user profiles
* account upgrade / downgrade
* simple user types (type 1, type 2, admin)
* supports local avatars and remote Gravatars
* supports native mail and SMTP sending (via PHPMailer and other tools)
* uses PDO for database access for sure, has nice DatabaseFactory (in case your project goes big) 
* uses URL rewriting ("beautiful URLs")
* proper split of application and public files (requests only go into /public)
* uses Composer to load external dependencies (PHPMailer, Captcha-Generator, etc.) for sure
* fits PSR-0/1/2/4 coding guidelines
* uses [Post-Redirect-Get pattern](https://en.wikipedia.org/wiki/Post/Redirect/Get) for nice application flow
* masses of comments


### Requirements <a name="requirements"></a>

Make sure you know the basics of object-oriented programming and MVC, are able to use the command line and have
used Composer before.

* **PHP 5.5+**
* **MySQL 5** database (better use versions 5.5+ as very old versions have a [PDO injection bug](http://stackoverflow.com/q/134099/1114320)
* installed PHP extensions: pdo, gd, openssl (the install guideline shows how to do)
* installed tools on your server: git, curl, composer (the install guideline shows how to do)
* for professional mail sending: an SMTP account (I use [SMTP2GO](http://www.smtp2go.com/?s=devmetal))
* activated mod_rewrite on your server (the install guideline shows how to do)
