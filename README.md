This is outdated.  Use `marked` instead.

This is an implementation of
[Markdown](http://daringfireball.net/projects/markdown/) forked from
GitHub's own Javascript implentation.  It is designed to be usable in
Node or the browser.

As an npm package:

    npm install ghm

And then in your node program:

    var ghm = require('ghm')
    ghm.parse('I **love** GHM.\n\n#2', 'isaacs/npm')
    // returns:
    // '<p>I <strong>love</strong> GHM.  '+
    // '<a href="http://github.com/isaacs/npm/issues/2">#2</a></p>'

To get the sha/issue/fork links, pass in a second argument specifying
the current project that things should be relative to.
