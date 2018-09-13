python-vipaccess
================

|PyPI| |License| |Build Status| |Coverage Status|

python-vipaccess is a free and open source software (FOSS)
implementation of Symantec's VIP Access client. It is able to generate
OATH URIs and their corresponding QR codes so any TOTP-generating
application can be used as a VIP OTP token.

Right now, it only supports the bare minimum number of features of the
VIP Access provisioning protocol to work, but I might add support for
the other features at some point in the future.

You can see my original blog post
`here <https://www.cyrozap.com/2014/09/29/reversing-the-symantec-vip-access-provisioning-protocol/>`__,
in which I describe how I reverse-engineered the VIP Access application.

Dependencies
------------

-  Python 2.6, 2.7, 3.3, 3.4, 3.5
-  `image <https://pypi.python.org/pypi/image/1.3.3>`__
-  `lxml <https://pypi.python.org/pypi/lxml/3.4.0>`__
-  `oath <https://pypi.python.org/pypi/oath/1.2>`__
-  `PyCrypto <https://pypi.python.org/pypi/pycrypto/2.6.1>`__
-  `qrcode <https://pypi.python.org/pypi/qrcode/5.0.1>`__
-  `requests <https://pypi.python.org/pypi/requests/>`__

If you have ``pip`` installed on your system, you can easily install the dependencies by running
``pip install -r requirements.txt`` in the project root directory.

To install ``pip`` see the ``pip`` installation documentation `here <https://pip.pypa.io/en/stable/installing/>`__.

Installation
------------

Via pip (recommended)
~~~~~~~~~~~~~~~~~~~~~

``pip install python-vipaccess``

Manual
~~~~~~

1. Check out this repository by running
   ``git clone https://github.com/cyrozap/python-vipaccess.git``
2. Switch to the ``python-vipaccess`` directory by running
   ``cd python-vipaccess``
3. Install the ``vipaccess`` module

   -  With pip: ``pip install .``
   -  Without pip: ``python setup.py install``

Usage
-----

Execute ``vipaccess`` (it should be in your ``PATH``).

.. |PyPI| image:: https://img.shields.io/pypi/v/python-vipaccess.svg
   :target: https://pypi.python.org/pypi/python-vipaccess
.. |License| image:: https://img.shields.io/pypi/l/python-vipaccess.svg
   :target: https://www.apache.org/licenses/LICENSE-2.0.html
.. |Build Status| image:: https://travis-ci.org/cyrozap/python-vipaccess.svg?branch=master
   :target: https://travis-ci.org/cyrozap/python-vipaccess
.. |Coverage Status| image:: https://coveralls.io/repos/cyrozap/python-vipaccess/badge.svg?branch=master
   :target: https://coveralls.io/r/cyrozap/python-vipaccess?branch=master
