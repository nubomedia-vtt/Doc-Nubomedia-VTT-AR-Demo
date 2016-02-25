*****
Installation Guide
*****


Installing Optional ArMarkerDetectorDemo
========================================

These are the instructions how to utilize the ar-markerdetector filter
of of the `ARModule <https://github.com/nubomedia-vtt/armodule>`__.
Thus, after installation of ar-markerdeterctor is done, you can test the
filter with this sample application.

It is assumed that the sample application will be installed to the same
host where KMS is installed. Otherwise change the code of ar3d.

**Installing**

Fetch and execute the installation script:

.. code:: bash

    wget -N https://github.com/nubomedia-vtt/armoduledemos/raw/master/install_ar3d.sh
    chmod u+x ./install_ar3d.sh
    ./install_ar3d.sh

**For Ubuntu Server Users**

Run X:

.. code:: bash

    xinit

If you're not authorized to run X, the following might help:

.. code:: bash

    sudo dpkg-reconfigure x11-common

**For Ubuntu Desktop Users**

If you're not authorized to access X, then:

.. code:: bash

    xhost +

On some environments, for some reason, it has been reported that since
KMSv6 screen can get partially or totally blank. But if you are
utilizing Ubuntu Server installation this is not an issue.

Models
------

Copy some sample models from:

.. code:: bash

    https://github.com/nubomedia-vtt/armoduledemos/tree/master/Models

into the default folder that is:

.. code:: bash

    /opt

Artifact
--------

**On the server side**

Fetch artifact and execute it:

.. code:: bash

    wget -nd http://ssi.vtt.fi/ar-markerdetector-binaries/ar-markerdetector_0.0.6~rc1_java/armarkerdetector-6.1.0.jar
    wget -nd http://ssi.vtt.fi/ar-markerdetector-binaries/ar-markerdetector_0.0.6~rc1_java/keystore.jks
    java -jar armarkerdetector-6.1.0.jar

**On the client side**

Browse with WebRTC compliant browser (eg Chrome, Firefox) to the server
where ar3d is launched https://IP\_OF\_AR3DHOST:8443/ Change the
IP\_OF\_AR3DHOST and port (8443) if needed.

You should now see AR Demo so just follow the given instructions on that
page.
