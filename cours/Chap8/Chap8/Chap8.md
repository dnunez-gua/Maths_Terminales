[Retour](../../Chap.md)
# Orthogonalité dans l'espace

## Méthodes 
**Méthode1** : Connaitre les formules du produit scalaire :  
- $\vec{u}.\vec{v}=\left\lVert \vec{u}\right\rVert \times \left\lVert \vec{v}\right\rVert\times \cos(\vec{u},\vec{v})$  
- $\overrightarrow{AB}.\overrightarrow{AC}= AB\times AH$ si $(\overrightarrow{AB},\overrightarrow{AC})\in [-\dfrac{\pi}{2}; \dfrac{\pi}{2}]$

$=-AB\times AH$ sinon.  
Avec H le projeté orthogonal de C sur (AB)  
- Formules de polarisation :  
$\vec{u}.\vec{v}=\dfrac{1}{2}[\left\lVert \vec{u}\right\rVert^2 + \left\lVert \vec{v}\right\rVert^2-\left\lVert \vec{u}-\vec{v}\right\rVert^2]$  
$\vec{u}.\vec{v}=\dfrac{1}{2}[-\left\lVert \vec{u}\right\rVert^2 - \left\lVert \vec{v}\right\rVert^2+\left\lVert \vec{u}+\vec{v}\right\rVert^2]$

**Méthode 2** : Un plan a pour équation cartésienne $ax+by+cz+d=0$ avec le vecteur normal  
$\vec{n}=(a,b,c)$

**Méthode 3:** Trouver les intersections de droites et plans, intersection de plans, intersection de sphère et plan.   
Projection orthogonal d'un point sur un plan  
Distance d'un point à un plan.
    
## Cours 
[cours Chap8](./Cours-Chap8.pdf){:target="_blank"}  

## Démonstrations

!!! note "Equation cartésienne du plan :" 
    === "Propriété : " 
         Un plan a pour équation cartésienne $ax+by+cz+d=0$ avec le vecteur normal  $\vec{n}=(a,b,c)$  
    === "Démonstration :"
        $\vec{n}$ est normal au plan P contenant le point A. Donc pour tout $M(x,y,z)$ du plan P, le produit scalaire $\overrightarrow{AM}.\vec{n}=0$  
        $a(x-x_A)+b(y-y_A)+c(z-z_A)=0 \Leftrightarrow ax+by+cz-(ax_A+by_A+cz_A)=0$.  
        En posant $d=-(ax_A+by_A+cz_A)$ on a bien l'équation cartésienne de P:  $ax+by+cz+d=0$

!!! note "Distance et projeté :" 
    === "Propriété : " 
        Si H est le projeté orthogonal de A sur un plan P, alors la distance de A à P est AH.
    === "Démonstration :" 
        Soit M un point du plan différent de H. Le triangle AHM est rectangle en H, donc l'hypoténuse AM>AH. Ainsi AH est la plus petite longueur de A au plan P.
## Exercices

!!! question " Produit scalaire analytique :"
    === "Exercices :" 
         N°22-30 p102  
         N°64-65 p105  
         N°79 p107
    === "Corrigés :"  
         [22-30](./corr/22-30.pdf){:target="_blank"}  
         [64-65](./corr/64.65.pdf){:target="_blank"}  
         [79](./corr/79.pdf){:target="_blank"}   
    === "Exercices :" 
         N°34-36 p103  
         N°66 p105  
         N°74-75 p106       
    === "Corrigés :"  
        [34-36](./corr/34-36.pdf){:target="_blank"}  
        [66](./corr/66.pdf){:target="_blank"}  
        [74-75](./corr/74-75.pdf){:target="_blank"}  
        
!!! question "Calcul d'angles :"
    === "Exercices"
        N°29-28-27 p105  
        N°53-54-57 p106  
    === "Corrigés"  
          [29-28-27](./corr/29-28-27.pdf){:target="_blank"}  
           [53-54-57](./corr/53-54-57.pdf){:target="_blank"}  

!!! question "Projection orthogonale - Distance à un plan :"
    === "Exercices" 
        N°38-39-40-42-43 p106  
        N°89 p108  
        N°100 p109  
        
    === "Corrigés"  
        [38-39-40-42-43](./corr/38-39-40-42-43.pdf){:target="_blank"}  

!!! question "Equations de sphères - Intersection de plans :"
    === "Exercices" 
        N°44-45 p106  
        N°110 p112  
        Intersection de plans :   
        N°83p108  
        N°106 p111  
    === "Corrigés"  
        [44-45](./corr/44-45.pdf){:target="_blank"}  
        [110](./corr/110.pdf){:target="_blank"} 
        [83](./corr/83.pdf){:target="_blank"} 
        [106](./corr/106.pdf){:target="_blank"} 



!!! question "Problèmes :"
    === "Exercices" 
        N°105p 110
        N°117 p115  
    === "Corrigés"  
          A venir
