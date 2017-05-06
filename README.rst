QCustomListWidget widget (PyQt)
*************************

- Git-hub repo: https://github.com/luchko/QCustomListWidget
- Free software: MIT license

Overview
========

``QCustomListWidget`` is a light code editor widget based on ``QPlainTextEdit`` and provides the following features:

- **line numbers bar** - set by DISPLAY_LINE_NUMBERS flag True
    
- **curent line highligthing** - set by HIGHLIGHT_CURRENT_LINE flag True
   
Widget is compatible with Python 2.7 or Python 3.3+ and PyQt4 4.6+ or PyQt5 5.2+.

-------------------------

.. figure::  ./demo.gif
   :align:   center
   :figwidth: 100 %
   
-------------------------

API
===

.. code-block:: python

    class QCodeEditor(QPlainTextEdit):

        def __init__(self, DISPLAY_LINE_NUMBERS=True, HIGHLIGHT_CURRENT_LINE=True,
                     SyntaxHighlighter=None, *args):        
            '''
            Parameters
            ----------
            DISPLAY_LINE_NUMBERS : bool 
                defines the presence of the lines number bar
            HIGHLIGHT_CURRENT_LINE : bool
                switch on/off the current line highliting
            SyntaxHighlighter : QSyntaxHighlighter
                should be inherited from QSyntaxHighlighter            
            '''                          

References:
===========

- XMLHighlighter: http://www.yasinuludag.com/blog/?p=49
- https://john.nachtimwald.com/2009/08/19/better-qplaintextedit-with-line-numbers/    
- http://doc.qt.io/qt-5/qtwidgets-widgets-codeeditor-example.htmls
