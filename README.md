### Welcome to the *Zend Framework 2.0.0* Release!

Master: [![Build Status](https://secure.travis-ci.org/zendframework/zf2.png?branch=master)](http://travis-ci.org/zendframework/zf2)

## RELEASE INFORMATION

*Zend Framework 2.0.0rc3*

This is the third release candidate for 2.0.0. We will be releasing RCs
on a weekly basis until we feel all critical issues are addressed. At
this time, we anticipate few API changes before the stable release, and
recommend testing your production applications against it.

09 August 2012

### UPDATES IN RC3

- Zend\Http
  - Socket client: Updated to enable verify_peer by default, to prevent
    potential Man-In-The-Middle attacks.

- Zend\EventManager\SharedEventManager
  - SharedEventManager::attach now returns a callbackhandler for detaching,
    inline with what EventManager::attach does.

- Zend\Form\Annotation
  - Form annotation builder - if isRequired is true, automatically add required attribute.

- Zend\Mvc\Controller
  - Removed duplication between AbstractActionController and AbstractRestfullController.
    The AbstractController has the shared functions of both and allows to reuse it without the unneeded
    specific functions from AbstractActionController.

- Zend\Feed
  - Added trim() to XML input when importing an XML or HTML string. This prevent a few isolated problems
    with the feeds of some applications having illegal preceeding space in an XML feed.

- PSR-2 compatible
  - We refactored some of the components in order to be PSR-2 compatible. We will continue to check for
    PSR-2 compatibility in the next RC.

- Removed the doc2rst scripts
  - We removed the scripts bin/doc2rst.php, bin/doc2rst.xsl, and bin/ZendBin for the conversion from
    DocBook to reStructuredText (all the doc files have been converted).

Around 65 pull requests for a variety of features and bugfixes were handled
since RC2!

### SYSTEM REQUIREMENTS

Zend Framework 2 requires PHP 5.3.3 or later; we recommend using the
latest PHP version whenever possible.

### INSTALLATION

Please see INSTALL.md.

### CONTRIBUTING

If you wish to contribute to Zend Framework 2.0, please read both the
README-DEV.md and README-GIT.md file.

### QUESTIONS AND FEEDBACK

Online documentation can be found at http://framework.zend.com/manual.
Questions that are not addressed in the manual should be directed to the
appropriate mailing list:

http://framework.zend.com/wiki/display/ZFDEV/Mailing+Lists

If you find code in this release behaving in an unexpected manner or
contrary to its documented behavior, please create an issue in the Zend
Framework issue tracker at:

http://framework.zend.com/issues/browse/ZF2

If you would like to be notified of new releases, you can subscribe to
the fw-announce mailing list by sending a blank message to
<fw-announce-subscribe@lists.zend.com>.

### LICENSE

The files in this archive are released under the Zend Framework license.
You can find a copy of this license in LICENSE.txt.

### ACKNOWLEDGEMENTS

The Zend Framework team would like to thank all the [contributors](https://github.com/zendframework/zf2/contributors) to the Zend
Framework project, our corporate sponsor, and you, the Zend Framework user.
Please visit us sometime soon at http://framework.zend.com.
