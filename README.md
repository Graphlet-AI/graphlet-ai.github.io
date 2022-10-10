# Graphlet AI

Graphlet AI an artificial intelligence platform for using knowledge graphs to explain the decisions of machine learning models in terms of their business logic.

This is a website for **Graphlet AI** built on Jekyll

## Installation

To run this project locally,

- Install Ruby

On Mac OS X:

```bash
brew install ruby
```

Add this to your `~/.zshrc`:

```bash
# Make brew Ruby default
echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc

# Brew says: For compilers to find ruby you may need to set
export LDFLAGS="-L/usr/local/opt/ruby/lib"
export CPPFLAGS="-I/usr/local/opt/ruby/include"
export PATH="/usr/local/opt/ruby/bin:$PATH"
```

- Clone this repository
- Install the dependencies

```bash
bundle install
```

- Go into /graphlet_ai and run the command

```bash
bundle exec jekyll serve
```

The site will serve on [localhost:4000](http://localhost:4000)

- Note: in _config.yaml, baseurl should be empty ""

## Usage

Click here to open this website hosted on Github Pages : [insert URL]
