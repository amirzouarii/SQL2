🧍 Table CLIENT
sql
Copier
Modifier
INSERT INTO CLIENT (ID_CLIENT, NOM, PRENOM, ADRESSE, TELEPHONE) VALUES
  (1, 'Dupont', 'Jean', '10 rue des Lilas', '0123456789'),
  (2, 'Martin', 'Claire', '25 avenue de Paris', '0987654321'),
  (3, 'Bernard', 'Luc', '5 boulevard Haussmann', '0678123456');
📦 Table PRODUIT
sql
Copier
Modifier
INSERT INTO PRODUIT (ID_PRODUIT, NOM_PRODUIT, PRIX, CATEGORIE) VALUES
  (101, 'Chaise', 49.99, 'Mobilier'),
  (102, 'Table', 89.50, 'Mobilier'),
  (103, 'Lampe', 29.90, 'Éclairage');
🧾 Table COMMANDE
sql
Copier
Modifier
INSERT INTO COMMANDE (ID_COMMANDE, ID_CLIENT, DATE_COMMANDE) VALUES
  (1001, 1, TO_DATE('2023-10-01', 'YYYY-MM-DD')),
  (1002, 2, TO_DATE('2023-10-05', 'YYYY-MM-DD')),
  (1003, 3, TO_DATE('2023-10-10', 'YYYY-MM-DD'));
📋 Table LIGNE_COMMANDE
sql
Copier
Modifier
INSERT INTO LIGNE_COMMANDE (ID_COMMANDE, ID_PRODUIT, QUANTITE) VALUES
  (1001, 101, 2),
  (1001, 103, 1),
  (1002, 102, 1),
  (1003, 101, 4),
  (1003, 103, 2);
