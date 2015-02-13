PmagPy-Cookbook
===============

This repository contains the cookbook for installing and using PmagPy. The cookbook can be viewed as a webpage at: http://ltauxe.github.io/PmagPy-Cookbook/PmagPy.html or at http://earthref.org/PmagPy/cookbook/ where it is nicely presented in the earthref.org format. PmagPy is a software package written in Python that contains programs and function libraries used for the analysis and plotting of paleomagnetic and rock magnetic data. The PmagPy code is hosted here: https://github.com/ltauxe/PmagPy 

Project Information
---------------

This documentation of the PmagPy software is updated from that in the book entitled Essentials of Paleomagnetism by Tauxe et al., (2010). This cookbook was designed and written by Lisa Tauxe as a companion website to the the book Essentials of Paleomagnetism, 2nd Web Edition. Chapter references to this companion book are, for example, “Essentials Chapter X”.

The files in the cookbook were first added to this Github repository on January 14, 2014 and at that point represented a version of the cookbook that was last updated on May 24, 2013. The vast majority of the content was written and generated by Lisa Tauxe with contributions from other "chefs," in particular, the MagIC Database Team (Cathy Constable, Anthony Koppers, Rupert Minnett, Nick Jarboe, and Ron Shaar) and Nick Swanson-Hysell.

Generating the PDF and website after edits to the cookbook
---------------
1) Typeset PmagPy.tex in LaTEX with the customlinks import line commented and all of the \customlink lines commented to get a new PmagPy.pdf file

2) Uncomment the customlinks import line commented and all of the \customlink lines

3) Execute the htlatex command (this comes with standard latex distributions) as follows:

    % htlatex PmagPy "html,1,sections+"
    
4) This command will regenerate PmagPy.html and the .png files that are called upon in the .html

5) If this all works, you will have updated the webpage which can be checked locally by opening PmagPy.html in a browser. If satisfied with the results, commit the changes and synchronize with the master PmagPy-Cookbook branch. Github hosts the webpage through the gh-pages branch of the PmagPy-Cookbook. When changes are committed to the master branch they need to be merged into the gh-pages branch so they appear at: http://ltauxe.github.io/PmagPy-Cookbook/PmagPy.html This can be done readily in the Github app within the branches tab or with these commands:

    git checkout gh-pages
    git merge master
    git push origin gh-pages
    git checkout master
