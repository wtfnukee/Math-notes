## Парадокс Рассела
$M = \set{A:A \notin A}$
$M \in M ?$
Если $M \in M$, то $M \notin M$
Если $M \notin M$, то $M \in M$
## Система аксиома Цермело-Френкеля
1. **Аксиома объемности.** 
	Одинаковы те множества, что состоят из тех же элементов $A = B \iff \forall x (x \in A \iff x \in B)$
	- Хотя бы одно множество есть
	- $A \subset B$, если $\forall x (x \in A \implies x \in B)$
2. **Аксиома выделения**
	$A$ - множество со свойством $P(x)$ - $\set{x: x \in A \ \text{и} \ P(x)}$
	$\varnothing = \set{x: x \in A \ \text{и} \ x \ne x}$
3. **Аксиома степени**
	Для всякого множества $A$ семейство его подмножеств является множеством $2^A = \set{x:x \subset A}$
4. **Аксиома пары**
	$A, B \to \set{A, B}$
	$\set{A,A} = \set{A}$
5. **Аксиома суммы**
	$\bigcup M := \set{x | \exists A \in M: x \in A}$

- $A \cup B = \{ x: x \in A \lor \ x \in B \} = \bigcup \set{A;B}$
- $A \cap B = \{ x: x \in A \land \ x \in B \}$ 
- $A \setminus B = \set{x: x \in A \land x \notin B}$
- $(a,b) = \set{\set{a}, \set{a,b}}$
#Упражнение $(a,b) = (c,d) \implies a=c, b=d$
- $A \times B = \set{(a, b)| a \in A \land b \in B} = \set{x: x \in 2^{2^{A \cup B}} \land \exists a \in A, b \in B: x = (a, b)}$

$f: X \to Y$ - функция, каждому $x$ сопоставляется $y = f(x)$
$\Gamma_f = \set{(x,y) : y = f(x)}$
1. $\forall x \exists y \in Y: (x,y) \in \Gamma$
$\forall x,y,z (x,y) \in \Gamma \land (x,z) \in \Gamma \implies y = z$

$f: X \to Y$ и $g: Y \to Z$
$g \circ f (x) = g(f(x))$
$\Gamma_{g \: \circ f} = \set{(x,y) | \exists y \in Y: (x,y) \in \Gamma_f \land (y, z) \in \Gamma_g}$
#Упражнение $g \circ (f \circ h) = (g \circ f) \circ h$

$f: X \to Y$ инъекция, если $x_1 \ne x_2 \implies f(x_1) = f(x_2)$
$f: X \to Y$ сюръекция, если $\forall y \exists x: f(x) = y$
$f: X \to Y$ биекция, если $f$ и инъективна, и биективна

#Теорема 
1. $f$ и $g$ - биекция $\implies f \circ g$ биекция
2. $f$ - биективна $\implies \set{(y,x): y = f(x)}$ задает функцию $f^{-1} : Y \to X$, которая является биективной и называется обратной

$X \ne \varnothing, G(X) = \set{f | f: X \to X - \text{биекция}}$ 
$G(X)$ - группа биекций (симметрическая группа)
$(f,g) \mapsto f \circ g$
1. $f \circ (g \circ h) = (f \circ g) \circ h$
2. $e \circ f = f \circ e = f$ ($e(x) = x$)
3. $\forall f \ \exists f^{-1} : f \circ f^{-1} = f^{-1} \circ f = e$

Группа биекций
$(\mathbb{R}, +) \cong T^a(x) = x+a$
$a \mapsto T^a$

$\mathbb{Z}_2 \cong \mathbb{R}^\pi$
$(G, \circ) \cong (M, \star) \iff \exists \ \text{биекция} \ f: G \to M: \ f(a \circ b) = f(a) \star f(b)$
Если $(G, \circ), G \supset H, (H, \circ)$ - группа $\implies H$ - подгруппа

#Теорема Теорема Кэли
Всякая группа изоморфна подгруппе некоторой группе биекций.
*Доказательство*
$(X, \star)$ и $(G(X), \circ)$
$z \in X \mapsto f_z(x) = z \star x$ - искомый изоморфизм на подгруппу 