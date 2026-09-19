# Starklingnet stop wuauserv
net stop cryptSvc
net stop bits
net stop msiserver


ren %systemroot%\SoftwareDistribution SoftwareDistribution.old
ren %systemroot%\System32\catroot2 catroot2.old

net start wuauserv
net start cryptSvc
net start bits
net start msiserver
