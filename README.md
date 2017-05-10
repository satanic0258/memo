$F$ を体、 $V$ を $F$ 上の $n$ 次元数ベクトル空間、$(b_1, b_2, \cdots, b_n)$ は $V$ の基底であるとする。  
このとき、$V$ の任意のベクトル $\mathbb{v}\in V$ は、 $b_1, b_2, \cdots, b_n$ の一次結合
$$ \mathbb{v} = c_1b_1 + c_2b_2 + \cdots + c_nb_n \ (c_1, c_2, \cdots , c_n \in F) $$  
の形で一意的に表せることを示せ。

---

$(b_1, b_2, \cdots, b_n)$ は $V$ の基底であるから、$\{ b_1, b_2, \cdots, b_n \}$ は一次独立。  
$i.e. B=(b_1, b_2, \cdots, b_n), \mathbb{c}\in F^n$ としたとき、$B\mathbb{c}=\mathbb{0}$ の解は $\mathbb{c} = \mathbb{0}$ のみ。  
これは、 $B$ を適切に行基本変形すると、 $n$次元単位行列$E_n$に出来ることと同値である。  
（ただし、 $E_n$ は対角成分に乗法単位元 $1_F$ を、非対角成分に加法単位元 $0_F$ を並べた $n$ 次正方行列）  
ここで、行基本変形の各操作は、ある行列を左からかけることと同値である。  
具体的には、$n$ 次正方行列 $X, Y$ に対して、
* $X \xrightarrow[(p)\leftrightarrow (q)]{} Y$ (ただし、 $1 \leq p,q \leq n$) のとき、
  ${}^\exists P\ s.t.\ PX=Y$。  

  このとき、$P = (p_{ij})_ {i=1}^n$ として、  
  $$p_{ij} =
  \begin{cases}
    1_F & (i=p \text{ かつ } j=q \text{ 、または } i=q \text{ かつ } j=p \text{ 、または } i\neq p, q \text{ かつ } i=j ) \\
    0_F & (それ以外)
  \end{cases}$$
* $X \xrightarrow[k(p)]{} Y$ (ただし、 $1 \leq p \leq n, k\in F$ ) のとき、
  ${}^\exists P\ s.t.\ PX=Y$。  

  このとき、$P = (p_{ij})_ {i=1}^n$ として、  
  $$p_{ij} =
  \begin{cases}
    k & (i=j=p)\\
    1_F & (i=j\neq p) \\
    0_F & (それ以外)
  \end{cases}$$
* $X \xrightarrow[(p)+k(q)]{} Y$ (ただし、 $1 \leq p,q \leq n, k\in F$ ) のとき、
    ${}^\exists P\ s.t.\ PX=Y$。  

    このとき、$P = (p_{ij})_ {i=1}^n$ として、  
    $$p_{ij} =
    \begin{cases}
      k & (i=p, j=q)\\
      1_F & (i=j) \\
      0_F & (それ以外)
    \end{cases}$$

従って、 $m$ 回の操作により $B$ を行基本変形により $E_n$ と出来るとき、第 $i$ 番目の操作を、上記のような行列 $P_i$ を左からかけることに対応させると、
$$ P_m P_{m-1} \cdots P_2 P_1 B = E_n $$
が成り立つ。今、$P:=P_m P_{m-1} \cdots P_2 P_1$ とする。このとき、 $PB=E_n$ である。  

故に、 ${}^\forall \mathbb{v}\in V$に対して、 連立一次方程式 $B\mathbb{c} = \mathbb{v}$ は、両辺に左から $P$ をかけると、
$$\begin{eqnarray}
PB \mathbb{c} &=& P\mathbb{v} \\
E_n\mathbb{c} &=& P\mathbb{v} \\
\mathbb{c} &=& P\mathbb{v}
\end{eqnarray}$$
従って、解は $\mathbb{c} = P\mathbb{v}$ のただ一つである。  
$\therefore$ $V$ の任意のベクトルは $b_1, b_2, \cdots, b_n$ の一次結合で一意に表せる。 //
