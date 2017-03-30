=====================
scrapy-dotpersistence
=====================

Scrapy extension to sync `.scrapy` folder to an S3 bucket.

Installation
============

You can install scrapy-dotpersistence using pip::

    pip install scrapy-dotpersistence

You can then enable the extension in your `settings.py`::

    EXTENSIONS = {
        ...
        'scrapy_dotpersistence.DotScrapyPersistence': 0
    }

How to use it
=============

Enable extension through `settings.py`::

    DOTSCRAPY_ENABLED = True

Configure the exension through `settings.py`::

    DOTSCRAPY_AWS_ACCESS_KEY_ID = "ABC"
    DOTSCRAPY_AWS_SECRET_ACCESS_KEY = "DEF"
    DOTSCRAPY_S3_FOLDER = "foldername"
    DOTSCRAPY_S3_BUCKET = "test-bucket-name"

You can change a dotpersistence folder path with environ::

    export DOTSCRAPY_DIR='/tmp/.scrapy'
