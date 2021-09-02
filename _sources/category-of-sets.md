# Categoria dos Conjuntos

**Conjunto**: uma coleção qualquer de elementos, sendo que para quaisquer dois elementos $x$, $x'$ pertencentes a um conjunto $X$, devemos ser capazes de distinguir se são iguais ou diferentes. Para denotar que um elemento pertence a um conjunto, usamos $x \in X$. Note que um subconjunto não precisa ser necessariamente finito. 

**Subconjunto**: dizemos que um conjunto $A$ é um subconjunto de outro conjunto $B$, se para todo $a \in A$, temos que $a \in B$. Para denotar que $A$ é subconjunto de $B$, usamos $A \subseteq B$. Note que todo conjunto é subconjunto dele mesmo: $A \subseteq A$.

**Conjunto Vazio**: definimos o conjunto $\{\ \ \}$ com nenhum elemento como conjunto vazio. Também usamos a notação $\emptyset$ para representar o conjunto vazio. O conjunto vazio é subconjunto de qualquer conjunto $\emptyset \subseteq A$.

**Conjunto de partes**: o conjunto de todos os possíveis subconjuntos de um determinado conjunto $A$ é denominado conjunto das partes de $A$. Usamos a notação $\mathcal{P}(A)$ para denotar o subconjunto das partes de $A$.

**Função ou mapa**: sejam $A$ e $B$ dois conjuntos quaisquer, definimos uma função $f: A \rightarrow B$ como um mapeamento de todo elemento $a$ do conjunto $A$ para um elemento do conjunto $B$, o qual chamamos $f(a)$. Chamamos $A$ de **domínio** da função e $B$ de **codomínio**. Chamamos de **imagem** da função $f$ o subconjunto do codomínio $B$ cujos elementos são associados aos elementos do domínio $A$. Formalmente, temos: 

$$Im(f) = \{b \in B \ \vert \ \exists \ a \in A \text{ tal que } f(a) = b \}$$

**Mapa injetivo (1-on-1 ou into)**: seja $f:X \rightarrow Y$. O mapa $f$ é chamado de um-a-um se para cada $y \in Y$ existe somente um $x \in X$. Se para $x, x' \in X, x \ne x' \Longrightarrow f(x) \ne f(x')$ ou $f(x) = f(x') \Longrightarrow x = x'$. Exemplo: $f: \mathbb{R}_{\ge 0} \rightarrow \mathbb{R}$ definido por $f(x) = x^{2}$.

**Mapa sobrejetivo (onto)**: um mapa é chamado de sobrejetivo (onto) se para cada $y \in Y$ existe pelo menos um $x \in X$ tal que $f(x) = y$. Se $f: X \rightarrow Y$, é comum dizer apenas "$f$ é um mapa de $X$ sobre $Y$.” Exemplo: seja $X = \lbrace x \in \mathbb{R} \vert -\frac{\pi}{2} \le x \le \frac{\pi}{2} \rbrace$. Seja $f: X \rightarrow \mathbb{R}$ definido pela função tangente: $f(x) = \tan{x}$.

**Mapa bijetivo (1-on-1 correspondence)**: um mapa é dito bijetivo ou que é uma bijeção se é tanto 1-1 quanto sobrejetivo. Exemplo: a função exponencial, $f: \mathbb{R} \rightarrow \mathbb{R}_{\ge 0}$, definida por $f(x) = e^{x}$.

**Mapa de Inclusão**: dado um subconjunto $A \subseteq X$, o mapa $i : A \rightarrow X$ deﬁnido como $i(a) = a\ \forall a \in A$ é
chamado de mapa de inclusão, também denotado como $i : A \xhookrightarrow{} X$. Exemplo: os naturais são um subconjunto dos reais, $\mathbb{N} \subset \mathbb{R}$. Então um mapa de inclusão pode ser $i : \mathbb{N} \xhookrightarrow{} \mathbb{R}$, definido por $i(n) = n\ \forall n \in \mathbb{N}$.

