# Conception de réseau sécurisé pour MboaTech SARL
  Présentation du projetCe projet concerne la mise en place d'une infrastructure réseau sécurisée pour l'entreprise MboaTech SARL, basée à Yaoundé. L'objectif est de segmenter le réseau pour 45 employés répartis dans différents départements afin d'optimiser la gestion et la sécurité des flux de données..  

# Outils utilisé 
  Cisco Packet Tracer pour la simulation.  
  Git et GitHub pour le versionnement et le dépôt du projet.  
  Editeur de texte pour la rédaction de la documentation technique.  

# Architecture Réseau
Le réseau utilise une topologie de routage inter-VLAN basée sur un routeur principal et plusieurs commutateurs. Cette configuration permet de séparer les flux de communication entre les services. 

# Plan d'adressage
  IPVLAN 10 (ADMIN) : 192.168.10.0/24 (Passerelle : 192.168.10.1).  
  VLAN 20 (DEV) : 192.168.20.0/24 (Passerelle : 192.168.20.1).  
  VLAN 30 (SUPPORT) : 192.168.30.0/24 (Passerelle : 192.168.30.1).  
  VLAN 40 (INVITÉ) : 192.168.40.0/24 (Passerelle : 192.168.40.1).  
  VLAN 50 (SERVEURS) : 192.168.50.0/24 (Passerelle : 192.168.50.1).  

# Règles de sécurité (ACL)
Les listes de contrôle d'accès (ACL) ont été configurées sur le routeur pour appliquer les restrictions suivantes: 
  Le VLAN ADMIN dispose d'un accès complet à l'ensemble des serveurs.  
  Le VLAN DEV peut uniquement accéder au serveur d'application et au serveur web.  
  Le VLAN SUPPORT est limité à l'accès au serveur web uniquement.  
  Le VLAN GUEST est totalement isolé des serveurs internes et peut uniquement accéder à Internet.. 
  
# Travail réalisé
  Configuration des VLAN et du routage inter-VLAN. 
  Mise en place d'un serveur DHCP pour l'attribution automatique des adresses IP.  
  Implémentation des ACL pour le filtrage du trafic.  
  Tests de connectivité via des commandes ping et vérification de l'accès aux services web. 
  VivablesFichier de simulation .pkt fonctionnel.  Documentation technique détaillée. 
  Captures d'écran des tests de connectivite réussies et des accès bloqués. 
  
# Candidat :
​ Mvondo Nko'o Arnold Daniel
 Niveau : Licence 2 TIC
 Date : mai 2026  
