# Rails 5 Blog v1.0

## Installation:
```
git clone https://github.com/ravuthz/rails_5_blog.git blog_name

cd blog_name

bundle install
```


#### Installed Plugins:

##### Install Haml (template engine)
```
gem 'haml-rails'
```

##### Install Boostrap Generator (scaffold generator template with bootstrap)
```
gem 'bootstrap-generators', '~> 3.3.4'

rails generate bootstrap:install --template-engine=haml
rails generate bootstrap:install --stylesheet-engine=scss

rails generate bootstrap:install -e=haml -se=scss
```

##### Change: app/assets/stylesheets/application.css
```
 *= require bootstrap-generators.scss
```

##### Install Boostrap Form helper (bootstrap_form_for)
```
gem 'bootstrap_form'
```

##### Change: app/assets/stylesheets/application.css
```
 *= require rails_bootstrap_forms
```


##### Install Friendly id (Pretty url with slug)
```
gem 'friendly_id', '~> 5.1'

rails generate friendly_id
rails db:migrate
```

##### Install Devise (User authentication)
```
gem 'devise', '~> 4.2'

rails generate devise:install
rails generate controller pages home about contact
rails generate devise User
rails db:migrate
```

#### *References*:
* https://github.com/decioferreira/bootstrap-generators
* https://github.com/bootstrap-ruby/rails-bootstrap-forms
* https://github.com/norman/friendly_id
* https://github.com/plataformatec/devise
