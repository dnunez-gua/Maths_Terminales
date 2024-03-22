[Retour](../../Chap.md)
# Chapitre 1 - Limites de fonctions
## Progression
!!! info " Méthodes "
    **méthode 1** : $a$ désigne un nombre réel ou $+\infty$ ou $-\infty$. $f$ est une fonction définie au voisinage de $a$.
    - Dire que $f$ a pour limite $a$ quand $x$ tend vers $a$ (resp $+\infty$) signifie que, quelque soit le réel $A,f(x)>A$ dès que $x$ suffisamment proche de $a$)(resp. $x$ suffisamment grand). On écrit : $\displaystyle\lim_{x \to a} f(x)=+\infty$ (resp. $\displaystyle\lim_{x \to +\infty} f(x)=+\infty$).
    - De façon analoque : $\displaystyle\lim_{x \to -\infty} f(x)=+\infty$ ;  $\displaystyle\lim_{x \to +\infty} f(x)=-\infty$ ;  $\displaystyle\lim_{x \to -\infty} f(x)=-\infty$
    - Dire que $f$ a pour limite $l$ quand $x$ tend vers $a$ (resp $+\infty$) signifie que quelques soit $\epsilon>0; |f(x)-l|<\epsilon$ dès que $x$ suffisamment proche de $a$)(resp. $x$ suffisamment grand). On écrit $\displaystyle\lim_{x \to a} f(x)=l$ (resp. $\displaystyle\lim_{x \to +\infty} f(x)=l$).
    - Cela permet de :  
     Etudier le comportement de $f$ même lorsque la fonction n'est pas définie (pour une valeur interdite).  
     Déterminer des asymptotes
     
     **méthode 2** : Des théorèmes permettent de donner la limite d'une somme, d'un produit ou d'un quotient de fonctions. Les formes indéterminées sont de la forme $\infty -\infty$ ou $0\times \infty$ ou $\infty / \infty$ ou $0/0$. Il faudra transformer la fonction pour casser l'indetermination.  
     **méthode 3** : Si pour tout $x\in I, f(x)\geq g(x)$ et $\displaystyle\lim_{x \to +\infty} g(x)=+\infty$ alors $\displaystyle\lim_{x \to +\infty} f(x)=+\infty$  
     Si pour tout $x\in I, f(x)\leq g(x)$ et $\displaystyle\lim_{x \to +\infty} g(x)=-\infty$ alors $\displaystyle\lim_{x \to +\infty} f(x)=-\infty$  
     Si pour tout $x\in I, g(x)\leq f(x)\leq h(x)$ et $\displaystyle\lim_{x \to +\infty} g(x)=\displaystyle\lim_{x \to +\infty} h(x)=l$ alors $\displaystyle\lim_{x \to +\infty} f(x)=l$ (théorème des gendarmes)  
     **méthode 4** : $ \displaystyle\lim_{x \to +\infty} e^x=+\infty$ et $ \displaystyle\lim_{x \to -\infty} e^x=0$.
      Pour tout n entier $ \displaystyle\lim_{x \to +\infty} \dfrac{e^x}{x^n}=+\infty$ et $ \displaystyle\lim_{x \to -\infty} x^n.e^x=0$ (théorème des croissances comparées)
   
    
    
## Cours 

[cours Chap1](./Cours-Chap1.pdf){:target="_blank"}

### Démonstrations du chapitre 1
!!! attention "Démonstration de la limite de $e^x$ en $+\infty$"
    ===  "Propriété : "
        $$\displaystyle\lim_{x \to +\infty} {e^x}=+\infty$$
    
    ===  "Démonstration :"
        **Pré-requis : théorème de comparaison** <br>
        Soit la fonction $g$ définie sur $\mathbb{R}$ par $g(x)=e^x-x$ <br>
        $g$ est dérivable sur $\mathbb{R}$ et $g'(x)=e^x-1$ <br>
        $g'(x)>0 \Leftrightarrow x>0$. <br>
        $g$ admet donc un minimum en 0 qui vaut $g(0)=1$. Donc $g(x)>0$ pour tout $x\in \mathbb{R}$<br>
        Donc pour tout réel $x$, $e^x>x$ <br>
        Par comparaison: 
        $\displaystyle\lim_{x \to +\infty} {e^x}>\displaystyle\lim_{x \to +\infty} {x}$ <br>
        donc         $\displaystyle\lim_{x \to +\infty} {e^x}=+\infty$ **CQFD**
       
