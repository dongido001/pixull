# Pixull PHP Framework

The Pixull PHP framework was created primarily to be used as a backend framework, though using it for a frontend is quite feasible and easy as well. It is a lighter weight alternative to popular frameworks such as Symfony and Laravel, with a clearer codebase and shallow learning curve.

It comes with many great features built-in to make your life easier so you can spend your time actually building stuff.

Pixull is coded and maintained by Kevin Dion.

### Main Features

* Complete user system including role levels and permissions
* A simple folder structure so your MVC files are very easy to locate
* Regex, auth, and permission-based URL routing
* A dozen helper classes used to do things like alert, mail, redirect, route, sanitize, validate, and more
* Unlimited environment support
* "Demo mode", allowing you to put your app into demo mode and restrict controller activities
* Simple versioning
* User timezone support
* Super easy user permission system
* Object generator to create new object database tables and files on the fly
* PHPMailer used for sending mail

### UI Features

* [Bootstrap](http://getbootstrap.com) + [AdminLTE](https://almsaeedstudio.com) themes for a nice UI
* Full [Datatables](https://datatables.net) integration
* [FontAwesome](http://fontawesome.io) fonts
* [jQuery](http://jquery.com)

# Installation

**Note: the default admin login for Pixull is `admin@example.com`, password `admin123`. Make sure you change this right after installation is complete.**

### 1. Install Pixull

Pixull uses [Composer](https://getcomposer.org/) for installation and dependency management. Open a command prompt in the folder you will be creating a new project folder inside of. Then run `composer create-project kjdion84/pixull new_folder_name`, where `new_folder_name` is the name of the folder that Pixull will be installed into.

### 2. Configure Settings

Go through each file in the `config/` folder and define the constants in each. Pay attention to `environment.php` first, as that file is what is used to define your environments. Make sure you create a new database, and define your database constants in `database.php` before going to the next step.

### 3. Install Database

Run `php cli install database` from the command line. This will create the core Pixull database tables in your new database.

### 4. Create New Objects

Pixull comes with a handy object generator to generate your database table, routes, permissions, menu item, and MVC files for a new object in seconds. Just run `php cli generate "New Object Name"` from the command line, where `New Object Name` is the singular name for the new object. 

If you generate objects this way, Pixull will automatically execute the `composer update` command for the new model and controller files. If you create controller and model files manually, you must make sure you run the `composer update` command afterwards, so that Composer can update the autoloader with the new filenames.

# Documentation & Support

The website is located at [Pixull.com](http://pixull.com). You can [email me](mailto:kjdion84@gmail.com) any time, or visit GitHub to view the [wiki](https://github.com/kjdion84/pixull/wiki) and [issues](https://github.com/kjdion84/pixull/issues).

# Contributions

If you want to help improve the framework, please post post an [issue](https://github.com/kjdion84/pixull/issues). If you want to donate, there is a donation link on the [website](http://pixull.com) as well.

# License

Pixull is completely open-source and licensed under the [MIT License](http://opensource.org/licenses/MIT).