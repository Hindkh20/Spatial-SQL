# Base de Données Spatiale
# Base de Données Spatiale

**Base de données spatiale**  
**Pr Hatim Lechgar**  
**SIG-3**  
**2024-2025**

## TD-1 : Installation de PostGIS et création d’une BD spatiale

### 1. Download et Install PostgreSQL
- Accédez à la [page de téléchargement de PostgreSQL](https://www.postgresql.org/download/) pour télécharger la dernière version de PostgreSQL adaptée à votre système d'exploitation (Linux, MacOS, Windows, BSD, Solaris).
- Suivez le guide d'installation pour installer le logiciel.
- Définissez un mot de passe pour l'utilisateur `Postgres` lors de l'installation. **Note : Utilisez un mot de passe facile à retenir.**

### 2. Download et Install PostGIS
- Lors de l'installation de PostgreSQL, cochez tous les composants nécessaires (y compris **Stack Builder**).
- Lancez **Stack Builder** pour télécharger PostGIS.
- Sélectionnez la version de PostgreSQL correspondante, et téléchargez PostGIS.
- Une fois l'installation terminée, cliquez sur **Fermer**.

### 3. Create a Database using PgAdmin 4
- Lancez **pgAdmin** et connectez-vous avec le mot de passe défini pour `Postgres`.
- Développez `Servers` > Faites un clic droit sur PostgreSQL > **Create** > **Database**.
- Donnez un nom à votre base de données, comme `spatial-db-1`, puis cliquez sur **Save**.
- Développez `Databases`, accédez à votre nouvelle base, et ajoutez l'extension PostGIS avec la commande suivante dans **Query Tool** :
  ```sql
  CREATE EXTENSION postgis;
