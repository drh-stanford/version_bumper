= version_bumper

Simple. Bump your versions.

    $ gem install version_bumper

In your Rakefile `require 'version_bumper'` and you're done.
  
    $ rake -T
    rake bump:build     # bump build
    rake bump:init      # write a blank version to VERSION
    rake bump:major     # bump major
    rake bump:minor     # bump minor
    rake bump:revision  # bump revision
    
    
    $ rake bump:init
    version: 0.0.0.0
    $ rake bump:revision
    version: 0.0.1.0
    $ rake bump:major
    version: 1.0.0.0

You can optionally use `bumper_file 'version.txt'` in your rake file to switch from the default `VERSION` file name.
Use `bumper_version` anywhere you need access to the current version in your rake script.

== Contributing to version_bumper
 
* Check out the latest master to make sure the feature hasn't been implemented or the bug hasn't been fixed yet
* Check out the issue tracker to make sure someone already hasn't requested it and/or contributed it
* Fork the project
* Start a feature/bugfix branch
* Commit and push until you are happy with your contribution
* Make sure to add tests for it. This is important so I don't break it in a future version unintentionally.
* Please try not to mess with the Rakefile, version, or history. If you want to have your own version, or is otherwise necessary, that is fine, but please isolate to its own commit so I can cherry-pick around it.

== Copyright

Copyright (c) 2011 Dotan Nahum. See LICENSE.txt for
further details.
