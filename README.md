django-publications
===================

A Django app for managing scientific publications.


Features
--------

* automatically creates lists for individual authors and keywords
* BibTex import/export
* RIS export (EndNote, Reference Manager)
* unAPI support (Zotero)
* customizable publication categories/BibTex entry types
* PDF upload
* RSS feeds
* support for images

Requirements
------------

* Python >= 3.5.0
* Django >= 2.1.0
* Pillow >= 2.3.0

Installation
------------

1) Run `pip install django-publications`.

2) Add `'publications'` to `INSTALLED_APPS` in your project's `settings.py`.

3) Add the following to your project's `urls.py`:

	```python
	url(r'^publications/', include('publications.urls')),
	```

4) Run the following:

	```
	./manage.py makemigrations publications
	./manage.py migrate
	```
