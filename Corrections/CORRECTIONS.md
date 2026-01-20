# Élements de corrections

## Séance 2.

### Questions

- Il manque quelques éléments.

### Code

- Problème d'encodage !

- **Question 12.** Je n'arrive pas à comprendre pourquoi votre code ne marche pas.

## Séance 3.

### Questions

- **Question 3.** La partie sur la moyenne n'est pas assez développée. Vous n'expliquez pas quand le mode est calculable.

- **Question 5.** L'écart à la moyenne peut être non nul.

### Code

- Excellent !

## Séance 4

### Questions

- Il manque beaucoup d'éléments.

### Code

- La bibliothèque `import matplotlib.pyplot as plt` n'a pas été importée.

- Pour exécuter le code, il faut remplacer `stats.` ... par `scipy.stats.` ... .

- Une fois corrigé, ça marche !

 -**Question 2.** partiellement répondue.

## Séance 5

### Questions

- Il manque quelques éléments.

### Code

- Où sont les commentaires demandés dans le rapport ?

- **Question 3.** Pour que le code fonctionne, il faut remplacer :

```
    data1 = pd.read_csv('./data/Loi-normale-Test-1.csv', header=None)[0]
    data2 = pd.read_csv('./data/Loi-normale-Test-2.csv', header=None)[0]
```

par :

```
    data1 = pd.DataFrame(ouvrirUnFichier('./data/Loi-normale-Test-1.csv'))
    data2 = pd.DataFrame(ouvrirUnFichier('./data/Loi-normale-Test-2.csv'))
```

Pour être certain que ça marche, il faut écrire juste après :

```    
    stat1,p1 = scipy.stats.shapiro(data1['Test'])
    stat2,p2 = scipy.stats.shapiro(data2['Test'])
```

## Séance 6

### Questions

- Il manque quelques éléments.

### Code

- Où sont les commentaires demandés dans le rapport ?

- Les tests sont faux. En utilisant vos variables, il faut écrire :

```
    spearman_pop = scipy.stats.spearmanr(rank_pop2007, rank_pop2025)
    kendall_pop = scipy.stats.kendalltau(rank_pop2007, rank_pop2025)

    spearman_dens = scipy.stats.spearmanr(rank_dens2007, rank_dens2025)
    kendall_dens = scipy.stats.kendalltau(rank_dens2007, rank_dens2025)
```

## Humanités numériques

- Aucune analyse rendue.

## Remarques générales

- Aucun dépôt régulier sur `GitHub`.
