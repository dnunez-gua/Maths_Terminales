[Retour](../../Chap.md)
# Compléments sur les dérivées

## Progression
!!! info "Méthodes"
    **Méthode 1**: Soient $u$ une fonction définie et  dérivable sur un intervalle I à valeurs dans J, et $v$ une fonction définie et dérivable sur J. Alors la fonction $v°u$ est dérivable sur I. et pour tout $x_0 \in I, (v° u)'(x_0)=u'(x_0)\times (v'° u)$  
    **Méthode 2** : Soit $f$ une fonction dérivable sur I, f est convexe si et seulement si $f'$ est croissante sur I.  Cela permet de :   
    - déterminer la convexité d'une fonction.  
    - étudier la position de la courbe par rapport à ses sécantes ou ses tangentes  
    - déterminer les points d'inflexion  
    **Méthode 3** : Soit $f$ dérivable sur I et $f'$ dérivable sur I. $f$ est convexe sur I si et seulement si $f''$ est positive sur I. Cela permet de :   
    - déterminer la convexité d'une fonction.  
    - étudier la position de la courbe par rapport à ses sécantes ou ses tangentes  
    - déterminer les points d'inflexion  
    
## Démonstrations Chapitre 4
!!! attention "Démonstration "
    === "Propriété : "  
         $f''(x)>0$ sur un intervalle I $\Leftrightarrow \mathcal{C}_f$ est au-dessus de ses tangentes  
    ===  "Démonstration :"  
        Soit $T_a$ la tangente à $\mathcal{C}_f$ au point d'abscisse $a$ avec $T_a:y=f'(a)(x-a)+f(a)$.  
        On note $\phi$ la fonction définie par $\phi(x)=f(x)-y=f(x)-(f'(a)(x-a)+f(a))=f(x)-f'(a)(x-a)-f(a)$.  
        $\phi$ est deux fois dérivable, $\phi'(x)=f'(x)-f'(a)$ (les autres termes de $\phi$ étant des constantes).  
        Donc $\phi''(x)=f''(x)>0$ donc $\phi'$ est croissante sur I. 
        
        - Si $x>a \Leftrightarrow \phi'(x)>\phi'(a)$ avec $\phi'(a)=f'(a)-f'(a)=0$ donc $\phi'(x)>0 \Leftrightarrow \phi$ est croissante sur I, donc $\phi(x)>\phi(a)$ avec $\phi(a)=0$.  
        Ainsi $\phi(x)>0 \Leftrightarrow f(x)-y>0 \Leftrightarrow f(x)>y$ donc $\mathcal{C}_f$ est au-dessus de ses tangentes.  
        
        - Si $x<a \Leftrightarrow \phi'(x)< \phi'(a) \Leftrightarrow \phi'(x)<0$  donc $\phi(x)$ est décroissante. Donc $x<a \Leftrightarrow \phi(x)> \phi(a) \Leftrightarrow \phi(x)>0$.  
        Ainsi $f(x)-y>0 \Leftrightarrow f(x)>y$ donc $\mathcal{C}_f$ est au-dessus de ses tangentes.
## Cours 
[cours Chap4](./Cours-chap4.pdf){:target="_blank"}
## Rappels de première
!!! question "Rappels  :"
    === "Nombre dérivé "
        Le nombre dérivé $f'(a)$ est le coefficient directeur de la tangente à $\mathcal{C}_f$ au point d'abscisse $a$.  
        Ex1 du cours  
        N°1 p210  
    === "Correction :" 
        [Ex 1](./corr/1.pdf){:target="_blank"}
        
## Exercices 

        
!!! question "Des nouvelles formules de dérivées :"
    === "Exercices :" 
        Activité A p 212  
        N°21-23-24-25-26p222  
        N°43-45 p224  
    === "Correction :" 
        [Ex 21-23-24-25-26](./corr/21-23-24-25-26.pdf){:target="_blank"}  
        [Ex 43-45](./corr/43-45.pdf){:target="_blank"}  


!!! question " Dérivées secondes - Convexité :"
    === "Exercices :"
        N°5p210
        Activtés B p212  
        Interprétation graphique de la convexité  
        N°31p222  
        N°32p222  
        Lien entre dérivées et convexité  
        N°70p227    
        N°71p227  
        N°75-76-77 p228  
        N°53p225
    === "Correction : "
        [Ex 70](./corr/70.pdf){:target="_blank"}  
        [Ex 53](./corr/53.pdf){:target="_blank"}  
        [Ex 31](./corr/31.pdf){:target="_blank"}  
        [Ex 71](./corr/71.pdf){:target="_blank"}  
        [Ex 32](./corr/32.pdf){:target="_blank"}  
        [Ex 75-76-77](./corr/75-76-77.pdf){:target="_blank"}  
