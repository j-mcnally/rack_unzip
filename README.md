# Rack Unzip

This is a simple Rack middleware based on https://gist.github.com/relistan/2109707

It will unzip gzipped post bodies.


Add The gem

`gem 'rack_unzip', github: 'j-mcnally/rack_unzip'`

Add the Middleware

```
config.middleware.insert_before ActionDispatch::ParamsParser, 'RackUnzip::CompressedRequests'
```
