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

Execute the following commands if not already done:

.. code:: bash

sudo apt-get install xinit -y
sudo apt-get install git -y
sudo apt-get install maven2 -y
sudo apt-get install libsoup2.4-dev -y
sudo apt-get install openjdk-7-jdk -y



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

Finally, instead of xinit, there is the following alternative:

.. code:: bash

	  sudo apt-get install xserver-xorg-video-dummy 
	  wget xpra.org/xorg.conf 
	  Xorg -noreset +extension GLX +extension RANDR +extension RENDER -logfile ./0.log -config ./xorg.conf :0

If you have problems with port, just try another eg:

.. code:: bash

	  Xorg -noreset +extension GLX +extension RANDR +extension RENDER -logfile ./10.log -config ./xorg.conf :10

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

To install Java interface to arfilter, fetch artifact with artifactId arfilter from Maven Central Repository and install it:

.. code:: bash

http://search.maven.org/

.. code:: bash

Install the arfilter artifact, eg:

.. code:: bash

 mvn org.apache.maven.plugins:maven-install-plugin:2.5.2:install-file -Dfile=arfilter-1.0.0.jar

You can also install JavaScript interface:

.. code:: bash

bower install fi-vtt-nubomedia-kurento-module-armarkerdetector

Fetch keystore:

.. code:: bash

    wget -nd http://ssi.vtt.fi/ar-markerdetector-binaries/demo/keystore.jks


Fetch artifact with artifactId arfilterdemo from Maven Central Repository:

.. code:: bash

http://search.maven.org/


Execute artifact:

.. code:: bash

    java -jar arfilterdemo-1.0.1.jar


**On the client side**

Browse with WebRTC compliant browser (eg Chrome, Firefox) to the server
where ar3d is launched https://IP\_OF\_AR3DHOST:8443/ Change the
IP\_OF\_AR3DHOST and port (8443) if needed.

You should now see AR Demo so just follow the given instructions on that
page.
