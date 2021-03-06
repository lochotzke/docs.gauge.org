.. role:: alternate-methods
.. role:: installer-icon
.. role:: macos

.. cssclass:: dynamic-content macos

:macos:`Step 1: Installing Gauge on macOS`
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section gives specific instructions on setting up Gauge in a macOS environment.

:installer-icon:`Install Using HomeBrew`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. admonition:: System Requirements

    - macOS  >= Mac OS X v10.6

    - Homebrew

    - Commandline tool

    - Terminal


1. Install brew if you haven't already: Go to the `brew website <https://brew.sh>`__, and follow the
directions there.

2. Run the brew command to install Gauge

.. code-block:: console

    brew install gauge

if HomeBrew is working properly, you should see something similar to the following:


.. code-block:: text

    ==> Downloading https://homebrew.bintray.com/bottles/gauge-1.0.6.mojave.bottle.tar.gz
    ==> Downloading from https://akamai.bintray.com/45/45b496b39ee682a95ca49b36a94e8041e03fca3644e80223c36539f495fee384?__gda__=exp=1568017021~hmac=f6ca3a9
    ######################################################################## 100.0%
    ==> Pouring gauge-1.0.6.mojave.bottle.tar.gz
    🍺  /usr/local/Cellar/gauge/1.0.6: 3 files, 18.5MB

.. cssclass:: alternate-installation

:alternate-methods:`Alternate Installation Methods`

.. cssclass:: collapsible curl-installer first

:installer-icon:`Install using CURL`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. cssclass:: toggle collapsible-content

    .. admonition:: System Requirements

        - macOS >= Mac OS X v10.6

        - Commandline tool (`curl` command)

        - Terminal


    Install Gauge to /usr/local/bin by running

.. cssclass:: toggle collapsible-content

.. code-block:: console

    curl -Ssl https://downloads.gauge.org/stable | sh

.. cssclass:: toggle collapsible-content

Or install Gauge to a [custom path] using

.. cssclass:: toggle collapsible-content
.. code-block:: console

    curl -Ssl https://downloads.gauge.org/stable | sh -- --location=[custom path]

.. cssclass:: collapsible zip-installer

:installer-icon:`Install using ZIP file`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. cssclass:: toggle collapsible-content

    .. admonition:: System Requirements

        - macOS >= Mac OS X v10.6

        - Commandline tool (`unzip` command)

        - Terminal

    1. For signed binaries first download the zip installer
            `Zip Installer <https://github.com/getgauge/gauge/releases/download/vGAUGE_LATEST_VERSION_PLACEHOLDER/gauge-GAUGE_LATEST_VERSION_PLACEHOLDER-darwin.x86_64.zip>`__

    2. Run the following command in your Commnad line tool to complete the installation.

.. cssclass:: toggle collapsible-content
.. code-block:: console

    unzip -o gauge-GAUGE_LATEST_VERSION_PLACEHOLDER-darwin.x86_64.zip -d /usr/local/bin


.. cssclass:: collapsible npm-installer

:installer-icon:`Install using NPM installation`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. cssclass:: toggle collapsible-content

    .. admonition:: System Requirements

        - `Node.js <nodejs.org>`__  >= 10.16.3 (LTS)

        - `NPM <npmjs.org>`__ >= (6.9.0)

        To install gauge using NPM you will need the latest node version.

            - `If you have Node.js already installed - to get the latest version of npm use the following command:`

            'npm install -g npm@latest'


    You can install Gauge by running the following command in Terminal.


.. cssclass:: toggle collapsible-content

.. code-block:: console

    npm install -g @getgauge/cli
