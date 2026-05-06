# Jekyll Local Development Setup

This project is designed to run with GitHub Pages locally using Jekyll.

## Prerequisites

Make sure you have the following installed:

* Ruby
* Bundler

Install Bundler if needed:

```bash
gem install bundler
```

---

## Setup

Install the required gems using the provided `Gemfile`:

```bash
bundle install
```

The `Gemfile` should include:

```ruby
gem "github-pages", group: :jekyll_plugins
```

This ensures your local environment matches GitHub Pages, including themes and supported plugins.

---

## Running the site locally

This project uses the `/docs` folder as the site source.

Start the local server with:

```bash
bundle exec jekyll serve --source docs
```

Then open your browser and go to:

```
http://localhost:4000
```

---

## Notes

* If changes don’t appear, try clearing the build cache:

```bash
rm -rf _site .jekyll-cache
bundle exec jekyll serve --source docs
```

* Always use `bundle exec` to ensure the correct gem versions are used.
