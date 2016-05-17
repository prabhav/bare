# Bare

Naked, but mildly opinionated boilerplate based on Jekyll for [Siteleaf (v2)](http://v2.siteleaf.com/).

##Notes to Self (or whoever wants to mess around)

- To run the site locally, open two terminals side by side running the following (assumning grunt and its packages are already installed):
    1. `grunt` for preprocessing, minification, etc.
    2. `grunt serve` this runs the jekyll serve task to build the site.
    3. Site should be running at [localhost:4000](http://localhost:4000)
- `_config-dev.yml` is for local dev since it doesn't return anything for `{{ site.baseurl }}`. **Only `baseurl` is taken from `config-dev.yml`, and the rest is taken from `config.yml` when running locally.**
- When shifting domains, remember to modify the `basurl` and `url` variables in `config.yml` so that asset linking works fine. **Remember to include `http://` for the baseurl**
- To avoid syncing conflicts, always use siteleaf directly to modify content.
