[Retour](../../Chap.md)
# Suites Numériques

## Progression
!!! info "Méthodes" 
    **Méthode 1** : Une suite $(u_n)$ a pour limite $l$ lorsque, pour tout $\epsilon$ on peut trouver un rang $n_0$ à partir duquel $l-\epsilon < u_n < l+\epsilon$.   
    Cela permet de :
    - montrer qu'une suite converge vers un réel $l$.  
    - Etudier le comportement asymptotique d'une suite, notamment dans la modélisation de problème.  
    **Méthode 2** : Une suite $(u_n)$ a pour limite $+\infty$ lorsque, pour tout $A$ on peut trouver un rang $n_0$ à partir duquel $u_n > A$.  
    Une suite $(u_n)$ a pour limite $-\infty$ lorsque, pour tout $B$ on peut trouver un rang $n_0$ à partir duquel $u_n < B$.  
    Cela permet de : 
    - montrer qu'une suite diverge.  
    - Etudier le comportement asymptotique d'une suite, notamment dans la modélisation de problème.   
    **Méthode 3** : Les limites de suites usuelles et les tableaux d'opérations sur les limites sont à connaitre.  
    **Méthode 4** : Théorèmes de comparaison, théorème des gendarmes.  
    **Méthode 5**: Théorème des convergences monotone : Toute suite croissante majorée converge. Toute suite décroissante minorée converge.
    **Méthode 6** : Démonstration par récurrence :  
    - Initialisation : Montrer qu'une propriété est vraie au rang 0 ou 1 (ou $n_0$).  
    - Hypothèse de récurrence : On suppose qu'il existe un $k$ entier plus grand que $n_0$ telque la propriété est vraie au rang $k$.  
    - Hérédité : On montre que la propriété est vraie au rang $k+1$.  
    - Conclusion : pour tout n, la propriété est vraie.  
    
    
    
## Cours 
[cours Chap2](./Cours-chap2.pdf){:target="_blank"}

## Rappels principaux  

!!! info " Sens de variations d'une suite" 
    === "Méthode 1" 
        Calculer $u_{n+1}-u_n$ et étudier son signe.  
        - Si $u_{n+1}-u_n<0$ alors la suite est décroissante  
        - Si $u_{n+1}-u_n>0$ alors la suite est croissante  
        
    === "Méthode 2" 
        Calculer $\dfrac{u_{n+1}}{u_n}$ et étudier son signe.  
        - Si $\dfrac{u_{n+1}}{u_n}<1$ alors la suite est décroissante  
        - Si $\dfrac{u_{n+1}}{u_n}>1$ alors la suite est croissante  
    
    === "Méthode 3" 
        Etudier la fonction $f$ telle que $f(x)=u_n$.  
        - Si $f$ est décroissante alors la suite $u_n$ est décroissante  
        - Si $f$ est croissante alors la suite $u_n$ est croissante  
        ATTENTION : ne pas confondre $u_n = f(n)$ et $u_{n+1}=f(u_n)$. Cette méthode ne s'appliquerait pas dans ce cas.  

!!! info "Nature d'une suite "
    === "Suites arithmétiques "
        - Définition :$u_n$ est une suite arithmétique de raison $r$ si $\forall n \in \mathbb{N}, u_{n+1}=u_n+r$  
        - Propriété : Si $u_n$ est une suite arithmétique de raison $r$ et premier terme $u_0$ alors $\forall n \in \mathbb{N}, u_n=u_0+nr$  
        - Remarque : si $u_n$ a pour premier terme $u_1$ alors $\forall n \in \mathbb{N}, u_n=u_1+(n-1)r$  
        
    === "Suites géométriques "
        - Définition :$u_n$ est une suite géométrique de raison $q$ si $\forall n \in \mathbb{N}, u_{n+1}=u_n\times q$  
        - Propriété : Si $u_n$ est une suite géométrique de raison $q$ et premier terme $u_0$ alors $\forall n \in \mathbb{N}, u_n=u_0\times q^n$  
        - Remarque : si $u_n$ a pour premier terme $u_1$ alors $\forall n \in \mathbb{N}, u_n=u_1\times q^{n-1}$  
        
        
