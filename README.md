yuicompressor-maven m2e connector
=============================================

This m2e connector for the yuicompressor maven plugin is designed to handle the compress and jslint goals of the [yuicompressor-maven-plugin](http://davidb.github.io/yuicompressor-maven-plugin/)

[![Build Status](https://buildhive.cloudbees.com/job/coderplus/job/m2e-connector-yuicompressor-maven-plugin/badge/icon)](https://buildhive.cloudbees.com/job/coderplus/job/m2e-connector-yuicompressor-maven-plugin/)

## FAQ ##

### How do I use it? ###

First off, note that this is currently Beta code.  It has been minimally tested, and all the usual early adopter
warnings apply.  That said if you're willing to help test the connector all you have to do is:

1. Drag the Install button into your eclipse workspace to install the connector from the Eclipse Market place
[![Install the Connector](http://marketplace.eclipse.org/sites/all/modules/custom/marketplace/images/installbutton.png)](http://marketplace.eclipse.org/marketplace-client-intro?mpc_install=1952619)

	or use the  [update site](http://coderplus.com/m2e-update-sites/yuicompressor-maven-plugin/)

2. Remove any [lifecycle mapping metadata](http://wiki.eclipse.org/M2E_plugin_execution_not_covered#ignore_plugin_goal)
you might have had in your POMs for the yuicompressor:compress or  yuicompressor:jslint goals.







That's it!  The connector will run on full builds. It will be executed on incremental builds only if something interesting to the plugin has changed.

### How can I help the project? ###

Thanks for asking...

* If you're a yuicompressor:compress or  yuicompressor:jslint user:
	* Test this out.  [File an issue](https://github.com/coderplus/m2e-connector-yuicompressor-maven-plugin/issues) if it doesn't
	work for you.  File an issue if you think it should do something more, or something different.
* If you're a Tycho/Eclipse Plugin/m2e  expert:
	* File an issue or submit a pull request if there is something that could be done better.
	* Contribute test cases.
* If you're a representative of the Eclipse Foundation or Apache Software Foundation or similar:
	* I'd be happy to consider donating this plugin&mdash;do get in touch.


## Thanks ##

Many thanks to the folks from the m2e-dev mailing list 
