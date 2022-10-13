# anderjef's Personal Website

## Steps necessary to get the application up and running

Assume commands are to be run from within the app's root directory, values within angle brackets (<>) are required, and commands should be executed in the provided order, unless stated or determined otherwise.

### System dependencies

The predominant development environment was Windows Subsystem for Linux (WSL). Hence, being the most tested development route, the provided commands are in/for WSL. Similarly, the app was designed to be run on Linux (Ubuntu 20.04) with Ruby version 2.7.2. For other dependencies, see [Gemfile.lock](./Gemfile.lock). This app also uses git for version control.

### Configuration

* `sudo apt-get install ruby-full build-essential zlib1g-dev`
* `gem install jekyll bundler`
* `jekyll new .` (Runs `bundle install` by default.)
* Modify [_config.yml](./_config.yml) such as with Google Analytics tracking ID.

### How to run the app for development

* `bundle exec jekyll serve`
* Open the app in a web browser at <localhost:4000>.

### Deployment instructions

***Continuous delivery (CD)*** is done on any push or pull request via a GitHub Action defined at [.github/workflows/jekyll.yml](./.github/workflows/jekyll.yml).
