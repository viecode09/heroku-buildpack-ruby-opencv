# Heroku buildpack: Ruby with OpenCV

This is a fork of the [Heroku Ruby buildpack](https://github.com/heroku/heroku-buildpack-ruby), that includes OpenCV and CMake for gems like `ruby-opencv` and 'ropencv' and all the fun computer vision tools to work on Heroku.

## Usage

Just set this as your buildpack with the following command:

```sh
heroku config:add BUILDPACK_URL=https://github.com/lilibethdlc/heroku-buildpack-ruby-opencv
```

## Flow

Here's the basic flow of how the buildpack works:

* Installs CMake, unless already installed.
* Installs OpenCV, unless already installed.
* Continues with the [heroku-buildpack-ruby flow](https://github.com/heroku/heroku-buildpack-ruby#flow)
