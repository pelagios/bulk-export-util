# Recogito Bulk Export Utility

A Python commandline script for bulk-exporting annotations from a Recogito account.

## Configure

1. Create a copy of the file `config.py.template` named `config.py`.
2. Replace the dummy account details in `config.py` with your own Recogito username and password. Keep in mind that Recogito username and password are case-sensitive!
   - To bulk-export annotations from documents __in a specific folder__, specify the folder ID in `config.py`
   - To bulk-export annotations from __all documents from this account__, leave the value on the `DOWNLOAD_FOLDER` config property as `False`

## Bulk Download

Run the download script with `python download.py`. The Script requires Python 3 installed on your system. After completion, the annotations will be in the download-folder configured in `config.py`, in both JSON-LD and CSV format.
