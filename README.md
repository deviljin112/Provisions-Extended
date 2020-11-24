# Provisions

Provisioning is derived from providing and supplying something. For example, Provisioning for food or water. In Vagrant provides our Virtual Machine with instructions, variables, files, and folders.
</br>
This means we can set up a machine to a specific state when initialized.

## Upload a single file to VM

`vagrant upload <path/to/file>`

This uploads single file to the machine.

## New project environment

When given a new project, you want to ask a few questions to help you get going. For example

- What language is it in?
- Is there a framwork to install? (Rails, Flask, Django, Wordpress)
- Any specific packages? If so, is there a list? (Gemfile, Requirements.txt)
- Any tests?

### What language is it in

Code is in JS and orthers. There are some tests in ruby and rpsec.

### Is there a framework to install

No. Only testing framework `rspec`.

### Any specific packages

Yes, wit the environment file you have a Gemfile with dependencies.

### Any tests

Yes, there are 2 tests. Integration test to run outside the machine with `rake spec`. There is also some unit testing in JS, inside the machine.

## Gem and builder vs PIP and Packages

- Gems are packages in ruby or dependencies
- Bundler is ruby's package manager
- Gemfile keeps a list of dependencies to be installed
- To install gems from the Gemfile, you run:
  - `bundle install`

## Ruby's testing framework

rspec nees to be installed

## JS Package manager

npm packages (node package manager)
</br>
After version 6, comes pre-loaded with NPM.

## Ubuntu package manager

apt-get (Mostly depreciated)
apt (preferred)

## Installing Test

1. Locate folder with Gemfile
2. Run `bundle`
3. Ensure Rakefile is there
4. Run `rake spec`
