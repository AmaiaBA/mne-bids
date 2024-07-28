:orphan:

.. _whats_new:

.. currentmodule:: mne_bids

What's new?
===========

.. _changes_0_16:

Version 0.16 (unreleased)
-------------------------

👩🏽‍💻 Authors
~~~~~~~~~~~~~~~

The following authors contributed for the first time. Thank you so much! 🤩

* `Amaia Benitez`_

The following authors had contributed before. Thank you for sticking around! 🤘

* `Daniel McCloy`_
* `Eric Larson`_
* `Stefan Appelhoff`_

Detailed list of changes
~~~~~~~~~~~~~~~~~~~~~~~~

🚀 Enhancements
^^^^^^^^^^^^^^^

- nothing yet

🧐 API and behavior changes
^^^^^^^^^^^^^^^^^^^^^^^^^^^

- :func:`mne_bids.read_raw_bids` no longer warns about unit changes in channels upon reading, as that information is taken from ``channels.tsv`` and judged authorative, by `Stefan Appelhoff`_ (:gh:`1282`)

🛠 Requirements
^^^^^^^^^^^^^^^

- MNE-BIDS now requires MNE-Python 1.6.0 or higher.

🪲 Bug fixes
^^^^^^^^^^^^

- When anonymizing the date of a recording, MNE-BIDS will no longer error during `~mne_bids.write_raw_bids` if passing a `~mne.io.Raw` instance to ``empty_room``, by `Daniel McCloy`_ (:gh:`1270`)
- Fixed a KeyError in the `_channels_tsv()` function when using the `write_raw_bids()` command for OPM data by expanding the list of supported OPM channels in `get_coil_types()`, by `Amaia Benitez`_ (gh:1222:)

⚕️ Code health
^^^^^^^^^^^^^^

- Keep MNE-BIDS up to date with recent changes on participant birthday date handling in MNE-Python, by `Eric Larson`_ (gh:1278:)
- Make rules for linting more strict, make quality assessment exceptions less permissive, by `Stefan Appelhoff`_ (gh:1283:)

:doc:`Find out what was new in previous releases <whats_new_previous_releases>`

.. include:: authors.rst