!!! attention  "Démonstration de la limite de $e^x$ en $-\infty$"  
    ===  "Propriété : "
        $$\displaystyle\lim_{x \to -\infty} {e^x}=0$$
    
    ===  "Démonstration :"
        **Pré-requis : limite en $+\infty$ et composition de limite** <br>
        $\displaystyle\lim_{x \to -\infty} {e^x}=\displaystyle\lim_{x \to +\infty} {e^{-x}}$<br>
        $=\displaystyle\lim_{x \to +\infty} \frac{1}{e^x}=0$ **CQFD**

!!! attention "Démonstration du théorème des croissances comparées"
    === "Théorème 1: "
        $\displaystyle\lim_{x \to +\infty} \frac{e^x}{x^n}=+\infty$
        
    === "Démonstration 1"
        **Pré-requis : Opérations sur les limites, composition de limites, théorème des gendarmes**<br>
        **Cas $n=1$**<br>
        Soit la fonction $g$ définie sur $\mathbb{R}$ par $g(x)=e^x-\frac{x^2}{2}$ <br>
        $g$ est dérivable sur $\mathbb{R}$ et $g'(x)=e^x-x$ <br>
        On a montré dans la démonstration de la limite de $e^x$ que $g'(x)>0$ donc $g$ est croissante sur $\mathbb{R}$.<br>
        donc $\forall x>0$, on a $g(x)>g(0) \Leftrightarrow g(x)>1>0$ donc $e^x>\frac{x^2}{2} \Rightarrow \frac{e^x}{x}>\frac{x}{2}$<br>
        Par comparaison, comme $\displaystyle\lim_{x \to +\infty} \frac{x}{2}=+\infty$ alors $\displaystyle\lim_{x \to +\infty} \frac{e^x}{x}=+\infty$ <br>
        
        **Cas $n> 1$** <br>
        $\frac{e^x}{x^n}=(\frac{e^{\frac{x}{n}}}{\frac{x}{n}})^n\times(\frac{1}{n})^n$<br>
        Posons $X=\frac{x}{n}$ alors $(\frac{e^{\frac{x}{n}}}{\frac{x}{n}})^n\times(\frac{1}{n})^n=(\frac{e^X}{X})^n\times(\frac{1}{n})^n$. <br>
        On a $\displaystyle\lim_{x \to +\infty}X=+\infty$ et on a vu que $\displaystyle\lim_{X \to +\infty} \frac{e^X}{X}=+\infty$ donc par produit $\displaystyle\lim_{X \to +\infty} \frac{e^X}{X}\times(\frac{1}{n})^n=+\infty$ <br>
        Et par composition on a         $\displaystyle\lim_{x \to +\infty} \frac{e^x}{x^n}=+\infty$
        **CQFD**
        
    === "Théorème 2 : "
        $\displaystyle\lim_{x \to -\infty} {x^n e^x}=0$
        
    === "Démonstration 2"
        **Pré-requis : Théorème 1, opérations sur les limites, composition de limites, théorème des gendarmes**<br>
        $x^n e^x=\frac{x^n}{e^{-x}}$ <br>
        $\displaystyle\lim_{x \to -\infty} {x^n e^x}=\displaystyle\lim_{x \to -\infty}\frac{x^n}{e^{-x}}=\displaystyle\lim_{x \to +\infty}\frac{(-x)^n}{e^{x}}=\displaystyle\lim_{x \to +\infty}(-1)^n\frac{x^n}{e^{x}}$<br>
        On sait que $\displaystyle\lim_{x \to +\infty} \frac{e^x}{x}=+\infty$ donc par inverse, $\displaystyle\lim_{x \to +\infty}\frac{x^n}{e^{x}}=0$. De plus, $-1\leq (-1)^n\leq 1$ donc $-\frac{x^n}{e^{x}}<(-1)^n\frac{x^n}{e^{x}}<\frac{x^n}{e^{x}}$ par produit $\displaystyle\lim_{x \to +\infty}-\frac{x^n}{e^{x}}=\displaystyle\lim_{x \to +\infty}\frac{x^n}{e^{x}}=0$<br>
        Donc par le théorème des gendarmes         $\displaystyle\lim_{x \to -\infty} {x^n e^x}=0$ **CQFD**
      
        
