# SoundMonk

SoundMonk is a simple but useful music application that lets users store their song online and play them via the app.

![Albums](https://github.com/bkaankuguoglu/SoundMonk/tree/master/media/albums.png "Albums")

![Album Detail](https://github.com/bkaankuguoglu/SoundMonk/tree/master/media/detail.png "Album Detail")



## Getting Started

Assuming that you have already installed all the prerequisites, you can run the application right away after you clone this repo. For those who use PyCharm it is just as easy as clicking the run button; while those who prefer to use Django on different IDEs may use the following commands on the terminal:

```
 $ cd <project_directory>
 $ python manage.py runserver 8000
```

This will run the server as well as your app on the local server. The number 8000 is just the port number and it can be chosen arbitrarily. Now you should be able to see your app running on [your localhost](127.0.0.1:8000/music)

SoundMonk is going to ask your user information, even though you haven't created any account yet. You may login using the credentials for the admin:

- username: admin
- password: SoundMonk

However, you might want to create your own account as well by simply following the guidelines in the application.

Here's one simple trick if you wish to change the password for any user, including the admin:

```
 $ python manage.py changepassword <username>
```

Also, you may run into some error if you're already running an application on the same port of your localhost. One way to solve this problem is:

```
$ sudo lsof -t -i tcp:8000 | xargs kill -9
```

This might seem quite odd to you, but hey, it works!


### Prerequisites

- Django 1.9.4 (Required)
- PyCharm (Not required but highly recommended)
- Bootstrap (If you're willing to add more funky stuff on the frontend)

### Installing

#### Django

The latest version of Django framework can be installed by simply following [the official documentation](https://docs.djangoproject.com/en/1.10/topics/install/). Super easy.

#### PyCharm

This is one of my favorite IDEs and I highly recommend you to download it from [this link](https://www.jetbrains.com/pycharm/download/#section=mac) and start doing some fun stuff with it. Yet again, if you feel more comfortable using other IDEs, do not feel obliged to do this step. As mentioned, this is just a friendly suggestion.

#### Bootstrap

Another optional step. If you're not familiar with this framework, you might just want to skip this step as the main frontend of the application is already built. However, if you'd like to give it a try, you can start by following [this brief tutorial](https://tutorial.djangogirls.org/en/css/)


## Deployment

Well, we all know this documentation was going to come to this point. If you ever want to make this application live, here is [a super awesome tutorial](https://tutorial.djangogirls.org/en/deploy/) about deployment using Django Framework.


## Version

* **v1.0.0**

## Authors

* **Berk Kaan Kuguoglu**


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


## Acknowledgments

* Special thanks to [buckyroberts](https://github.com/buckyroberts) who has made this application possible for me to develop by following [his tutorial](https://www.youtube.com/watch?v=qgGIqRFvFFk).
