### Dimostrazione 3.1.5
[[Teoremi, proposizioni e definizioni#Proposizione 3.1.5 Span e sottospazi vettoriali | Proposizione 3.1.5]]

* Definzioni e teoremi usati:
 [[Teoremi, proposizioni e definizioni#Definizione 3.1.2 Sottospazio generato | Definizione di Sottospazio generato]]
 [[Teoremi, proposizioni e definizioni#Definizione 2.4.1 Sottospazio vettoriale| Definizione di un sottospazio vettoriale]]
 

1) $v_1,\dots,v_n \in V, W = \langle v_1,\dots,v_n\rangle, W \subseteq V$
	Lo span è definito come $\langle v_1,\dots,v_n\rangle = \{\lambda_1v_1 + \dots+\lambda_nv_n | \lambda_1,\dots,\lambda_n \in \mathbb{R} \}$, verifichiamo le tre proprietà di un sottospazio:
	1) $0_v \in \langle v_1,\dots,v_n\rangle$ in quanto $0_v = 0v_1+\dots+0v_n$
	2) Siano $v,w \in W$, per definizione di span $v = \alpha_1v_1+\dots+\alpha_nv_n, \ e \ w = \beta_1v_1+\dots+\beta_nv_n$ . Quindi $v+w = (\alpha_1+\beta_1)v_1+\dots+(\alpha_n + \beta_n)v_n$, essendo il vettore $v+w$ combinazione lineare di $v_1,\dots,v_n$ appartiene a W.
	3) Siano $v \in W, k \in \mathbb{R}$, per definizione di sottospazio generato $v = \alpha_1v_1+\dots+\alpha_nv_n$. Quindi $kv = (k\alpha_1)v_1+\dots+(k\alpha_n)v_n$, essendo il vettore $kv$ combinazione lineare di $v_1,\dots,v_n$, appartiene a W.
2) $Z\subseteq V, v_1,..,v_n \in Z: \langle v_1,..,v_n\rangle \subseteq Z$
	Segue immediatamente dalla definizione di span: ogni combinazione lineare dei $v_i$ resta in Z se Z è chiuso rispetto a somma e prodotto per scalare.  La dimostrazione è quindi analoga al punto 1.

### Dimostrazione 3.1.8
[[Teoremi, proposizioni e definizioni#Proposizione 3.1.8 Insieme di generatori con combinazioni lineari|Proposizione 3.1.8]]

* Definizioni e teoremi usati
...

Siano $V$ uno spazio vettoriale e $v_1,\dots,v_n \in V$, allora: $w\in \langle v_1,\dots,v_n\rangle \iff \langle v_1,\dots,v_n\rangle=\langle v_1,\dots,v_n,w\rangle$

Dimostro entrambe le di