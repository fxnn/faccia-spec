Faccia: Idea
============

Faccia is a software system to provide integrated and unified interfaces to
multiple, heterogenous computer systems.

Hereby, a **computer system** is any system that offers its functionality via
an interface to third party software.
An interface could be e.g. REST, SOAP, RPC or simple commandline calls.

An **interface** could possibly be

* a graphical user interface (GUI).
* a textual user interface.
* an interface for users with disabilities, for example providing only haptic
  or acoustic input and output.
* an interface for automatic service discovery through third party software.
* an application programmer's interface (API).

Thus, Faccia aims to **integrate** multiple systems into one unified interface,
and therefore separates service from interface.
This allows

* users to use multiple, heterogenous services through one common, unified and
  then well-known interface.
* developers to focus on service implementation.
  It is not necessary to go through all the user interface design for every
  application.
* developers to focus on interface implementation.
  By improving the interfaces provided through Faccia, a benefit for users of
  many different applications can be created.

Possible user stories of an integrated Faccia **graphical user interface** could
be as follows.

* The user reconfigures the user interface to adapt it to his habits.
* The user interface proposes automatic reconfiguration to the user, based
  on how frequent and in what relationship the user interacted with UI elements.
* The user connects multiple of his devices over a network, allowing him to
  combine the user interfaces. Examples:
   * The user connects is mobile device to his television, so that he can use
     his mobile device as a remote control. 
   * The user connects his mobile device to his television, so that he can use
     the television as a larger screen for data retrieved on the mobile device.
   * The user connects his tablet to a couple of virtual machines, controlling
     the VMs from his tablet.

Naming
------

The name Faccia is the italian word for _face_.
It reminds of Faccia being a facade for multiple systems.

Motivation
----------

In Star Trek&#174;, computer systems are accessed using the
[LCARS](https://en.wikipedia.org/wiki/LCARS), which can be perceived as a
unified graphical user interface.
Every since I was a child, I wondered whether this could be a valid approach
for computer systems.
Faccia is my attempt to research this idea.
