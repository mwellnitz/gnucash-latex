gnucash-latex
=============

Create good looking invoices for gnucash using latex and python

###### Marcus Wellnitz (MWE) 2014-10-19
###### Die in dieser Distribution von mir vorgenommenen Änderungen unterliegen, soweit nicht anders bezeichnet, der GNU General Public License. 
###### Bitte beachten: Die Rechte Anderer Autoren sind entsprechend gekennzeichnet (Quellcode)
###### 
###### All my changes are distributed under the terms of the GNU General Public License if no other license is named.
###### This is a collection of different tools. Some files have been licensed different.

Weitegehende Infos im Wiki: [https://github.com/mwellnitz/gnucash-latex/wiki]

##### Install latex environment and gnucash-python
* for Ubuntu 14.04: <code>sudo aptitude install texlive-latex-base texlive-latex-recommended python-gnucash texlive-lang-german pdflatex ipython</code>

##### Get this software package:
<code>git clone https://github.com/mwellnitz/gnucash-latex</code>

##### Change for your needs:
* latex_invoices.py: scroll down to 'def main' and change input_url = '' to your gnucash connections (file, mysql, etc.) for MySQL it's mysql://\<USERNAME>:\<PASSWORD>@\<SERVER>/\<DATABASE>
* Replace Benjamin_Franklein.pdf with your signature (source:https://commons.wikimedia.org/wiki/File:Autograph_of_Benjamin_Franklin.svg)
* adapt company.lco to fit your needs

##### Now you can start:
<code>python latex_invoices.py -l</code>

<code>python latex_invoices.py -n <YOUR_INVOICE_NO></code>
