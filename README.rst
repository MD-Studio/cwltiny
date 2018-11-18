################################################################################
cwltiny
################################################################################

A tiny workflow runner with partial CWL support.

This is a very minimal workflow runner that can run some CWL workflows. Its main
feature is that it does not have any dependencies beyond Python 3.4+ and its
standard library. This makes it easy to install in places where virtual
environments are hard to come by, such as some High Performance Computing
machines used in science, because you can just copy a single file and make it
executable.

Unfortunately, the trade-off is that many things are not supported, including
YAML. That means that you'll have to convert all workflows and steps to plain
JSON, and that many more advanced features of CWL won't work. You are probably
better off using ``cwltool`` in almost all situations; ``cwltiny`` was developed
as a fall-back solution for `Cerise <https://github.com/MD-Studio/cerise>`_ in
case ``cwltool`` cannot be used.

Installation
------------

To install cwltiny, do:

.. code-block:: console

  git clone https://github.com/MD-Studio/cwltiny.git
  cd cwltiny
  pip install .


Run tests (including coverage) with:

.. code-block:: console

  python setup.py test


Contributing
************

If you want to contribute to the development of cwltiny,
have a look at the `contribution guidelines <CONTRIBUTING.rst>`_.

License
*******

Copyright (c) 2018, Netherlands eScience Center and VU University Amsterdam

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
