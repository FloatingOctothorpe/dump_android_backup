Dump Android backup
===================
This is a short Python script to extract Android backups. Although the script
should work as expected, it's mainly a proof of concept, I would recommend
using [Android backup extractor][github-abe] instead if
Java is available on your system.

Installation
------------
Clone the script from GitHub:

    git clone https://github.com/FloatingOctothorpe/dump_android_backup.git

This script requires [pyaes][pypi-pyaes]; you can install this using `pip`:

    pip install -r requirements.txt

Usage
-----
The script should called with a minimum of two arguments, the path to the
backup file and an output file:

    dump_android_backup.py BACKUP_FILE OUTPUT_FILE

By default if a password is required the script will prompt for it.
Alternatively the `-p` option can be used to specify the password as an
augment. The `-d` option can also be used to show debug output.

License
-------
This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the [GNU General Public License][gplv3] for more
details.

[github-abe]: https://github.com/nelenkov/android-backup-extractor
[pypi-pyaes]: https://pypi.python.org/pypi/pyaes
[gplv3]: https://www.gnu.org/licenses/gpl-3.0.html
