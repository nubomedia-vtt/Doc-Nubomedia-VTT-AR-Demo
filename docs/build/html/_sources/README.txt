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

**License**

Kurento is distributed as Open Source Software basing LGPL v2.1 license.

ALVAR 2.0.0 - A Library for Virtual and Augmented Reality Copyright 2007-2012 VTT Technical Research Centre of Finland Licensed under the GNU Lesser General Public License

Irrlicht Engine, the zlib and libpng. The Irrlicht Engine is based in part on the work of the Independent JPEG Group The module utilizes IJG code when the Irrlicht engine is compiled with support for JPEG images.

**Contribution policy**

You can contribute to the Nubomedia community through bug-reports, bug-fixes, new code or new documentation. For contributing to the Nubomedia community, drop a post to the [Nubomedia Public Mailing List] providing full information about your contribution and its value. In your contributions, you must comply with the following guidelines

* You must specify the specific contents of your contribution either through a
  detailed bug description, through a pull-request or through a patch.
* You must specify the licensing restrictions of the code you contribute.
* For newly created code to be incorporated in the Nubomedia code-base, you must
  accept Nubomedia to own the code copyright, so that its open source nature is
  guaranteed.
* You must justify appropriately the need and value of your contribution. The
  Nubomedia project has no obligations in relation to accepting contributions
  from third parties.
* The Nubomedia project leaders have the right of asking for further
  explanations, tests or validations of any code contributed to the community
  before it being incorporated into the Nubomedia code-base. You must be ready to
  addressing all these kind of concerns before having your code approved.

Support

-------
Support is provided through the [Nubomedia Public Mailing List]

[NUBOMEDIA]: http://www.nubomedia.eu
[Nubomedia Public Mailing List]: https://groups.google.com/forum/#!forum/nubomedia-dev
