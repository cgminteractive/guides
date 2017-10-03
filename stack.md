# CGM Tech Stack

## Frameworks and Services

Payment Gateway:

* [Authorize.net API](https://developer.authorize.net/) for payment processing and subscriptions
* [Authorize.net Webhooks](https://developer.authorize.net/api/reference/features/webhooks.html) for failed payment notifications

Application Framework

* [Ruby on Rails](http://guides.rubyonrails.org/) for MVC web application
* [FeathersJS](https://docs.feathersjs.com/) for real-time service layer

Suggested Application gems:

* [Devise](https://github.com/plataformatec/devise) for user authentication
* [Active Admin](https://github.com/activeadmin/activeadmin) for straightforward admin interface building
* [Kaminari](https://github.com/kaminari/kaminari) for elegant pagination for any sort of collection
* [Flutie](https://github.com/thoughtbot/flutie) for `page_title` and `body_class` view
  helpers
* [High Voltage](https://github.com/thoughtbot/high_voltage) for static pages
* [jQuery Rails](https://github.com/rails/jquery-rails) for jQuery
* [Postgres](https://github.com/ged/ruby-pg) for access to the Postgres database
* [Rack Canonical Host](https://github.com/tylerhunt/rack-canonical-host) to
  ensure all requests are served from the same domain
* [Rack Timeout](https://github.com/heroku/rack-timeout) to abort requests that are
  taking too long
* [Simple Form](https://github.com/plataformatec/simple_form) for form markup
  and style
* [Puma](https://github.com/puma/puma) to serve HTTP requests
* [Ransack](https://github.com/activerecord-hackery/ransack) for a simple search API to query your data
* [Select2](https://github.com/argerim/select2-rails) for jQuery Select boxes
* [Sidekiq](http://sidekiq.org/) for background job processing
* [Paperclip](https://github.com/thoughtbot/paperclip) for programmatic file attachments
* [Webpacker](https://github.com/rails/webpacker) for Asset pre-processing and bundling
* [Smarter CSV](https://github.com/tilo/smarter_csv) for CSV loading
* [PDFKit](https://github.com/pdfkit/pdfkit) for using HTML/CSS to gernerate PDFs
* [Delayed Job](https://github.com/collectiveidea/delayed_job) for background processing

Suggested Development gems:

* [Dotenv](https://github.com/bkeepers/dotenv) for loading environment variables
* [Pry Rails](https://github.com/rweng/pry-rails) for interactively exploring
  objects
* [ByeBug](https://github.com/deivid-rodriguez/byebug) for interactively
  debugging behavior
* [Bullet](https://github.com/flyerhzm/bullet) for help to kill N+1 queries and
  unused eager loading
* [Bundler Audit](https://github.com/rubysec/bundler-audit) for scanning the
  Gemfile for insecure dependencies based on published CVEs
* [Spring](https://github.com/rails/spring) for fast Rails actions via
  pre-loading
* [Web Console](https://github.com/rails/web-console) for better debugging via
  in-browser IRB consoles.

Suggested Testing gems:

* [Capybara](https://github.com/jnicklas/capybara) and
  [Capybara WebKit](https://github.com/thoughtbot/capybara-webkit) for
  integration testing
* [Factory Girl](https://github.com/thoughtbot/factory_girl) for test data
* [Formulaic](https://github.com/thoughtbot/formulaic) for integration testing
  HTML forms
* [RSpec](https://github.com/rspec/rspec) for unit testing
* [RSpec Mocks](https://github.com/rspec/rspec-mocks) for stubbing and spying
* [Shoulda Matchers](https://github.com/thoughtbot/shoulda-matchers) for common
  RSpec matchers
* [Timecop](https://github.com/travisjeffery/timecop) for testing time

Yarn Packages:

* [FeathersJS Client](https://github.com/feathersjs/feathers-client) for interfacing with services layer
* [Boostrap](https://www.npmjs.com/package/bootstrap) for front end layout and mobile-first design

Salesforce Integration:

* [Heroku Connect](https://www.heroku.com/connect) for Salesforce data sync

Hosting:

* [Heroku](https://www.heroku.com/)

Transactional Email:

* [Mailgun](https://www.mailgun.com/)
* [Mandrill](https://www.mandrill.com/)
* [SendGrid](https://sendgrid.com/)

Image Storage + CDN:

* [AWS S3 + Cloudfront](https://aws.amazon.com/cloudfront/)

## Tools Needed

macOS tools:

* [Homebrew] for managing operating system libraries.

[Homebrew]: http://brew.sh/

Unix tools:

* [Git] for version control
* [OpenSSL] for Transport Layer Security (TLS)
* [Zsh] as your shell

[Git]: https://git-scm.com/
[OpenSSL]: https://www.openssl.org/
[Zsh]: http://www.zsh.org/

Heroku tools:

* [Heroku CLI] and [Parity] for interacting with the Heroku API

[Heroku CLI]: https://devcenter.heroku.com/articles/heroku-cli
[Parity]: https://github.com/thoughtbot/parity

GitHub tools:

* [Hub] for interacting with the GitHub API

[Hub]: http://hub.github.com/

Image tools:

* [ImageMagick] for cropping and resizing images

Testing tools:

* [Qt 5] for headless JavaScript testing via [Capybara Webkit]

[Qt 5]: http://qt-project.org/
[Capybara Webkit]: https://github.com/thoughtbot/capybara-webkit

Programming languages, package managers, and configuration:

* [ASDF] for managing programming language versions
* [Bundler] for managing Ruby libraries
* [Node.js] and [NPM], for running apps and installing JavaScript packages
* [Ruby] stable for writing general-purpose code
* [Yarn] for managing JavaScript packages

[Bundler]: http://bundler.io/
[ImageMagick]: http://www.imagemagick.org/
[Node.js]: http://nodejs.org/
[NPM]: https://www.npmjs.org/
[ASDF]: https://github.com/asdf-vm/asdf
[Ruby]: https://www.ruby-lang.org/en/
[Yarn]: https://yarnpkg.com/en/

Databases:

* [Postgres] for storing relational data
* [Redis] for storing key-value data

[Postgres]: http://www.postgresql.org/
[Redis]: http://redis.io/
