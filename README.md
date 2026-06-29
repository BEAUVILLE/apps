[README(26).md](https://github.com/user-attachments/files/29450272/README.26.md)# DIGIY APPS — Les bras numériques du terrain

Ce dépôt sert la page publique :

```txt
https://apps.digiylyfe.com/
```

## Rôle de cette page

`apps.digiylyfe.com` est une façade publique qui rassemble les portes utiles DIGIYLYFE :

- HUB DIGIY
- DRIVER
- LOC
- RESTO
- RESA
- MARKET
- BUILD
- JOBS
- PAY
- Espace Pro
- Activation module

Cette URL ne doit pas ouvrir un backoffice, un cockpit privé ou une porte admin.

## Doctrine

DIGIYLYFE ouvre les bras numériques du terrain :

- contact direct
- QR direct
- réservation directe
- paiement direct au professionnel
- 0% commission
- 0% dépendance
- le professionnel garde son client et son argent

## Séparation importante

```txt
apps.digiylyfe.com       = page publique des applications DIGIY
backoffice.digiylyfe.com = espace admin privé
digiy-hub.digiylyfe.com  = rond-point principal du terrain
```

Le backoffice doit rester privé et en `noindex`.

La page APPS, elle, peut être indexée par Google car elle sert de porte publique propre.

## DNS recommandé

Pour GitHub Pages, le DNS doit pointer vers :

```txt
CNAME  apps  BEAUVILLE.github.io
```

Ne pas garder en même temps :

```txt
A  apps  72.61.199.43
```

Un sous-domaine ne doit pas avoir à la fois un `A` et un `CNAME`.

## Fichier CNAME

Dans le dépôt GitHub Pages, créer un fichier `CNAME` contenant exactement :

```txt
apps.digiylyfe.com
```

## Fichiers du dépôt

```txt
index.html
README.md
CNAME
```

## Test après déploiement

Après push GitHub et mise à jour DNS :

```txt
https://apps.digiylyfe.com/?v=apps-public-ok
```

La page doit afficher :

```txt
DIGIY APPS — Les bras numériques du terrain
```

et ne doit plus afficher :

```txt
DIGIY Backoffice — Login
PIN + Token
```

## Signature

DIGIYLYFE ∞  
Le terrain garde la main.

