# heroku-pgrootcert-buildpack

A buildpack that does one thing: create a symlink to the Heroku default system
CA certificates file into `~/.postgresql/root.crt`, so that PG client libraries
can use `sslmode=verify-full`.
