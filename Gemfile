source "https://rubygems.org"

gem "rake"

group :test do
  platforms :jruby do
    gem "activerecord-jdbcmysql-adapter"
    gem "jdbc-mysql"

    gem "activerecord-jdbcpostgresql-adapter"
    gem "jdbc-postgres"

    gem "activerecord-jdbcsqlite3-adapter"
    gem "jdbc-sqlite3"
  end

  platforms :ruby, :mswin, :mingw do
    gem "mysql", "~> 2.9"
    gem "pg"
    gem "sqlite3"
    gem "mysql2"
  end

  gem "coveralls", require: false
  gem "rspec", ">= 3"
  gem "rubocop", ">= 0.23"
  gem "simplecov", require: false
end

gem "delayed_job", platforms: :ruby,
  git: 'https://github.com/yangzhichina/delayed_job.git',
  branch: 'delayed_job_for_rails510'

gemspec
