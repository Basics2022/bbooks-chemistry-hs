(book:chemistry-hs:reactions)=
# Reazioni chimiche

## Dinamica di reazioni elementari

Data una reazione diretta (o irreversibile)

$$a A + b B \rightarrow c C + d D \ ,$$

si può definire la velocità della reazione come

$$v = -\frac{1}{a} \frac{d [A]}{dt} = -\frac{1}{b} \frac{d [B]}{dt} = \frac{1}{c} \dfrac{d [C]}{dt} = \frac{1}{d}\frac{d [D]}{dt} = \frac{d \xi}{dt} \ ,$$

avendo definito con $\xi$ il **grado di avanzamento della reazione**. Sperimentalmente, secondo la **legge di massa**, si osserva che la velocità di reazione è direttamente proporzionale alla concentrazione dei reagenti (**todo** *in quali condizioni? aggiungere qualche considerazione...*) e a un fattore che dipende dalla temperatura $T$,

$$v \sim k(T) [A]^{\alpha} [B]^{\beta} \ .$$

I coefficienti $\alpha$, $\beta$, $\gamma$, $\delta$ sono definiti **ordini parziali della reazione**, in generale non coincidono con i coefficienti stechiometrici, e vengono determinati sperimentalmente. La somma degli ordini parziali viene definito **ordine globale della reazione**.
Il coefficiente $k(T)$ è definito **costante specifica di velocità** della reazione, e anch'esso viene determinato sperimentalmente tramite la determinazione dei coefficienti di un'espressione che prende il nome di **equazione di Arrhenius**,

$$k = A e^{-\frac{\Delta E}{R T}} \ .$$

Il coefficiente $A$ viene definito fattore pre-esponenziale e il parametro $\Delta E$, che può dipendere dalla temperatura, prende il nome di **energia di attivazione**.

```{prf:example} Reazione diretta del primo ordine
:class: dropdown

$$A \rightarrow P$$

$$r = \dfrac{d [A]}{dt} = - k [A]$$

```

```{prf:example} Reazione diretta del secondo ordine
:class: dropdown

$$2 A \rightarrow P$$

$$r = \dfrac{d [A]}{dt} = - k [A]^2$$

```

```{prf:example} Reazione diretta del secondo ordine con due reagenti
:class: dropdown

$$A + B \rightarrow P$$

$$r = \dfrac{d [A]}{dt} = \frac{d [B]}{d t} = - k [A][B]$$

```

## Equilibrio chimico
Per una reazione reversibile

$$a A + b B \rightleftharpoons c C + d D \ .$$

la variazione delle concentrazioni è determinata dalla legge di massa,

$$\begin{aligned}
  \frac{1}{a} \frac{d [A]}{dt} & = -  k_+ [A]^a [B]^b + k_{CD} [C]^c [D]^d \\
  \frac{1}{b} \frac{d [B]}{dt} & = -  k_+ [A]^a [B]^b + k_{CD} [C]^c [D]^d \\
  \frac{1}{c} \frac{d [C]}{dt} & =    k_+ [A]^a [B]^b - k_{CD} [C]^c [D]^d \\
  \frac{1}{d} \frac{d [D]}{dt} & =    k_+ [A]^a [B]^b - k_{CD} [C]^c [D]^d \\
\end{aligned}$$

avendo definito le velocità delle reazioni diretta e inversa,

$$\begin{aligned}
  v_+ & = k_+ [A]^{\alpha} [B]^{\beta} \\
  v_- & = k_- [C]^{\gamma} [D]^{\delta} \\
\end{aligned}$$

L'equilibrio chimico è determinato dalla condizioni in cui le due velocità sono uguali, e quindi le concentrazioni non cambiano,

$$v_+ = v_- \ .$$

La condizione di equilibrio di una reazione è contraddistinta dalla costante di equilibrio $K$,

$$1 = \frac{v_-}{v_+} = \frac{k_- [C]^{\gamma} [D]^{\delta}}{k_+ [A]^{\alpha} [B]^{\beta}}
\qquad \rightarrow \qquad
K := \frac{[C]^{\gamma} [D]^{\delta}}{[A]^{\alpha} [B]^{\beta}} = \frac{k_+}{k_-}
$$

**Principio di Le Chatelier** (1884): perturbando il sistema, l'evoluzione del sistema si sposta verso un nuovo equilibrio che tende ad annullare la perturbazione. Ad esempio, aggiungendo $A$ il sistema si trova inizialmente in un eccesso di reagenti, e tenderà a ridurre questo eccesso.

**Gibbs - Energia libera di Gibbs** (1873): la condizione di equilibrio di una reazione che avviene a temperatura e pressione costante è raggiunta in corrispondenza di un minimo dell'energia libera di Gibbs. Se una reazione è descritta da una coordinata di avanzamento $\xi$, e l'energia libera di Gibbs dipende unicamente da questa variabile, allora la condizione di equilibrio è determinata dalla condizione $\frac{d G}{d \xi} = 0$.

**to be continued** wiki,
- chemical equilibrium
- Gibbs\textquotesingle free energy



- chemical kinetics

