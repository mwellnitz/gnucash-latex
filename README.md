gnucash-latex
=============

Create good looking invoices for gnucash using latex and python

## Marcus Wellnitz (MWE) 2014-10-19
## Die in dieser Distribution von mir vorgenommenen Änderungen sind Public domain. 
## Bitte beachten: Die Rechte Anderer Autoren sind entsprechend gekennzeichnet (Quellcode)

Install latex environment and gnucash-python
* for Ubuntu 14.04: sudo aptitude install texlive-latex-base texlive-latex-recommended python-gnucash texlive-lang-german pdflatex ipython

Change for your needs:
* latex_invoices.py: scroll down to 'def main' and change input_url = '' to your gnucash connections (file, mysql, etc.) for MySQL it's mysql://\<USERNAME>:\<PASSWORD>@\<SERVER>/\<DATABASE>
* Replace Benjamin_Franklein.pdf with your signature (source:https://commons.wikimedia.org/wiki/File:Autograph_of_Benjamin_Franklin.svg)
* adapt company.lco to fit your needs

Run as follows:
python latex_invoices.py -l 
python latex_invoices.py -n <YOUR_INVOICE_NO>
