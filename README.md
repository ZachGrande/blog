# Blog

Welcome to my Blog application, used as a general introduction to Rails 7!

## Installation

To set up the project, follow these steps:

1. **Clone the repository:**

```
git clone git@github.com:ZachGrande/blog.git
git cd blog
```

2. **Install dependencies:**

```
bundle install
```

## Database Setup

Make sure to set up the database before running the application:

1. **Create the database:**

```
rails db:create
```

2. **Run migrations:**

```
rails db:migrate
```

3. **Seed the database (if needed):**

```
rails db:seed
```

## Running the Application

To start the Rails server, use the following command:

```
rails server
```

Access the application by visiting http://localhost:3000 in your web browser.

## Generating Models, Controllers, and More

### Generating a Model

To create a new model, use the `rails generate` command followed by the model name and its attributes:

```
rails generate model ModelName attribute1:type attribute2:type

# example:
    rails generate model Article title:string body:text
# output:
    invoke  active_record
    create    db/migrate/20231116184422_create_articles.rb
    create    app/models/article.rb
    invoke    test_unit
    create      test/models/article_test.rb
    create      test/fixtures/articles.yml
```

### Generating a Controller

To generate a new controller, use:

```
rails generate controller ControllerName action1 action2

# example:
    rails generate controller Articles index --skip-routes
# output:
    create  app/controllers/articles_controller.rb
    invoke  erb
    create    app/views/articles
    create    app/views/articles/index.html.erb
    invoke  test_unit
    create    test/controllers/articles_controller_test.rb
    invoke  helper
    create    app/helpers/articles_helper.rb
    invoke    test_unit
```

### Running Tests

To run tests, use:

```
rails test
```

## Additional Notes

- **Gemfile:** Check and update the Gemfile for any additional gems needed.
- **Routes:** Application routes are defined in `config/routes.rb`.
- **Views:** Views for controllers are located in the `app/views` directory.
