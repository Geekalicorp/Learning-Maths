# Vector transformation

$$
\begin{matrix}

\begin{bmatrix}
  x \\
  y
\end{bmatrix}
\begin{bmatrix}
  a & b \\
  c & d
\end{bmatrix}

\end{matrix}
$$ 

$$
\begin{matrix}

x \begin{bmatrix}
a \\
c
\end{bmatrix}
+
y \begin{bmatrix}
b \\
d
\end{bmatrix}
& = & \begin{bmatrix}
  ax + by \\
  cx + dy
\end{bmatrix}

\end{matrix}
$$


# 2D matrix multiplication

## Init

$$
\begin{matrix}

\begin{bmatrix}
  a & b \\
  c & d \\
\end{bmatrix}
\begin{bmatrix}
  e & f \\
  g & h \\
\end{bmatrix}

\end{matrix}
$$

### Vector i

$$
\begin{matrix}

\begin{bmatrix}
  a & b \\
  c & d \\
\end{bmatrix}
\begin{bmatrix}
e \\
b \\
\end{bmatrix}
& = & e \begin{bmatrix}
a \\
c \\
\end{bmatrix}
+
g \begin{bmatrix}
b \\
d \\
\end{bmatrix}
& = & \begin{bmatrix}
  ae + bg \\
  ce + dg \\
\end{bmatrix}

\end{matrix}
$$

### Vector j

$$
\begin{matrix}

\begin{bmatrix}
  a & b \\
  c & d \\
\end{bmatrix}
\begin{bmatrix}
f \\
h \\
\end{bmatrix}
& = & f \begin{bmatrix}
  a \\
  c \\
\end{bmatrix}
+
h \begin{bmatrix}
  b \\
  d \\
\end{bmatrix}
& = & \begin{bmatrix}
  af + bh \\
  cf + dh \\
\end{bmatrix}

\end{matrix}
$$

## Total

$$
\begin{matrix}

\begin{bmatrix}
  ae + bg & af + bh \\
  ce + dg & cf + dh \\
\end{bmatrix}

\end{matrix}
$$


# 3D matrix multiplication

## Init

$$
\begin{matrix}

\begin{bmatrix}
  a & b & c \\
  d & e & f \\
  g & h & i \\
\end{bmatrix}
\begin{bmatrix}
  j & k & l \\
  m & n & o \\
  p & q & r \\
\end{bmatrix}

\end{matrix}
$$

### Vector i

$$
\begin{matrix}

\begin{bmatrix}
  a & b & c \\
  d & e & f \\
  g & h & i \\
\end{bmatrix}
\begin{bmatrix}
  j \\
  m \\
  p \\
\end{bmatrix}
& = & j \begin{bmatrix}
  a \\
  d \\
  g \\
\end{bmatrix}
+
m \begin{bmatrix}
  b \\
  e \\
  h \\
\end{bmatrix}
+
p \begin{bmatrix}
  c \\
  f \\
  i \\
\end{bmatrix}
& = & \begin{bmatrix}
  aj + bm + cp \\
  dj + em + fp \\
  gj + hm + ip \\
\end{bmatrix}

\end{matrix}
$$

### Vector j

$$
\begin{matrix}

\begin{bmatrix}
  a & b & c \\
  d & e & f \\
  g & h & i \\
\end{bmatrix}
\begin{bmatrix}
  k \\
  n \\
  q \\
\end{bmatrix}
& = & k \begin{bmatrix}
  a \\
  d \\
  g \\
\end{bmatrix}
+
n \begin{bmatrix}
  b \\
  e \\
  h \\
\end{bmatrix}
+
q \begin{bmatrix}
  c \\
  f \\
  i \\
\end{bmatrix}
=\begin{bmatrix}
  ak + bn + cq \\
  dk + en + fq \\
  gk + hn + iq \\
\end{bmatrix}

\end{matrix}
$$

### Vector k

$$
\begin{matrix}

\begin{bmatrix}
  a & b & c \\
  d & e & f \\
  g & h & i \\
\end{bmatrix}
\begin{bmatrix}
  l \\
  o \\
  r \\
\end{bmatrix}
& = & l \begin{bmatrix}
  a \\
  d \\
  g \\
\end{bmatrix}
+
o \begin{bmatrix}
  b \\
  e \\
  h \\
\end{bmatrix}
+
r \begin{bmatrix}
  c \\
  f \\
  i \\
\end{bmatrix}
& = & \begin{bmatrix}
  al + bo + cr \\
  dl + eo + fr \\
  gl + ho + ir \\
\end{bmatrix}


\end{matrix}
$$

## Total

$$
\begin{matrix}

\begin{bmatrix}
  aj + bm + cp & ak + bn + cq & al + bo + cr \\
  dj + em + fp & dk + en + fq & dl + eo + fr \\
  gj + hm + ip & gk + hn + iq & gl + ho + ir \\
\end{bmatrix}


\end{matrix}
$$


# 2D Determinant

$$
\begin{matrix}

det \begin{bmatrix}
  a & b \\
  c & d \\
\end{bmatrix}
& = & (a+b) (c+d) - ac - bd -2bc \\
& = & ad - cb

\end{matrix}
$$


# 3D Determinant

$$
\begin{matrix}

det \begin{bmatrix}
  a & b & d \\
  e & f & g \\
  h & i & j \\ 
\end{bmatrix}
& = & a * det\begin{bmatrix}
  e & f\\
  h & i
\end{bmatrix} \\
& - & b * det\begin{bmatrix}
  d & f\\
  g & i
\end{bmatrix} \\
& + & c * det\begin{bmatrix}
  d & e\\
  g & h
\end{bmatrix}

\end{matrix}
$$

<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
