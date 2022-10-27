```python
import pandas as pd
df=pd.read_excel("pupils.xlsx")
s=df["age"]
s[2] ###renvoie l'age d'indice 3
###pour selectionner directement la personne dont on veut l'âge
df=df.set_index("name")
s["carol"] ###renvoie 14
df["weight"]=[25,40,45,17,32] #pour rajouter une colonne de poids
df.types #renvoie les types de données dans les colonnes
dtype=("age": np.int64)
df["IMC"]=df["weight"]/df["height"]
df.loc["Carol","age"]
df.loc[:,"age"]
#df.loc[abscisse,ordonnée] les arguments peuvent être une liste un tableau un seul élément selon ce que l'on veut séléctionner
#df.iloc[0,2] cherchl'info en oubliant les indexs
```


