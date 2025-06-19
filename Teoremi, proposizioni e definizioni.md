Il seguente file contiene tutti i teoremi, proposizioni, osservazioni e definizioni dei capitoli 2-10 del libro "Introduzione all'algebra lineare" di Fioresi e Morigi e delle dispense fornite a lezione sulle equazioni cartesiane ortogonalità.
Le dimostrazioni sono omesse, quelle richieste per l'esame si trovano nel file 'Dimostrazioni.md'
# Capitolo 2: Spazi Vettoriali

### Definizione 2.3.1: Spazio vettoriale
Uno spazio vettoriale è un insieme V munito delle operazioni di somma e prodotto per scalare:
$$\begin{align} + : V \times V \rightarrow V \qquad  (u,v) \mapsto u +v\end{align} $$
$$\begin{align} \cdot : R \times V \rightarrow V \qquad (\lambda,v) \mapsto \lambda v\end{align} $$
Tali che abbiano le seguenti proprietà:
Per la somma:
1) Commutativa: $\forall u,v \in V: u+v = v+u$
2) Associativa: $\forall u,v,w \in V:(u+v)+w = u+(v+w)$
3) Ammette u elemento neutro: $\exists0 \in V, \forall v\in V: 0+v = v$
4) Ogni elemento ha un suo opposto: $\forall u \in V \exists a: a+u = 0$
Per il prodotto scalare:
5) $1u = u$
6) $\forall \lambda,\mu \in \mathbb{R}, \forall u \in V :(\lambda \mu )u = \lambda(\mu u)$
7) $\forall \lambda \in \mathbb{R}, \forall u,v \in V :\lambda(v+u) = \lambda u + \lambda v$$
8) $\forall \lambda,\mu \in \mathbb{R}, \forall u \in V :(\lambda +\mu )u = \lambda u + \mu u$

### Proposizione 2.3.5: Proprietà di uno spazio vettoriale
1) Il vettore nullo è unico e chiamato $0_v$
2) Il vettore opposto a $v$ è unico e chiamato $-v$
3) $\forall \lambda \in \mathbb{R}: \lambda 0_v = 0_v$
4) $\forall u\in V: 0u = 0_v$
5) $\lambda u = 0_v \implies \lambda=0 \vee u = 0_v$
6) $(-\lambda)u = \lambda(-u) = -\lambda u$

### Definizione 2.3.6: Spazio vettoriale banale
Si dice uno spazio vettoriale banale indicato con $\{0_v\}$ uno spazio vettoriale che contiene solo il vettore nullo

### Osservazione 2.3.7: Operazioni in un spazio banale
Uno spazio vettoriale mantiene le operazioni di somma e prodotto scalare, infatti:
$$0_v + 0_v = 0_v$$
$$\forall \lambda \in \mathbb{R}: \lambda 0_v = 0_v$$

### Osservazione 2.3.8 Dimensione degli spazi vettoriali
Uno spazio vettoriale V non potrà mai essere vuoto, infatti contiene almeno il vettore nullo. Inoltre potrà avere o un solo elemento, il vettore nullo, o un vettore v con tutti i suoi multipli ($\lambda v$)

### Definizione 2.4.1: Sottospazio vettoriale
Chiamato W un sottoinsieme dello spazio vettoriale V, W è un sottospazio vettoriale di V ($W\subseteq V$) sse:
1) $W \neq \{\}$
2) W è chiuso rispetto alla somma: $\forall u,v \in W: u+v \in W$
3) W è chiuso rispetto al prodotto scalare: $\forall \lambda \in \mathbb{R},\forall u \in W: \lambda u \in W$
Da queste tre proprietà è evidente derivarne una quarta:
4) $0_v \in W$

### Osservazione 2.4.7 Multipli in un sottospazio
Affermare che W è chiuso rispetto al prodotto scalare equivale a dire che se W contiene un vettore non nullo v, allora contiene anche tutti i suoi multipli.
Ciò rende evidente che sottoinsiemi comuni come la circonferenza e la parabola non siano sottospazi vettoriali

