- 👋 Hi, I’m @Venomousking
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Venomousking/Venomousking is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
---
#!/usr/bin/python

import os                   # For operating system related call e.g [os.listdir()]
import sys


from PyQt4 import QtCore, QtGui

# Set Working directory'
if 'core' not in os.listdir(os.getcwd()):
    variable = sys.argv[0]
    direc = variable.replace('ghost.py',"")
    os.chdir(direc)

from gui import *

if __name__ == '__main__':
    app = QtGui.QApplication(sys.argv)
    run = ghost_phisher.Ghost_phisher()
    run.show()
    app.exec_()
    
