source "https://rubygems.org"

# Use Jekyll 3.x for better compatibility
gem "jekyll", "~> 3.9"
gem "webrick", "~> 1.8"
gem "kramdown-parser-gfm"

# Jekyll plugins (same as used in _config.yml)
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  gem "jekyll-paginate"
  gem "jekyll-theme-minimal"
end

# Windows and JRuby does not include zoneinfo files
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
