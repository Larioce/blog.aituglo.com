---
title: HTB | Lame
subtitle: Writeup Lame
category:
  - HTB Writeups
author: Cassim Khouani
date: 2020-02-06T13:28:03.595Z
featureImage: /uploads/Screenshot-2019-08-01-at-20.39.48.png
---
La box Lame est considéré comme l'une des box les plus simple à craquer, c'est donc pour cela que je commence par celle ci.

On commence tout d'abord par faire l'énumération avec nmap. On remarque qu'il y a sur le serveur un serveur smb et un serveur sftpd.

![](/uploads/nmap.png "Nmap scan")

On essaye tout d'abord avec sftpd, et j'ai fait un recherche sur searchsploit.

![](/uploads/searchsploit.png "Searchsploit")

Il existe un exploit metasploit pour cette version, j'essaye donc de l'utiliser mais j'ai une erreur, l'exploit a dû être fixé.

![](/uploads/error.png "Error Metasploit")

Je passe donc à Samba et il existe aussi un exploit metasploit. Mais ce coup ci, Bingo cela fonctionne et je suis directement root.

![](/uploads/final.png "Resultat")



Finalement cette machine était vraiment facile et ne nécessite que très peu de réflexion.
