# Helpers

## Readability

* [annotate\_models](https://github.com/ctran/annotate_models) - Automatically generates attributes as comments at the top of files to see what attributes are in models, fixture files, specs, factories, and more. Example:

  ```ruby
  # == Schema Info
  #
  # Table name: line_items
  #
  #  id                  :integer(11)    not null, primary key
  #  quantity            :integer(11)    not null
  #  product_id          :integer(11)    not null
  #  unit_price          :float
  #  order_id            :integer(11)
  #

   class LineItem < ActiveRecord::Base
     belongs_to :product
  # ...
  ```

## Migrations

* [strong\_migrations](https://github.com/ankane/strong_migrations) - Detect potentially dangerous migrations and prevent them from running by default, along with instructions on safer ways to do what you want.
* [native\_enum](https://github.com/iangreenleaf/native_enum) and [activerecord-postgres\_enum](https://github.com/bibendi/activerecord-postgres_enum) for backing Rails enums \(which are application-only\) by database enums, so people looking at the database can actually understand what all those integer values actually mean.

## View Helpers

Rails already provides a ton of view helpers \(e.g. `number_to_currency`\), they're listed [here](https://guides.rubyonrails.org/action_view_overview.html#overview-of-helpers-provided-by-action-view).

