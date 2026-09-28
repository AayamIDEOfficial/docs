.. _dev-intro:

AayamIDE Developer Guide
==========================

General information/guide about building the AayamIDE project locally. User's wiki is available :doc:`here </user/index>`.

.. note:: 
  The documentation is still a work in progress. It may contain out-of-date or incomplete information. If you find any issues,
  please open an issue at https://github.com/AayamIDEOfficial/docs/issues.

.. _dev-intro-projects:

Projects
--------

All source code that belongs to AayamIDE are split between repositories under the `AayamIDEOfficial <https://github.com/AayamIDEOfficial>`_
GitHub organisation.


* `AayamIDE <https://github.com/AayamIDEOfficial/AayamIDE>`_ - The AayamIDE application sources.
* `terminal-packages <https://github.com/AayamIDEOfficial/terminal-packages>`_ -
  patches and build system for the terminal packges (fork of `termux-packages <https://github.com/termux/termux-packages>`_\ ).
* `android-tree-sitter <https://github.com/AayamIDEOfficial/android-tree-sitter>`_ -
  Java bindings for the `tree-sitter <https://github.com/tree-sitter/tree-sitter>`_ library for fast and incremental syntax analysis.
* `androidide-tools <https://github.com/AayamIDEOfficial/androidide-tools>`_ -
  basic bash scripts for AayamIDE (including the installation script). The Android SDK updates and build/platform tools
  for AayamIDE are released in this repository.
* `platform-tools <https://github.com/AayamIDEOfficial/platform-tools>`_ -
  Patches and build configuration for building Android build/platform tools (``aapt2``, ``aidl``, ``adb``, etc.) for AayamIDE.
* `tree-sitter-* <https://github.com/orgs/AayamIDEOfficial/repositories?q=tree-sitter&type=all&language=&sort=>`_ - tree sitter grammars for AayamIDE.

This wiki provides information about building the `AayamIDE <https://github.com/AayamIDEOfficial/AayamIDE>`_ project.
To build other projects, visit the respective GitHub repositories.

.. _dev-intro-external_projects:

External projects
-----------------

Apart from the projects that are hosted under the GitHub organisation, AayamIDE also uses other projects. Some of them are listed below.


* `sora-editor <https://github.com/Rosemoe/sora-editor>`_ - A multifunctional Android code editor library.
* `AOSP <https://cs.android.com>`_ - AayamIDE uses projects from the Android Open Source Project.

  * `aaptcompiler* <https://github.com/AayamIDEOfficial/AayamIDE/tree/dev/subprojects/aaptcompiler>`_ -
    for parsing and analyzing XML sources in Android modules.
  * `layoutlib-api* <https://github.com/AayamIDEOfficial/AayamIDE/tree/dev/subprojects/layoutlib-api>`_ -
    The layoutlib API (required by aaptcompiler).
  * `tools-common <https://cs.android.com/android-studio/platform/tools/base/+/mirror-goog-studio-main:common/>`_ -
    Android SDK Commons.
  * other tools from AOSP (listed in version catalog)

* `nb-javac-android* <https://github.com/AayamIDEOfficial/nb-javac-android>`_ - The JDK 17's Java Compiler ported for Android
  (based on `nb-javac <https://github.com/oracle/nb-javac>`_\ ). It includes the following modules :

  * ``java-compiler`` - Java Compiler API.
  * ``jdk-compiler`` - Java Compiler (internal) implementation.
  * ``jdk-jdeps``

* `javapoet* <https://github.com/square/javapoet>`_ - for dynamically creating Java files.
* `eclipse-lemminx* <https://github.com/eclipse/lemminx>`_ - The DOM API from the Eclipse LemMinX project.
* `jaxp* <https://www.oracle.com/java/technologies/jaxp-introduction.html>`_ - for parsing & processing XML files (required by LemMinX's Parser).
* `flashbar* <https://github.com/aritraroy/Flashbar>`_ - for showing (interactive) messages in the IDE.
* `fuzzywuzzy* <https://github.com/xdrop/fuzzywuzzy>`_ - for fuzzy matching completion items.

*Projects marked with * are included directly in AayamIDE (i.e. they are built from source).*

.. _dev-intro-other_repos:

Other repositories
------------------

The following are some of the projects that are not directly linked with AayamIDE but can still be helpful to users/developers :

* `MrIkso/AayamIDE-NDK <https://github.com/MrIkso/AayamIDE-NDK>`_ - Script for installing NDK in AayamIDE.

.. _dev-intro-translations:

Translations
------------

Translations are managed on Crowdin. You can visit the `Crowdin project page <https://crowdin.com/project/androidide>`_ to help with the translations.

AayamIDE is translated into 10+ languages, thanks to all the `Crowdin contributors <https://crowdin.com/project/androidide/members>`_.

.. _dev-intro-projects-help_&_support:

Help & Support
--------------


* `Telegram group <https://t.me/androidide_discussions>`_ - You can join the Telegram group to discuss bugs, features and suggestions.
* `Telegram channel <https://t.me/AayamIDEOfficial>`_ - Join the channel to get latest updates about AayamIDE.

If you have any questions or need assistance with the contribution process, please don't hesitate to reach out.
We value your commitment to open source and look forward to collaborating with you.
