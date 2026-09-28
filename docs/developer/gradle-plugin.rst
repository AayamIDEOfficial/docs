.. _dev-gradle_plugin:

The AayamIDE Gradle Plugin
============================

The AayamIDE Gradle Plugin (``:gradle-plugin`` module) is used to configure the build for a project that is built **inside** AayamIDE.

.. _dev-gradle_plugin-initscript_plugin:

Init Script Plugin
------------------

The `AayamIDEInitScriptPlugin <https://github.com/AayamIDEOfficial/AayamIDE/blob/dev/gradle-plugin/src/main/java/com/itsaky/androidide/gradle/AayamIDEInitScriptPlugin.kt>`_ is applied using the `auto-generated <https://github.com/AayamIDEOfficial/AayamIDE/blob/dev/build-logic/ide/src/main/java/com/itsaky/androidide/plugins/tasks/GenerateInitScriptTask.kt>`_ Gradle initialization script. This init script configures the repositories and classpath for the root project and then applies the `AayamIDEPlugin <https://github.com/AayamIDEOfficial/AayamIDE/blob/dev/gradle-plugin/src/main/java/com/itsaky/androidide/gradle/AayamIDEGradlePlugin.kt>`_ to all subprojects.

.. _dev-gradle_plugin-project_plugin:

Project Plugin
--------------

The `AayamIDEPlugin <https://github.com/AayamIDEOfficial/AayamIDE/blob/dev/gradle-plugin/src/main/java/com/itsaky/androidide/gradle/AayamIDEGradlePlugin.kt>`_ configures all the subprojects. At the time of this writing, it only applies the ``LogSenderPlugin`` to all Android application modules (\ ``com.android.application``\ ).

.. _dev-gradle_plugin-logsender_plugin:

LogSender Plugin
----------------

The `LogSenderPlugin <https://github.com/AayamIDEOfficial/AayamIDE/blob/dev/gradle-plugin/src/main/java/com/itsaky/androidide/gradle/LogSenderPlugin.kt>`_ adds the LogSender dependency (\ ``:logsender`` module published to Maven Central) to all the debuggable variants of the Android application module.
