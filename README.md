# HFC

    Histogram Fuzzy Colour Filter (HFC) 


    Schulte Stefan, De Witte Valérie, Nachtegael Mike, Van Der Weken Dietrich and Kerre Etienne E. Histogram-based fuzzy colour filter for image restoration. Image and Vision Computing in press. 2007 

    Download the zip file here.


    Unzip the file into a certain directory.


    You have to add the folder to the current MATLAB search path by using the commando: addpath('path'), with ‘path’ the directory followed by the new map '/HFC' which should be created.


    The HFC filter is executed by using the Matlab commando:

    Out = HFC(Noise,Org);
    where Noise is the noisy input colour image and Org is the noise-free colour original image.


    In order to overcome some problems of Matlab you have to know that we have implemented most files in C-code. The switching between Matlab and C in realized by the 'mex' (see Matlab help for more information). If you never have used mex files before you probably have to do the following thinks:

    cd 'C:\Directory\'
    the current directory has to be changed to that map that was created in the first step

    mex –setup
    => Choose a compiler

    mex HFC1.c
    mex Detection2.c
    mex Detection3.c 
