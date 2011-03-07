CloudFiles-Nukem
=======

**cloudfiles-nukem** is a Rackspace CloudFiles variation of [s3nukem](https://github.com/lathanh/s3nukem) which is a slightly improved version of [s3nuke](http://github.com/SFEley/s3nuke/), a Ruby script by Steve Eley that relatively quickly deletes an Amazon Web Services (AWS) Simple Storage Service (S3) bucket with many objects (millions) by using multiple threads to retrieve and delete the individual objects.

Installation
------------
### You'll need:

* **Ruby >= 1.87**
    Ruby 1.9 should work faster because of the native thread implementation (on the other hand, network/S3 latency may be your biggest bottleneck).

* **[ruby-cloudfiles](https://github.com/rackspace/ruby-cloudfiles) gem** 

        sudo gem install cloudfiles

### Download and make executable; e.g.,

    # download
    git clone git@github.com:hathaway/cloudfiles-nukem.git

    # make executable
    chmod 755 cloudfiles-nukem


Obvious Warning
---------------
This script is _intended_ to delete all of the items in a CloudFiles container very quickly. You will not be prompted to ask you if you're sure. There is no undo.


License
-------
This script is released under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0). I really don't care what you do with it, so long as "sue me" is not on the agenda.


Credits
-------
Original s3nuke script by [Steve Eley](http://extraneous.org/).

Improvements by [Robert LaThanh](http://robertlathanh.com/2010/07/s3nukem-delete-large-amazon-s3-buckets/).

CloudFiles version by [Ben Hathaway](http://hathology.com/).
