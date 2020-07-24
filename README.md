# A SIMPLE FORM BUILT WITH RAILS

<br />
<p align="center">
  <a href="https://github.com/Jmagero/re-former">
    <img src="app/assets/images/microverse-logo.webp" alt="Logo" width="100" height="100">
  </a>

  <h3 align="center">Linter</h3>

  <p align="center">
    This is a collaborative project as part of the Microverse Ruby curriculum
    <br />
    <a href="https://github.com/Jmagero/re-former"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Jmagero/linter/issues">Report Bug</a>
    ·
    <a href="https://github.com/Jmagero/linter/issues">Request Feature</a>
  </p>
</p>


* Ruby version 2.7.1

## Table of Contents

* [About](#about)
* [Usage](#usage)
* [Development](#development)
  * [Built With](#built-with)
* [Author](#author)
* [Show Support](#show-your-support)
* [Acknowledgements](#acknowledgements)


## About

The aim of this project was to learn the basics about the multiple ways one can build a form in Rails. Such as by sending parameters to a controller so that it can build an instance of a model with those parameters.

We started the project by setting up the backend. 

* created and migrated a User model with `:username`, `:email` and `:password`.
* added validations for presence to each field in the model.
* created the `:users` resource in the routes file so that requests could have somewhere to go. We used the `:only` option to specify just the `:new` and `:create` actions.
* built a UsersController via the `$ rails generate controller Users` generator, rather than manually.
* wrote methods for `#new`, `#create`, `#edit` and `#update` in our UsersController.
* created the view for our `#new` method inside of `app/views/users/new.html.erb`.
* fired up a rails server every now and then to make sure everything worked.
* cheked our work by visiting `http://localhost:3000/users/new`.

After that, we moved on to creating our forms.

* built a form for creating a new user. 
* actually built three forms to create a new user.
* created a plain HTML form, then we created a form_tag type of form, using some of the Rails functionalities they have for form. Finally, we built a form_for, thus using the full functionalities Rails has in place for their forms.

The final action we had to account for in this project was the Edit button. For that we did the following:

* updated the routes and controller to handle editing and existing user.
* created the Edit view by building a similar form to what we had in the New view, using fomr_for.

The very last thing we did in this app was to create an error message to be displayed everytime the user failed to have all of the fields validated.


## Usage

### Installing Ruby

You shoudl have Ruby installed in your computer to run this project.

If you're not sure wether or not you have Ruby, type the following in your command line:<br>
`ruby -v`
That should return the version of Ruby that's running on your computer. 

If you need to install Ruby, follow the instructions in this [webpage](https://www.ruby-lang.org/en/documentation/installation/).

### Installing Rails

You should also have Rails installed in your computer.

Follow the instructions in this tutorial to install Rails [webpage](https://www.theodinproject.com/courses/ruby-on-rails/lessons/your-first-rails-application-ruby-on-rails)

### Clone the repo

Go ahead and clone the repo.

## Development

After cloning the repo, you should fire up a server. Open a command line terminal and paste the following command:

`rails s`

After that, open your browser and type the following in your address bar: 

`http://localhost:3000`

That will take you to the main form where you can create a new user. Fill out all the fields. If they pass validation, the form should be emptied out. Otherwise, you should get an error message on top of your form.


### Built With
* Ruby
* Rails
* Git
* Rubocop

## Authors

👤 **Jocylin Magero** 

- Twitter: [@magero_jocyline](https://twitter.com/magero_jocyline) 
- Github: [Jmagero](https://github.com/Jmagero)
- LinkedIn: [jocyline-magero](https://www.linkedin.com/in/jocyline-magero-9592b0145/)

👤 **Guilherme Recordon** 

- Twitter: [@guirecordon](https://twitter.com/RecordonG) 
- Github: [guirecordon](https://github.com/guirecordon)
- LinkedIn: [GuilhermeRecordon](www.linkedin.com/in/gui-recordon-marketingmba/)

## Show your support

Give a ⭐️ if you like this project!

## Acknowledgements

The Odin Project is awesome!
