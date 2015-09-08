Keera Hails is a toolkit to create reactive applications in Haskell.
It facilitates creating interactive applications that combine User
Interfaces, external devices, networks connections, files and, optionally,
FRP networks.

Keera Hails is modular and extensible. It is cross platform (Windows, Linux,
MacOSX, Android, GHCJS), UI-agnostic (Gtk+, WX, Qt, Android Native toolkit,
HTML DOM), FRP-agnostic and device-agnostic (Wiimote, Webcams, etc).

Keera Hails has been used to create large applications and is used commercially
in production.

The toolkit is divided in three parts:
* Reactive Values: they are typed mutable values with event dispatching and
access properties. They can be modified by lifting functions and applying
lenses to them. They can also be connected so that they stay in sync during
program execution.

  - http://github.com/keera-studios/hails-reactivevalues
  - http://github.com/keera-studios/hails-reactivelenses

* Reactive bindings: Widget properties/attributes can be seen as
reactive values. So can network sockets, files, application models ('model'
as in MVC) and external resources (polling). Uni-directional, Functional
Reactive Programming signal functions can also be wrapped into a pair
of RVs (see Yampa). The idea is that, at the highest application level
(controller), each layer is wrapped in a reactive container and connected
to others.

  - http://github.com/keera-studios/hails-reactive-fs
  - http://github.com/keera-studios/hails-reactive-network
  - http://github.com/keera-studios/hails-reactive-gtk
  - http://github.com/keera-studios/hails-reactive-wx
  - http://github.com/keera-studios/hails-reactive-qt
  - http://github.com/keera-studios/hails-reactive-htmldom (via GHCJS)
  - http://github.com/keera-studios/keera-hails-reactive-yampa
  - http://github.com/keera-studios/keera-hails-reactive-polling
  
  An experimental Android backend that uses Android's Native UI toolkit
  is also available. Please, contact Keera Studios if you wish to
  use it.

* Hails: a series of tools and libraries to create MVC programs using
  a reactive interface. The application architecture takes the approach of
  "convention over configuration", which means that certain modules will be
  expected to have predetermined names. If this is much of a problem, open a
  bug report.

  - http://github.com/keera-studios/keera-hails (this repository)
  - http://github.com/keera-studios/hails-mvc-model-lightmodel
  - http://github.com/keera-studios/hails-mvc-model-protectedmodels
  - http://github.com/keera-studios/hails-mvc-view-gtk
  - http://github.com/keera-studios/hails-mvc-view
  - http://github.com/keera-studios/hails-mvc-controller
  - http://github.com/keera-studios/hails-mvc-environment-gtk
  - http://github.com/keera-studios/hails-mvc-solutions-gtk
  - http://github.com/keera-studios/hails-mvc-solutions-config
  - http://github.com/keera-studios/hails-i18n
  - http://github.com/keera-studios/hails-templates

For a introduction to reactive values, see:
* [Bridging the GUI gap with reactive values and relations](http://dl.acm.org/citation.cfm?id=2804316)
* [Readme for Reactive Value library](http://github.com/keera-studios/hails-reactivevalues)
* [Ivan Perez's 1st PhD report, pages 29 and 40](http://www.cs.nott.ac.uk/~ixp/papers/2014-Perez-1st-year-report.pdf)
(page 40 is a paper of its own; page 29 is the thesis proposal outlining the
core ideas and problems that remain to be solved.)
* [TFP 2014 Pre-proceedings, pages 59-68](http://www.staff.science.uu.nl/~hage0101/preproceedingstfp2014.pdf)
* [Reactive Programming using Reactive Values (blog post)](http://keera.co.uk/blog/2014/05/24/reactive-programming-using-reactive-values/)
  
For bibtex references to these articles, see Publications in http://www.cs.nott.ac.uk/~ixp/.

Applications:
* http://github.com/keera-studios/keera-posture
* http://github.com/ivanperez-keera/SoOSiM-ui
* http://github.com/keera-studios/hails-reactive-wiimote-demo
* http://github.com/ivanperez-keera/haskellifi-trayicon
* http://github.com/ivanperez-keera/keera-diamondcard-sms-trayicon