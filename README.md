# L'user Agent

Pardon my French?

So I guess it's [cute](http://webaim.org/blog/user-agent-string-history/) but most days I really don't give a about [all this](http://www.nczonline.net/blog/2010/01/12/history-of-the-user-agent-string/) browser user agent <abbr title="shit">detritus</abbr>.

I just want to know which browser, which version, which operating system.

## Usage

    var ua = luserAgent(navigator.userAgent);
    console.log("Hello "+ua.app+" "+ua.v+", on "+ua.os);
    console.log(", world.");

You can drop the semi-colons or put them at the beginning of your lines or whatever if you're annoying like that, but honestly I'd rather you just use CoffeeScript at that point.

Eventually when I need it this will work as a CommonJS (node.js/CouchDB/browserify) module too. Right now I sometimes just copy/paste the code into my projects because that is *awesome* also\*.

## WARNING

**PLEASE**: if you use this for [browser detection](http://css-tricks.com/browser-detection-is-bad/) you yes you Are The Reason we got this mess in the first place and I will cry. For you Argentina.

### Exceptions.

**If** all of the following are true:

- you are not using jQuery, and
- you have heard of Modernizr, and
- you have filed a bug for the browser bug you are fighting

**Then** you may use the provided information to gaurd a carefully considered workaround for said browser bug.

**Else** you may only use this library for human consumption (e.g. reable browser info for statitics or exception logs)

## Related work

c.f. <http://www.quirksmode.org/js/detect.html> and probably many many others but I got sick of not being able to find them


## Fine print

\* so I really don't recommend just copy-pasting this into your project because my code here can only improve, but I also really don't care.

License: [this](http://www.wtfpl.net/txt/copying/) but © me and I guess whoever else helped instead of that Sam dude. I don't even know that Sam dude.


## Rhetorically asked questions
### Dare I submit a pull request or even fork this you seem really rude.
### And you hate jQuery? WHO HATES JQUERY IT IS THE WEB?!!!

But I love you.