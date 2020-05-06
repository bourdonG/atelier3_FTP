import ftplib as FTP
from ftplib import FTP
from getpass import getpass

host = "192.168.1.212"
ftp = FTP('192.168.1.212', 'user', 'testtest')

# Connexion
print ("Connexion a " +host)
etat = ftp.getwelcome()
print ("Etat : ",etat)
#input("------------")

# Liste des répertoires distant
print(ftp.dir())

