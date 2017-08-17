************
Prelude-SIEM
************

.. toctree::
   :maxdepth: 2

Prelude-SIEM is brought to you by CS (http://www.c-s.fr) under GPLv2 license :
https://www.prelude-siem.org

Copying and distribution of this library, with or without modification, are
permitted in any medium without royalty provided the copyright notice and this
notice are preserved. This file is offered as-is, without warranty of any kind.

For commercial use, if you need another license than GPLv2, please contact CS :
contact.prelude@c-s.fr

Prelude-SIEM Overview
=====================

Prelude is an agentless, universal, and hybrid security information and event
management (SIEM) system. Prelude collects, normalizes, sorts, aggregates,
correlates and reports all security-related events independently of the product
brand or license. Security events are normalized to an IDMEF format, allowing
native support with almost all security related event from an IT equipment.

While a malicious user (or software) may be able to evade the detection of a
single IDS (NIDS, HIDS, etc.), it becomes exponentially more difficult to get
around the defenses when there are multiple protection mechanisms. Prelude
comes with a large set of sensors, each of them monitoring different kind of
events. Prelude permits alert collection to WAN scale, whether its scope covers
a city, a country, a continent or the world.

Prelude claims that it is a SIEM system capable of inter-operating with all the
systems available on the market.[3] It is natively compatible with: AuditD,
Nepenthes, NuFW, OSSEC, Pam, Samhain, Sancp, Snort, and Suricata but anyone can
write its own sensors or utilize some of the 3rd party sensors that are
available, given Prelude's opened APIs and librairies.

Prelude SIEM Wiki
=================

`Global introduction <https://www.prelude-siem.org/projects/prelude/wiki>`_

* Introduction

  * `Glossary <https://www.prelude-siem.org/projects/prelude/wiki/PreludeGlossary>`_
  * `Prelude Components <https://www.prelude-siem.org/projects/prelude/wiki/PreludeComponents>`_
  * `Prelude Architecture <https://www.prelude-siem.org/projects/prelude/wiki/PreludeArchitecture>`_
  * `Prelude Standards <https://www.prelude-siem.org/projects/prelude/wiki/PreludeStandards>`_
  * `Prelude Compatibility <https://www.prelude-siem.org/projects/prelude/wiki/PreludeCompatibility>`_

* Installation

  * `Installation Requirements <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeRequirement>`_
  * `Installation from sources <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPrelude>`_

    * `Libprelude <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeLibrary>`_
    * `LibpreludeDB <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeDbLibrary>`_
    * `Prelude Manager <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeManager>`_
    * `Prelude Correlator <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeCorrelator>`_
    * `Prelude LML <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludeLml>`_
    * `Prewikka <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPreludePrewikka>`_

  * `Installation from packages <https://www.prelude-siem.org/projects/prelude/wiki/InstallingPackage>`_
  * Agents Installation

    * `Agents Registration <https://www.prelude-siem.org/projects/prelude/wiki/InstallingAgentRegistration>`_
    * `3rd Party Agents Installation <https://www.prelude-siem.org/projects/prelude/wiki/InstallingAgentThirdparty>`_

* Configuration

  * `General Configuration <https://www.prelude-siem.org/projects/prelude/wiki/ConfigurationGeneral>`_
  * Prelude Components Configuration

    * `Prelude-Manager <https://www.prelude-siem.org/projects/prelude/wiki/PreludeManager>`_
    * `Prelude-Correlator <https://www.prelude-siem.org/projects/prelude/wiki/PreludeCorrelator>`_
    * `Prelude-LML <https://www.prelude-siem.org/projects/prelude/wiki/PreludeLml>`_

  * `Howto Configure High Availability Central Services <https://www.prelude-siem.org/projects/prelude/wiki/HowtoHACentralServices>`_

* Optimisation

  * `Database Optimisation <https://www.prelude-siem.org/projects/prelude/wiki/DatabaseOptimisation>`_

* User Manuals

  * `Prewikka Manual <https://www.prelude-siem.org/projects/prelude/wiki/ManualPrewikka>`_
  * `Prelude-Admin Manual <https://www.prelude-siem.org/projects/prelude/wiki/ManualPreludeAdmin>`_
  * `PreludeDB-Admin Manual <https://www.prelude-siem.org/projects/prelude/wiki/ManualPreludeDbAdmin>`_

* Development

  * `Development guidelines <https://www.prelude-siem.org/projects/prelude/wiki/DevelopmentGuidelines>`_
  * `Source organization <https://www.prelude-siem.org/projects/prelude/wiki/SourceOrganization>`_
  * `Prewikka Apps <https://www.prelude-siem.org/projects/prelude/wiki/PrewikkaApps>`_
  * `Prelude Agent <https://www.prelude-siem.org/projects/prelude/wiki/DevelAgentQuickly>`_
  * `Prelude Agent contribution program <https://www.prelude-siem.org/projects/prelude/wiki/PreludeAgentContribution>`_

Prelude SIEM modules
====================

Prewikka
--------

Overview
^^^^^^^^

Originally written by Markus Alkio and Miika Keskinen, re-written and
maintained by Nicolas Delon with the help of Yoann Vandoorselaere and Audrey
Girard, on behalf of PreludeIDS Technologies, it was rapidly adopted as the new
Prelude frontend.

Prewikka is a professional looking application providing advanced features like
contextual filtering, aggregation, etc.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/prewikka

Prelude-Correlator
------------------

Overview
^^^^^^^^

Prelude-Correlator allows conducting multistream correlations thanks to a
powerful programming language for writing correlation rules. With any type of
alert able to be correlated, event analysis becomes simpler, quicker and more
incisive.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/prelude-correlator

Prelude-LML
-----------

Overview
^^^^^^^^

This is the Prelude-LML log analyzer, collecting events from log files
and/or syslog UDP messages.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/prelude-lml

Prelude-LML-Rules
-----------------

Overview
^^^^^^^^

Ruleset for pcre LML plugin.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/prelude-lml-rules

Prelude-Manager
---------------

Overview
^^^^^^^^

Prelude-Manager server is the Prelude events collector.

Prelude-Manager is a high availability server that accepts secured connections
from distributed sensors or other managers and saves received events to a media
specified by the user (database, logfile, mail, etc).

The server is a high availability server capable of handling large number of
connections, and processing large amounts of events. It uses a per client
scheduling queues in order to process events by severity fairly accross
clients.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/prelude-manager

LibPrelude
----------

Overview
^^^^^^^^

The Prelude Library is used to make sensor developers' life better by
providing features used by every sensor:

* Manager(s) Connection management (with fallback in case all configured
  Managers are down, and automatic reconnection).

* Interface to communicate with the Prelude Manager.

* Asynchronous Message interface (allowing sensor to emit message without
  blocking, even if there is latency on the wire).

* Asynchronous timer interface.

* Generic configuration API, providing a generic abstraction for command-line,
  configuration file option, and wide option support.

* Wide option managment allowing sensor-exported options to be directly
  accessible from the Manager administrative console.

* Generic plugin API.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/libprelude

LibPreludeDB
------------

Overview
^^^^^^^^

The PreludeDB Library provides an abstraction layer upon the type and the
format of the database used to store IDMEF alerts. It allows developers to use
the Prelude IDMEF database easily and efficiently without worrying about SQL,
and to access the database independently of the type/format of the database.

Github
^^^^^^

Project : https://github.com/Prelude-SIEM/libpreludedb

How to contribute
=================

IRC
---

If there's something you just can't find out elsewhere, you want to
give feedback directly to the authors or you're just bored, visit
#prelude on irc.freenode.net

Get Support
-----------

Prelude-user forums can be accessed at: 

* https://www.prelude-siem.org/projects/prelude/boards

Old mailing lists can be accessed at:

* http://premalink.gmane.org/gmane.comp.security.ids.prelude.user

Commercial Support is available through the CS company:

* http//www.prelude-siem.com, contact.prelude@c-s.fr

Help development
----------------

Submitting patches
^^^^^^^^^^^^^^^^^^

The Prelude source is constantly changing. If you want to submit a patch,
please do so from the most recent GIT source tree, subscribe to the
prelude-devel forum and post your patch with a description of functionality.
You can also attach patches to bugs on

* https://www.prelude-siem.org

Bugs
^^^^

If you find any bugs, please report them to:

* https://www.prelude-siem.org

Please make sure that what you're reporting is actually a BUG and not
a problem on your side.

Suggestions
^^^^^^^^^^^

Post on prelude-devel board and give us your suggestions.

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