## Exercices 
!!! example "Activités :" 
    A page 162 <br>
    B page 162

!!! question "Recherche de limites :"
    ===  "Exercices  :"
        N°17 p176 (5 minutes)<br>
        N°20 p176 (5 minutes)<br>
        N°21 p176 (5 minutes)<br>
        
    ===  "Corrigé :"
        
        [Correction 17-20-21](./corr/17-20-21.pdf){:target="_blank"}
        <br>
      
!!! question "Formalisme des limites :"
    === "Exercices :"
        N°38 p178 (15 minutes)
    === "Indice :"
        Pour $A$ donné, il faut résoudre l'inéquation $f(x)>A$
    === "Corrigé :"
        [Correction 38](./corr/38.pdf){:target="_blank"}  

       <br>
!!! question "Opérations sur les limites :"
    === "Exercices :"
        N°24 p177 (7 minutes)<br>
        N°25 p177 (7 minutes)<br>
        N°26 p177 (7 minutes)<br>
        N°52 p180 (10 minutes)
    === "Indice :"
        Utiliser les formules du cours <br>
        Tracer la courbe représentative à la calculatrice pour conjecturer le résultat.
    === "Corrigé :"
         [Correction 24-25-26](./corr/24-25-26-54.pdf){:target="_blank"}  

!!! question "Formes Indéterminées :"
    === "Exercices :"
        N°27 p177 (10 minutes)<br>
        N°28 p177 (10 minutes)<br>
    === "Indice :"
        Utiliser les méthodes vues page 9 du cours
        Tracer la courbe représentative à la calculatrice pour conjecturer le résultat.
    === "Corrigé :"
         [Correction 27-28](./corr/27-28.pdf){:target="_blank"}  

    
!!! question "Limite d'une composée de fonctions :" 
    === "Exercices : "
        Déterminer les limites suivantes :  
        $\displaystyle\lim_{x \to +\infty} \sqrt{x^2+3x+2}$  
        $\displaystyle\lim_{x \to +\infty} e^{-x^3-5x^2+2}$  


    
!!! question "Comparaisons - Théorème des gendarmes :"
    === "Exercices :"
        N°75 p183 (7 minutes)<br>
        N°77 p183 (12 minutes)<br>
        N°80 p183 (12 minutes)
    === "Indice :"
        Cours + les méthodes vues page 9 du cours (Ex 80)
        Tracer la courbe représentative à la calculatrice pour conjecturer le résultat.
    === "Corrigé :"
         A venir
         [75-77-80](./corr/75-77-80.pdf){:target="_blank"}  

!!! question "Demonstration limites de l'exponentielle : "
    === "Exercices :"
        N°91 p184 (fait ensemble)<br>
    
!!! question "Théorèmes des croissances comparées :"
    === "Exercices :"
        N°84 p183 (10 minutes)<br>
        Demonstration des théorèmes (faits ensemble)
    === "Indice :"
        Cours
        Tracer la courbe représentative à la calculatrice pour conjecturer le résultat.
    === "Corrigé :"
         A venir
         [84](./corr/84.pdf){:target="_blank"}  


!!! info " Correction de travail / Devoirs : "  
    [Correction QCM](./corr/CorrectionQCM.pdf){:target="_blank"}   
    [correction Eval G1](./corr/EvalG1.pdf){:target="_blank"}  
    [correction Eval G2](./corr/EvalG2.pdf){:target="_blank"}  
    




