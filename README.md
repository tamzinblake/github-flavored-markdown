[![build status](https://secure.travis-ci.org/thomblake/github-flavored-markdown.png)](http://travis-ci.org/thomblake/github-flavored-markdown)
See:
[github-flavored-markdown](http://github.github.com/github-flavored-markdown/)

As an npm package:

    npm install ghm

And then in your node program:

    var ghm = require("ghm")
    ghm.parse("I **love** GHM.\n\n#2", "isaacs/npm")
    // returns:
    // '<p>I <strong>love</strong> GHM.  '+
    // '<a href=\'http://github.com/isaacs/npm/issues/#issue/2\'>#2</a></p>'

To get the sha/issue/fork links, pass in a second argument specifying
the current project that things should be relative to.
