# -*- coding: utf-8 -*-
"""
Created on Wed Dec 12 14:51:49 2018

@author: UI
"""

import os
import os.path

# The path to the ui file
dir = './'

# List all UI files in the directory
def listUiFile():
    list = []
    #List all files in the current directory
    files = os.listdir(dir)
    #Filename fitter
    for filename in files:
        if os.path.splitext(filename)[1] == '.ui':
            list.append(filename)
    return list

# UI extension transformation
def transPyFile(filename):
    return os.path.splitext(filename)[0] + '.py'

#Convert files using system commands
def runMain():
    list = listUiFile()
    for uifile in list:
        cmd = "pyuic5 -o {uifile}".format(uifile=uifile)
        os.system(cmd)
if __name__ == "__main__":
    runMain()
