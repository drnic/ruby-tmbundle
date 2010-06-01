Ruby TextMate bundle
--------------------

The TextMate bundle that first appeared in the famous "Rails 15 minute video." This is it, many years later.

Installation
============

To install via Git:

    mkdir -p ~/Library/Application\ Support/TextMate/Bundles
    cd ~/Library/Application\ Support/TextMate/Bundles
    git clone git://github.com/drnic/ruby-tmbundle.git "Ruby.tmbundle"
    osascript -e 'tell app "TextMate" to reload bundles'

Source can be viewed or forked via GitHub: [http://github.com/drnic/ruby-tmbundle](http://github.com/drnic/ruby-tmbundle)

Validate and Save
=================

When you save a Ruby file, it will first validate the syntax and print any validation error as a tooltip.

<img src="http://img.skitch.com/20100601-eiw1ugr2ma8xwxbecjfbbpfgpk.preview.jpg" alt="Validate and Save - No Rubinius" />

You can get more detailed syntax error information if you have Rubinius installed (and `rbx` in TextMate's $PATH).

<img src="http://img.skitch.com/20100601-r66y9yr8nb14br4esi436prn1p.preview.jpg" alt="Validate and Save - Rubinius installed" />

If you have Homebrew installed:

    brew install rubinius

Then in TextMate, add your homebrew `bin` folder to the $PATH.

* Go to TextMate's Preferences (Cmd+,)
* Go to "Advanced", then "Shell Variables"
* Edit the `PATH` variable, and add ":/path/to/homebrew/bin"

For example, if you have homebrew installed in `~/.homebrew` then you might add `:/Users/drnic/.homebrew/bin`

Save a dodgy Ruby file and see the beautifully helpful syntax message.