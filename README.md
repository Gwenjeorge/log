Sur Ubuntu :  
Lancer un serveur Apache :  
`systemctl start apache2`  

A partir de l'host en bridge, vous connecter via un navigateur au serveur Apache sur http://<IP_VM_UBUNTU>.  

![log](/log/Loggin.png)  

Sur le serveur Apache, seul l'index existe, rentrer aléatoirement un /... après l'adresse pour générer une erreur 404.   

![log](/log/NotFound.png)  

Dans le journalct nous pouvons observer le démarrage du serveur Apache.  

![log](/log/log1.png)  

Dans `/var/log/apache2/access_log` on peut observer :  
L'ip qui se connecte, en l'occurence 172.16.149.31 (mon host).  
Les requêtes générées en rafraichissant la page.  
Les erreurs 404.  

![log](/log/log2.png)  


