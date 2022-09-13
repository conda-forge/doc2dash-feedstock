About doc2dash
==============

Home: https://pypi.org/project/doc2dash/

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/doc2dash-feedstock/blob/main/LICENSE.txt)

Summary: Convert docs to Dash.app

Development: https://github.com/hynek/doc2dash

Documentation: https://doc2dash.readthedocs.io/

doc2dash: Create docsets for Dash.app and clones
================================================

.. image:: https://readthedocs.org/projects/doc2dash/badge/?version=stable
   :target: https://doc2dash.readthedocs.io/en/stable/?badge=stable
   :alt: Documentation Status

.. image:: https://travis-ci.org/hynek/doc2dash.svg?branch=master
   :target: https://travis-ci.org/hynek/doc2dash

.. image:: https://codecov.io/github/hynek/doc2dash/branch/master/graph/badge.svg
  :target: https://codecov.io/github/hynek/doc2dash
  :alt: Test Coverage

.. begin


``doc2dash`` is an MIT-licensed extensible `Documentation Set`_ generator intended to be used with the `Dash.app`_ API browser for macOS or one of its many *free* `clones <https://doc2dash.readthedocs.io/en/latest/installation.html#viewer>`_ for all relevant platforms.

If you’ve never heard of Dash.app, you’re missing out:
together with ``doc2dash`` it’s all your API documentation at your fingertips!

``doc2dash``\ ’s documentation lives at `Read the Docs`_, the code on GitHub_.
It’s tested on Python 2.7, 3.4+, and PyPy.
Both Linux and macOS are tested although certain features are only available on macOS.


.. _`Documentation Set`: https://developer.apple.com/legacy/library/documentation/DeveloperTools/Conceptual/Documentation_Sets/010-Overview_of_Documentation_Sets/docset_overview.html#//apple_ref/doc/uid/TP40005266-CH13-SW6
.. _`Dash.app`: https://kapeli.com/dash/
.. _`Read the Docs`: https://doc2dash.readthedocs.io/
.. _`GitHub`:  https://github.com/hynek/doc2dash


Release Information
===================

2.2.0 (2017-06-12)
------------------

- ``InterSphinxParser`` is now open to extension.
  `#59 <https://github.com/hynek/doc2dash/pull/59>`_
- Support a ``--parser`` option to force the use of a custom parser class.
  `#60 <https://github.com/hynek/doc2dash/pull/60>`_

`Full changelog <https://doc2dash.readthedocs.io/en/stable/changelog.html>`_.

Authors
=======

``doc2dash`` is written and maintained by Hynek Schlawack.

The development is kindly supported by `Variomedia AG <https://www.variomedia.de/>`_.

A full list of contributors can be found on `GitHub's overview <https://github.com/hynek/doc2dash/graphs/contributors>`_.




Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=3883&branchName=main">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/doc2dash-feedstock?branchName=main">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-doc2dash-green.svg)](https://anaconda.org/conda-forge/doc2dash) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/doc2dash.svg)](https://anaconda.org/conda-forge/doc2dash) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/doc2dash.svg)](https://anaconda.org/conda-forge/doc2dash) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/doc2dash.svg)](https://anaconda.org/conda-forge/doc2dash) |

Installing doc2dash
===================

Installing `doc2dash` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `doc2dash` can be installed with `conda`:

```
conda install doc2dash
```

or with `mamba`:

```
mamba install doc2dash
```

It is possible to list all of the versions of `doc2dash` available on your platform with `conda`:

```
conda search doc2dash --channel conda-forge
```

or with `mamba`:

```
mamba search doc2dash --channel conda-forge
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search doc2dash --channel conda-forge

# List packages depending on `doc2dash`:
mamba repoquery whoneeds doc2dash --channel conda-forge

# List dependencies of `doc2dash`:
mamba repoquery depends doc2dash --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[Azure](https://azure.microsoft.com/en-us/services/devops/), [GitHub](https://github.com/),
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/),
[Drone](https://cloud.drone.io/welcome), and [TravisCI](https://travis-ci.com/)
it is possible to build and upload installable packages to the
[conda-forge](https://anaconda.org/conda-forge) [Anaconda-Cloud](https://anaconda.org/)
channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating doc2dash-feedstock
===========================

If you would like to improve the doc2dash recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/doc2dash-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@hoishing](https://github.com/hoishing/)
* [@pbronez](https://github.com/pbronez/)

