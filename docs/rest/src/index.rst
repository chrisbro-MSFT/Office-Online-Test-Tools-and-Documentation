
..  _index:

WOPI REST API Reference
=======================

..  sidebar:: Note

    This documentation is a work in progress. Topics marked with a |stub-icon| are placeholders that have not been
    written yet. You can track the status of these topics through our public documentation `issue tracker`_.

..  _issue tracker: https://github.com/Microsoft/Office-Online-Test-Tools-and-Documentation/issues


The Web Application Open Platform Interface Protocol (WOPI) defines a set of operations that enables a client to
access and change files stored by a server. WOPI is a REST-based protocol. It defines a set of
:ref:`REST endpoints<endpoints>` as well as operations that can be executed by issuing HTTP requests to those
endpoints.

The WOPI protocol is used by Office applications, such as Office Online, to view and edit files that are stored in
a cloud service. Thus, Office Online is a :term:`WOPI client`, while the cloud service that stores the files is a
:term:`WOPI server`, often referred to as a *host*.

This documentation is a reference for all of the defined WOPI operations. However, not all operations must be
implemented. WOPI is modular and a WOPI server need only implement the operations required by the WOPI client(s) the
server intends to integrate with. To learn more about the specific requirements for integrating with Office Online,
see the sections below:

* :ref:`officeonline:intro`


..  Navigation/TOC

..  toctree::
    :maxdepth: 2
    :hidden:
    :glob:
    :caption: Office WOPI Integrations

    Office Online <https://wopi.readthedocs.org/>


..  toctree::
    :maxdepth: 2
    :hidden:
    :glob:
    :caption: Getting Started

    /concepts
    /endpoints


..  toctree::
    :maxdepth: 2
    :hidden:
    :glob:
    :caption: File Operations

    /files/CheckFileInfo
    /files/GetFile
    /files/Lock
    /files/GetLock
    /files/RefreshLock
    /files/Unlock
    /files/UnlockAndRelock
    /files/PutFile
    /files/PutRelativeFile
    /files/RenameFile
    /files/PutUserInfo


..  toctree::
    :maxdepth: 2
    :glob:
    :hidden:
    :caption: Reference

    /glossary