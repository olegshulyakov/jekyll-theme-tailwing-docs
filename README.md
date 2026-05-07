# Jekyll Theme Tailwind Docs

A Jekyll theme in [Tailwind Docs](https://tailwindcss.com/docs) styles main content column.

## Usage

To use the Tailwind Docs theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    theme: jekyll-theme-tailwing-docs
    ```

2. Add this line to your site's `Gemfile`:

    ```ruby
    gem "jekyll-theme-tailwing-docs"
    ```

3. Execute:

    ```bash
    $ bundle install
    ```

## Customizing

### Configuration variables

This theme will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

*Note: If you'd like to change the theme's Sass variables, you must set new values before the `@import` line in your stylesheet.*

### Layouts

If you'd like to change the theme's HTML layout:

1. For some changes such as a custom `favicon`, you can add custom files in your local `_includes` folder. The files [provided with the theme](https://github.com/olegshulyakov/jekyll-theme-tailwing-docs/tree/master/_includes) provide a starting point and are included by the [original layout template](https://github.com/olegshulyakov/jekyll-theme-tailwing-docs/blob/master/_layouts/default.html).
2. For more extensive changes, [copy the original template](https://github.com/olegshulyakov/jekyll-theme-tailwing-docs/blob/master/_layouts/default.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
3. Create a file called `/_layouts/default.html` in your site
4. Paste the default layout content copied in the first step
5. Customize the layout as you'd like

## Project philosophy

The Tailwind Docs theme is intended to make it quick and easy for users to create beautiful documentation websites. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/olegshulyakov/jekyll-theme-tailwing-docs. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the Contributor Covenant code of conduct.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

## License

The theme is available as open source under the terms of the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
