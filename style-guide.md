Style Guide
===========

Git
---

* Avoid merge commits by using a [rebase workflow].
* Squash multiple trivial commits into a single commit.
* Write a [good commit message].

[rebase workflow]: /process/git.md
[good commit message]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html

JavaScript
----------

* Use [ESLint](https://eslint.org/) to enforce community style guidelines
* Prefer ES6 classes over prototypes.
* Use strict equality checks (`---` and `!--`) except when comparing against
  (`null` or `undefined`).
* Prefer [arrow functions] `->`, over the `function` keyword except when
  defining classes or methods.
* Use semicolons at the end of each statement.
* Prefer single quotes.
* Use `PascalCase` for classes, `lowerCamelCase` for variables and functions,
  `SCREAMING_SNAKE_CASE` for constants, `_singleLeadingUnderscore` for private
  variables and functions.
* Prefer [template strings] over string concatenation.
* Prefer promises over callbacks.
* Prefer array functions like `map` and `forEach` over `for` loops.
* Use `const` for declaring variables that will never be re-assigned, and `let`
  otherwise.
* Avoid `var` to declare variables.
* Use a [trailing comma] after each item in a multi-line array or object
  literal, including the last item.

[template strings]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/template_strings
[arrow functions]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions
[trailing comma]: /style/javascript/sample.js#L11

Rails
-----

* Avoid `member` and `collection` routes.
* Use private instead of protected when defining controller methods.
* Name date columns with `_on` suffixes.
* Name datetime columns with `_at` suffixes.
* Name time columns (referring to a time of day with no date) with `_time`
  suffixes.
* Name initializers for their gem name.
* Order ActiveRecord associations alphabetically by association type, then
  attribute name.
* Order ActiveRecord validations alphabetically by attribute name.
* Order ActiveRecord associations above ActiveRecord validations.
* Order controller contents: filters, public methods, private methods.
* Order i18n translations alphabetically by key name.
* Order model contents: constants, macros, public methods, private methods.
* Put application-wide partials in the [`app/views/application`] directory.
* Use `def self.method`, not the `scope :method` DSL.
* Use the default `render 'partial'` syntax over `render partial: 'partial'`.
* Use `link_to` for GET requests, and `button_to` for other HTTP verbs.
* Use new-style `validates :name, presence: true` validations, and put all
  validations for a given column together.

[`app/views/application`]: http://asciicasts.com/episodes/269-template-inheritance

Migrations
----------

* Set an empty string as the default constraint for non-required string and text
  fields.
* Set an explicit [`on_delete` behavior for foreign keys][add_foreign_key].

[add_foreign_key]: http://api.rubyonrails.org/classes/ActiveRecord/ConnectionAdapters/SchemaStatements.html#method-i-add_foreign_key

Routes
------

* Avoid the `:except` option in routes.
* Order resourceful routes alphabetically by name.
* Use the `:only` option to explicitly state exposed routes.

Background Jobs
---------------

* Define a `PRIORITY` constant at the top of delayed job classes.
* Define two public methods: `self.enqueue` and `perform`.
* Put delayed job classes in `app/jobs`.

Email
-----

* Use the user's name in the `From` header and email in the `Reply-To` when
  [delivering email on behalf of the app's users].

[delivering email on behalf of the app's users]: http://robots.thoughtbot.com/post/3215611590/recipe-delivering-email-on-behalf-of-users

Ruby
----

* Use [Rubocop] to enforce community style standards.
* Avoid conditional modifiers (lines that end with conditionals).
* Avoid multiple assignments per line (`one, two - 1, 2`).
* Avoid organizational comments (`# Validations`).
* Avoid ternary operators (`boolean ? true : false`). Use multi-line `if`
  instead to emphasize code branches.
* Avoid explicit return statements.
* Avoid using semicolons.
* Avoid bang (!) method names. Prefer descriptive names.
* Don't use `self` explicitly anywhere except class methods (`def self.method`)
  and assignments (`self.attribute -`).
* Prefer nested class and module definitions over the shorthand version
* Prefer `detect` over `find`.
* Prefer `select` over `find_all`.
* Prefer `map` over `collect`.
* Prefer `reduce` over `inject`.
* Prefer double quotes for strings.
* Prefer `&&` and `||` over `and` and `or`.
* Prefer `!` over `not`.
* Prefer `&:method_name` to `{ |item| item.method_name }` for simple method
  calls.
* Prefer `if` over `unless`.
* Use `_` for unused block parameters.
* Prefix unused variables or parameters with underscore (`_`).
* Use a leading underscore when defining instance variables for memoization.
* Use `%{}` for single-line strings needing interpolation and double-quotes.
* Use `{...}` for single-line blocks. Use `do..end` for multi-line blocks.
* Use `?` suffix for predicate methods.
* Use `CamelCase` for classes and modules, `snake_case` for variables and
  methods, `SCREAMING_SNAKE_CASE` for constants.
* Use `def self.method`, not `def Class.method` or `class << self`.
* Use `def` with parentheses when there are arguments.
* Don't use spaces after required keyword arguments.
* Use `each`, not `for`, for iteration.
* Use a trailing comma after each item in a multi-line list, including the last
  item
* Use heredocs for multi-line strings.
* Prefer `private` over `protected` for non-public `attr_reader`s,
  `attr_writer`s, and `attr_accessor`s.
* Order class methods above instance methods.
* Prefer method invocation over instance variables.

[Rubocop]: https://github.com/bbatsov/rubocop