XTiger XML specification
========================

This is the home of the XTiger XML specification. That repository is used to edit and publish the [latest version](http://ssire.github.com/xtiger-xml-spec/) of the specification as GitHub pages.

It replaces the [former document](http://media.epfl.ch/Templates/XTiger-XML-spec.html) hosted at the [MEDIA group](http://media.epfl.ch) of the Ecole Polytechnique de Lausanne ([EPFL](http://ww.epfl.ch)).

What is this specification ?
------------------

The XTiger XML Specification defines several XML elements and their attributes which can be mixed on a XHTML host document using a special namespace. This allows to create *document templates*. Each document template can be transformed into an interactive editing application using an XTiger XML processing engine. It is then possible to author XML document constrained by the document template. The edited documents will be conform to a target XML content model embedded inside the template.

Where can I find an XTiger XML processing engine ?
----------------

[AXEL](https://github.com/ssire/axel) (Adaptable XML Editing Library) is an open source (LGPL v2.1) client-side Javascript XTiger XML processing engine.

How can I edit this specification ?
----------------

The source file of the specification (`XTiger-XML-spec.html`) is edited with the demonstration XML authoring application that comes with AXEL using the `template/Specification.xhtml` document template.

You can try it by yourself from your local file system. Here are the instructions for Firefox : 

1. checkout axel (`git clone git://github.com/ssire/axel.git`)
2. checkout xtiger-xml-spec (`git clone git://github.com/ssire/xtiger-xml-spec.git`)
3. open the `editor/editor.xhtml` application from AXEL
4. follow the on screen instructions to allow access to local files to Firefox (this is restricted by default)
5. click the _Browse_ button to select the `template/Specification.xhtml` document template and click the _Visualize_ button to generate the editor.
6. click the _Load_ button to select the `XTiger-XML-spec.html` souce file
7. start editing
8. click the _Save_ button to save your version of the specification to disk
 
NOTE: theses instructions are for Firefox although AXEL works with most browsers. This is because we haven't investigated yet the equivalent of _step 4_ for other browsers.

How to publish this specification ?
----------------

Checkout the gh-pages branch, then copy the latest version of `XTiger-XML-spec.html` from the master branch as `index.html`, then push the gh-pages branch.