### Osservazione 2.4.8 Constatare un sottospazio
Per dimostrare che W è uno sottospazio vettoriale è necessario dimostrare che le proprietà valgono per tutti i possibili vettori e scalari, mentre per dimostrare che non lo è basta trovare un valore che invalida una delle proprietà

### Proposizione 2.4.12 Unione di sottospazi
$$\forall W_1,\ W_2 \subseteq V: \ W_1\cup W_2 \subseteq V \iff W_1\subseteq W_2\ \vee  W_2\subseteq W_1$$

### Proposizione 2.4.12 Intersezione di sottospazi
$$\forall W_1,\ W_2 \subseteq V: \ W_1\cap W_2 \subseteq V$$

# Capitolo 3: Combinazioni Lineari

### Definizione 3.1.1: Combinazione lineare
Siano $V$ uno spazio vettoriale, $v_1,..,v_n \in V, \lambda_1,..,\lambda_n \in \mathbb{R}$  dei vettori di $V$, il vettore
$w$ si dice combinazione lineare se $w = \lambda_1v_1 + ..+\lambda_nv_n$

### Definizione 3.1.2: Sottospazio generato
Dati $v_1,..,v_n \in V$ si dice sottospazio generato  da $v_1,..,v_n$ l'insieme di tutte le combinazioni lineari di $v_1,..,v_n$
$$\langle v_1,..,v_n\rangle = \{\lambda_1v_1 + ..+\lambda_nv_n | \lambda_1,..,\lambda_n \in \mathbb{R} \}$$
Quindi affermare che $w\in \langle v_1,\dots,v_n\rangle$ equivale ad affermare che $w$ è combinazione lineare di $v_1,\dots,v_n$.

NB: Il sottospaziono generato è anche chiamato span, questi due termini d'ora in poi verrano usati indistintamente.

### Osservazione 3.1.3: Sottospazi da singoli vettori
1) Se $v\in V$ allora il sottospazio generato da $v$ corrisponde a tutti i suoi multipli $\langle v \rangle = \{\lambda v | \lambda \in \mathbb{R}\}$
2) Lo span del vettore nullo è il vettore nullo, $\langle 0_v \rangle = \{0_v\}$

### Definizione 3.1.4: Insieme di generatori
Se $\langle v_1,..,v_n\rangle = V$ allora $\{v_1,..,v_n\}$ è detto insieme di generatori di $V$ e i vettori $v_1,..,v_n$ generano $V$

### Proposizione 3.1.5: Span e sottospazi vettoriali
1) $v_1,\dots,v_n \in V, W = \langle v_1,\dots,v_n\rangle, W \subseteq V$
2) $Z\subseteq V, v_1,..,v_n \in Z: \langle v_1,..,v_n\rangle \subseteq Z$, cioè $\langle v_1,..,v_n\rangle$ è il più piccolo sottospazio di $V$ contenente $\{ v_1,..,v_n\}$

[[Dimostrazioni#Dimostrazione 3.1.5|Dimostrazione]]

### Proposizione 3.1.8: Insieme di generatori con combinazioni lineari
Siano $V$ uno spazio vettoriale e $v_1,\dots,v_n \in V$, allora:
1) Se il vettore $w$ è combinazione lineare di $v_1,\dots,v_n$ allora $\langle v_1,\dots,v_n\rangle = \langle v_1,\dots,v_n, w\rangle$
2) Se $\langle v_1,\dots,v_n\rangle = \langle v_1,\dots,v_n, w\rangle$ allora $w$ è combinazione lineare di $v_1,\dots,v_n$
Riassumendo:
$$w\in \langle v_1,\dots,v_n\rangle \iff \langle v_1,\dots,v_n\rangle=\langle v_1,\dots,v_n,w\rangle$$

# Capitolo 4: Basi e dimensioni
# Capitolo 5: Applicazioni lineari


# Capitolo 6: Sistemi lineari

# Capitolo 7: Determinante e inversa

# Capitolo  8: Cambio di base

# Capitolo 9: Autovalori e autovettori

# Extra 1: Equazioni cartesiane

# Extra 2: Ortogonalità

# Capitolo 10: Elementi di matematica discreta