## Démonstrations Chapitre 2
!!! attention "Démonstration "
    === "Propriété : "
        Toute suite croissante non majorée diverge

    ===  "Démonstration :"
        Soit une suite $u_n$, une suite croissante et un réel $A>0$.<br>
        $u_n$ est non majorée donc, il existe un rang $n_0$ tel que $u_{n_0}>A$<br>
        $u_n$ est croissante donc pour tout $n>n_0$ on a $u_n>u_{n_0}$<br>
        On a donc montré que pour A>0 donné, il existe $n_0$ tel que pour tout $n>n_0$ on a $u_n>A$<br>
        ce qui est la définition de <br>
        $\displaystyle\lim_{n\to +\infty}{u_n}=+\infty$
        
        <br>
        **CQFD**

!!! attention "Démonstration "
    === " Théorème de comparaison :" 
        Toute suite majorée par une suite divergente, diverge
    === " Démonstration :"
        Soit deux suites $u_n$ et $v_n$ telles que à partir d'un rang $n_0$ on a $u_n\leq v_n$ <br>
        On a $\displaystyle\lim_{n\to +\infty}{u_n}=+\infty$ donc pour $A>0$ réel donné, il existe $n_1>0$ tel que $\forall n>n_1$ on a $u_n>A$<br>
        Donc pour tout $n>max(n_0,n_1)$ on a $v_n>u_n>A$ donc $\displaystyle\lim_{n\to +\infty}{v_n}=+\infty$
        <br>
        **CQFD**
    
!!! attention "Démonstration "
    === "Propriété : "
        Si $q>1$, alors $\displaystyle\lim_{n\to +\infty}{q^n}=+\infty$
    === "Pré-requis : "
        - Inégalité de Bernouilli : $\forall a>0, \forall n\geq 0, (1+a)^n>1+na$ <br>
        - Propriétés de comparaison

    ===  "Démonstration :"
        $q>1$ donc il existe un réel $a>0$ tel que $q=1+a$ <br>
        $q^n=(1+a)^n>1+na$ <br>
        Or $\displaystyle \lim_{n\to +\infty}{1+na}=+\infty$ donc par comparaison <br>
        $\displaystyle \lim_{n\to +\infty}{q^n}=+\infty$ 
    
        
        <br>
        **CQFD**
        


## Exercices 

!!! example "Pré-requis :" 
    N°1 page 126<br>
    N°2 page 126<br>
    N°3 page 126<br>
    N°6 page 126<br>

!!! question "Démonstration par récurrence :"
    === "Exercices :" 
        N°48 p27 (10 minutes)<br>
        N°49 p27 (15 minutes)<br>
        N°54 p27 (15 minutes)<br>
    === "Correction :"
        l'exercice 54 est la démonstration de l'inégalité de Bernoulli faite dans le cours  
        [49p27](./corr/49p27.pdf){:target="_blank"}  

!!! question "Opérations sur les limites :"
    === "Exercices :"
        N°25 page 145 (15 minutes) <br>
        N°27 page 145 (15 minutes) <br>
        N°31 page 145 (15 minutes) <br>
    === "Correction : "
        [25-27-31](./corr/25-27-31.pdf){:target="_blank"}

!!! question "Limites finies :"
    === "Exercices : "
        N°51p148 (20 minutes)<br>
        N°49p147 (20 minutes)  
    === "Correction : "
        [51-49](./corr/51-49.pdf){:target="_blank"}  


!!! question "Problèmes : "
    === "Exercices : "
        N°94 p153   
        N°73 p150
        
    === "Correction : "
         [94](./corr/94.pdf){:target="_blank"}  
         [73](./corr/73.pdf){:target="_blank"}

!!! note "Travail de groupe :"
    === "Indications :"
        [Courbe](./105-courbe.pdf)  
        [Tracer les termes d'une suite](https://www.youtube.com/watch?v=vsi4JWESSH0)  
    === "Correction :"
        [105](./corr/105.pdf){:target="_blank"}  
!!! info "Algorithme "
    TP Python seuil- suite
