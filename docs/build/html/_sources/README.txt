.. _README:

*****
Readme
*****
This project is part of NUBOMEDIA
`www.nubomedia.eu <http://www.nubomedia.eu>`__

========================= 

This document describes how to utilize the
`ARModule <https://github.com/nubomedia-vtt/armodule>`__

Some material that can be utilized is given at the end.


**Artifacts**

Maven Central:

http://repo1.maven.org/maven2/fi/vtt/nubomedia/arfilter/
http://repo1.maven.org/maven2/fi/vtt/nubomedia/kurento/arfilterdemo/

Npm:
https://www.npmjs.com/package/fi-vtt-nubomedia-kurento-module-armarkerdetector


**On the Server Side**

To lauch the test program clone this repository and execute

.. code:: bash

    cd armoduledemos/ar3d
    mvn compile exec:java -Dexec.mainClass="fi.vtt.nubomedia.kurento.Ar3DApp"

**On the Client Side**

Browse with WebRTC compliant browser (eg Chrome, Firefox) to the server
where ar3d is launched http://IP\_OF\_AR3DHOST:8080/ Change the
IP\_OF\_AR3DHOST and port (8080) if needed.

You should now see AR Demo so just follow the given instructions on that
page.

**Note For Ubuntu Desktop Users**

On some environments, for some reason, it has been reported that since
KMSv6 screen can get partially or totally blank. But because ssh works,
it might be better to install ssh server beforehand to gain control to
the host again.

Material
========

**Augmented Models**

Some models can be found eg from
`models <https://github.com/nubomedia-vtt/armoduledemos/tree/master/Models>`__