**Restrição de um mapa**: dado um subconjunto $A \subseteq X$, uma restrição de um mapa $f: X \rightarrow Y$ é $f|_{A}: A \rightarrow Y$, ou seja, fazemos uma restrição no domínio. Exemplo: o mapa $f: \mathbb{R} \rightarrow \mathbb{R}$ definido por $f(x) = x^{2}$ não é injetivo, mas podemos fazer a restrição no domínio e torná-lo injetivo: $f\vert_{\mathbb{R}_{\ge 0}}: \mathbb{R}_{\ge 0} \rightarrow \mathbb{R}$.

**Corestrição**: seja $i_{W}: W \xhookrightarrow{} Y$, onde $W \subseteq Y$ e seja $f: X \rightarrow Y$. A corestrição é a composição $i_{W} \circ f: X \rightarrow W$. Exemplo: a função exponencial, $f: \mathbb{R} \rightarrow \mathbb{R}_{\ge 0}$, definida por $f(x) = e^{x}$.

**Mapa Identidade**: dado o mapa de inclusão, se $A = X$ o mapa é chamado de mapa identidade (ou mapa de identidade), $id_{X} : X \rightarrow X$.

**Mapa Inverso**: seja o mapa $f : X \rightarrow Y$. Se existir um mapa tal que, $f^{-1} : Y \rightarrow X$, mantendo a paridade dos elementos de $X$ e $Y$, dizemos que $f^{-1}$ é o mapa inverso de $f$. Exemplo: a função exponencial, $f: \mathbb{R} \rightarrow \mathbb{R}_{\ge 0}$, definida por $f(x) = e^{x}$ e sua inversa é $f^{-1}: \mathbb{R}_{\ge 0} \rightarrow \mathbb{R}$ definida por $f^{-1}(x) = \ln{x}$.

**Isomorfismo**: se um mapa $f : X \rightarrow Y$ é **bijetivo** existe um mapa inverso, $f^{-1} : Y \rightarrow X$, tal que $f^{-1} : f(x) \rightarrow x$ é também bijetivo. Como consequência $f^{-1} \circ f = id_{X}$ e $f \circ f^{-1} = id_{Y}$. Podemos dizer que os conjuntos $X$ e $Y$ são isomórficos, denotado por $X \cong Y$.

**Composição**: dados os mapas $f: X \rightarrow Y$ e $g: Y \rightarrow Z$, o mapa composto é $g \circ f : X \rightarrow Z$, também denotado como $g(f(x)) = z$. Exemplo: $f(x) = x^{2}$ e $g(y) = y+1$, então $(g \circ f)(x) = g(f(x))$ é definido como $g(f(x)) = (x^{2}) + 1$.

**Mapa n-ário**: é o mapa $f : X^{n} \rightarrow Y$, deﬁnido como $f : (x_{1}, x_{2}, ..., x_{n}) \rightarrow y$.

$f: \mathbb{R}^{2} \times \mathbb{N}_{\ge 0} \rightarrow \lbrace 0,1 \rbrace$. $(x_{1},x_{2},n) \mapsto y$

$f:\mathbb{R}^{2} \rightarrow \mathbb{R}$, definido como $(z) \mapsto (x^{2} + 2 y)$

**Mapa de projeção**: é um mapa n-ário $pr_{i} : X_{1} \times X_{2} \times ... \times X_{n} \rightarrow X_{i}$ , deﬁnido como $pr_{i} : (x_{1}, ..., x_{n}) \rightarrow x_{i}$.

**Mapa Característico**: dado um subconjunto $A \subset X$, um mapa $\chi_{A} : X \rightarrow \lbrace 0, 1 \rbrace$ é dito característico de $A$, deﬁnido como $\chi_{A} (x) = 0$ se $x \notin A$ e $\chi_{A} (x) = 1$ se $x \in A$.

**$Hom_{Set}$**: sejam $X$ e $Y$ dois conjuntos. O conjunto de todos os possíveis mapas $X \rightarrow Y$ é denotado por $Hom_{Set}(X,Y)$.

{1,2,3,4,5} -> {x,y}; A -> B

$|Hom_{set}(A,B)| = |B|^{|A|} = 2^{5} = 32\\$
$|Hom_{set}(B,A)| = |A|^{|B|} = 5^{2} = 25$

**Cardinalidade**: seja $X$ um conjunto. O número de elementos de $X$, denotado $\vert X \vert$, é chamado de cardinalidade.