Personal Information Supply
===========================

This document describes a software architecture that satisfies the need
for an integrated and flexible interface to multiple, heterogenous computer systems.


Problem
-------

Todays developments in user interfaces focus on usability and appeal,
which creates an awesome world of great apps and sites.
However, from an end user perspective, the user interface (as a whole)
suffers from fragmentation and an exaggerated individualism.
Most user interfaces adapt to a companies brand and business goals,
but not to the users needs.

Looking at how user interfaces are implemented and integrated,
the means are quite low-level.
The implementation happens in terms of standard and custom-made graphical
elements like images, bars, buttons and boxes.
If a clear separation from business logic exists, it happens through
individually designed interfaces, either consisting of simple method calls,
or loosely adhering to communication protocols like SOAP and REST.
Most often, these interfaces transport data, but do only offer few (if none
at all) hints on the superior structure, relationships and semantics of
the data.

This contrasts to the information actually described by the data.
The information always obeys to a superior structure, having clear
relationships and a well-defined semantics -- because otherwise,
no human user would be able to understand and use the interfaces.
Therefore, we have a gap between the information transported and the means
of transportation.
Specifically, there is no general model that describes interfaces between
user and business logic.
But without a model there might might be no abstract reasoning and no
generic logic regarding the user interface.

Filling this gap by providing a common interface model for multiple
different, heterogenous backend systems allows us to provide the user with
one integrated and flexible user interface.
We can develop general logic and reason about how the user interface can
adopt to the user's needs, e.g. splitting the display between different
devices, without considering the concrete application.
Besides, an integrated interface model allows us to develop software
operating on these heterogenous backend systems, regardless of the singular
interface technologies they use.


Approach
--------

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

Thus, Personal Information Supply aims to **integrate** multiple systems into
one unified interface, and therefore separates service from interface.
This allows

* users to use multiple, heterogenous services through one common, unified and
  then well-known interface.
* developers to focus on service implementation.
  It is not _necessary_ to go through all the user interface design for every
  application (but should still be _possible_, if wanted). 
* developers to focus on interface implementation.
  By improving the interfaces provided through the Personal Information Supply,
  a benefit for users of many different applications can be created.

Possible user stories of an integrated **graphical user interface** could
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

Personal Motivation
-------------------

In Star Trek&#174;, computer systems are accessed using the
[LCARS](https://en.wikipedia.org/wiki/LCARS), which can be perceived as a
unified graphical user interface.
Every since I was a child, I wondered whether this could be a valid approach
for computer systems.
Faccia is my attempt to research this idea.

License
-------

Copyright (c) 2016-17 Felix Neumann.

Permission is granted to copy, distribute and/or modify this document
under the terms of the GNU Free Documentation License, Version 1.3
or any later version published by the Free Software Foundation;
with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
A copy of the license is included in the file `LICENSE`.
