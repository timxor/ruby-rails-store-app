# ruby-rails-store-app
ruby-rails-store-app

```
cd store
bin/rails server
```

To see your Rails application, open http://localhost:3000 in your browser.


Tutorial from ruby on rails getting started
https://guides.rubyonrails.org/getting_started.html



## ruby notes

------------------------------------------


ruby notes

ruby on rail notes

textmate editor


install with rbenv - ruby version manager

brew install rbenv ruby-build
brew install rust libyaml gmp openssl@3 readline



initialize rbenv in shell


# rbenv - ruby version manager
eval "$(rbenv init -)"
export LDFLAGS="-L$(brew --prefix)/lib"
export CPPFLAGS="-I$(brew --prefix)/include"
export RUBY_CONFIGURE_OPTS="--with-openssl-dir=$(brew --prefix openssl@3)"

source ~/.zshrc


verify works

rbenv --version


install latest stable ruby version - 3.4.4

RUBY_CONFIGURE_OPTS="$RUBY_CONFIGURE_OPTS --disable-yjit" rbenv install 3.4.4

rbenv install 3.4.4
rbenv global 3.4.4






install bundler and common tools

gem install bundler


gem install pry        # Powerful alternative to IRB for debugging
gem install rake       # Build automation tool (like Make for Ruby)
gem install rubocop    # Linter and style checker
gem install rspec      # Popular testing framework
gem install solargraph # Language server (LSP) for Ruby code intelligence



gem install rails      # Full-stack web framework
gem install sinatra    # Lightweight DSL for web apps
gem install puma       # Fast concurrent web server for Rack/Rails
gem install foreman    # Manage Procfile-based apps (used in dev environments)

gem install irbtools   # Enhances IRB with a better dev experience
gem install dotenv     # Load `.env` files for local config
gem install yard       # Documentation generator like Javadoc for Ruby


echo 'gem: --no-document' >> ~/.gemrc




ruby -v
gem -v
bundler -v
rbenv versions





Let me know if you're planning to use:
* Rails, Sinatra, or Jekyll?
* Ruby for scripting, devops, or CLI tooling?
* A specific IDE (e.g., VS Code, RubyMine)?
That will refine which tools are worth adding.




# create a new rails store app

ruby-rails-store-app - repo
https://github.com/timxor/ruby-rails-store-app


git clone https://github.com/timxor/ruby-rails-store-app.git

rails --version


rails new store




```
cd store
bin/rails server
```

To see your Rails application, open http://localhost:3000 in your browser.


Tutorial from ruby on rails getting started
https://guides.rubyonrails.org/getting_started.html




-----------------------------------------------------------------
sqlite
Our application is using SQLite which is the default for Rails.
-----------------------------------------------------------------






creating a database model
https://guides.rubyonrails.org/getting_started.html

```
bin/rails generate model Product name:string
```

running migrations

```
bin/rails db:migrate
```


rails console

```
bin/rails console
Rails.version
```
