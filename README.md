# Compte rendu du TP3

Objectif :

Le but de ce TP est de découvrir l'integration numérique en utilisant:
* La méthode des réctangles.
* La méthode des trapèzes.
* La méthode de Simpson.

# La méthode des réctangles

L’idée est d’interpoler g (avec g(t) = f(a+b/2 +b−a/2 * t), t∈[−1,1] )par un polynôme de degré 0, ce qui signifie qu’on remplace g par une fonction c constante. Reste à choisir la valeur de cette constante. 
(i) rectangles à gauche : c := f(−1); 
(ii) rectangles à droite : c := f(1); 
(iii) rectangles centrés : c = f(0). 
Cela conduit aux formules 
integde 1 à −1 de g(t) dt = 2g(−1) ou 2g(1) ou 2g(0). 

On pourrait aussi prendr en’importe quel point dans l’intervalle comme référence au lieu des extré-mitésouducentre,évidemment.

# La méthode des trapèzes

On remplace g par un polynôme d’interpolation de degré 1, passant aux extrémités. 
La formule donne :
integ de 1 à −1 de g(t)dt ~= g(−1)+g(1).
Là aussi,on pourrait choisir d’autres points d’interpolation que les deux extrémités.

# La méthode de Simpson

On remplace g par un polynôme d’interpolation de degré 2, c’est-à-direqu’on remplace g par une parabole coïncidant avec g aux point −1, 0, 1. Le calcul montre alors qu’on aboutit à laformule :
integ de 1 à −1 de g(t)dt ~= 1/3g(−1)+4/3g(0)+1/3g(1).


# Conclusion

Pour conclure,l'intégraltion numérique est une méthode pour calculer une valeur approximative dune fonction qui est compliqueé d'une autre coté l'intégration numérique permet destimé l'intégrale de cette fonction par la méthode d'interpolation avec certain erreur.
