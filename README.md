# Py-Browser
Created web browser in python using Qt C++ framework

PyQt5 is a python library or Qt API for python. Qt is a C++ cross-platform framework. Qt is a very powerful graphical user interface (GUI) framework written in C++. Using PyQt, developers can use the Qt GUI framework in python. 
Necessary library: to install in terminal….
pip install PyQt5 
pip install os-sys 

from PyQt5.QtWidgets import *
from PyQt5.QtCore import *
from PyQt5.QtWebEngineWidgets import *
import sys

QtWidgets is a class that has all user interface objects. Widgets are the basic building blocks for GUI. Widgets can display data and GUI components such as buttons, labels, and text editors. QtCore contains the core classes that include the event loop, signals, and slot mechanism. It contains non/GUI functionality for files and directories. PyQtWebEngine is a set of Python bindings for Qt’s Web Engine framework. This module contains classes for a chromium-based implementation of a web browser.

self.browser = QWebEngineView()
The QwebEngineView class contains a web engine page and provides a widget that is used to view and edit web documents. 

self.browser.setUrl(QUrl("http://www.google.com"))
To set a default browser homepage as google homepage:

navbar = QToolBar()
A QToolBar widget is a movable panel consisting of text buttons, buttons with icons, or other widgets such as a navigation bar. 

back_btn = QAction('⮜', self)
QAction may contain an icon, menu text, a shortcut, status text, "What's This?" text, and a tooltip. Most of these can be set in the constructor.

self.url_bar = QLineEdit()
The QLineEdit widget is a one-line text editor. A line edit allows the user to enter and edit a single line of plain text with a useful collection of editing functions, including undo and redo, cut and paste, and drag and drop. For example, here, it uses to add a URL bar within the navigation bar. 

![py_browser](https://user-images.githubusercontent.com/58274552/187764223-1b93fd27-a35d-4214-ad9c-5020525ffea3.PNG)
