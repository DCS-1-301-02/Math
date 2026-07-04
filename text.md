# 数式の書き方

## インライン数式

```
数式の書き方には，$ f(𝑥)=𝑥^2+3𝑥+2 $ のように文の途中に書く
```
数式の書き方には，$f(𝑥)=𝑥^2+3𝑥+2$ のように文の途中に書く

## ブロックレベル数式

```
$$
    f(𝑥)=𝑥^2+3𝑥+2
$$
```

$$
    f(𝑥)=𝑥^2+3𝑥+2
$$

## 数値

`$ 1, 0.5, 3.14159 $` → $1, 0.5, 3.14159$ 

## 変数名，関数名

`$ a, x, y, func() $` → $ a, x, y, func() $

## 演算子

### 加算，減算

`$ a + b, c - d $` → $ a + b, c - d $

### 乗算，除算

`$ a \cdot b, c \times d，e \div f $` → $ a \cdot b, c \times d, e \div f $

### 等号，不等号

`$ =, \neq, >, \geq, <, \leq $` → $ =, \neq, >, \geq, <, \leq $

## 指数，添字，根号

### 指数 (上付き文字列)

`$x^2, 2^{128}$` → $x^2, 2^{128}$ ... 1文字でないときは{ }で囲む

### 添字 (下付き文字列)

`$y_1, a_{12}$` → $y_1, a_{12}$ ... 1文字でないときは{ }で囲む

(`$z_1^2, z^2_1$`のようにすれば，$z_1^2, z^2_1$ のように上下に付けられる )

### 根号

`$\sqrt{2}, \sqrt[3]{3}$` → $\sqrt{2}, \sqrt[3]{3}$

## ギリシャ文字

数式でよく使うギリシャ文字

### 小文字
$ \alpha, \beta, \gamma, \delta, \epsilon, \varepsilon, \lambda, \pi, \sigma, \theta, \phi, \psi, \omega $ ←
`$ \alpha, \beta, \gamma, \delta, \epsilon, \varepsilon, \lambda, \pi, \sigma, \theta, \phi, \psi, \omega $`

### 大文字
$ \Alpha, \Beta, \Gamma, \Delta, \Pi, \Sigma, \Theta, \Phi, \Psi, \Omega $
← `$ \Alpha, \Beta, \Gamma, \Delta, \Pi, \Sigma, \Theta, \Phi, \Psi, \Omega $`


## 分数

分数は `\frac{分子}{分母}` のように書く，
インラインだと相対的に小さくなるので，ブロックレベルで表示の方が見易い

`$ \frac{1}{2}x, \frac{1}{2a} $` → $\frac{1}{2}x, \frac{1}{2a} $

`$$ \frac{1}{2}x, \frac{1}{2a} $$`
$$ \frac{1}{2}x, \frac{1}{2a} $$

## 2項関係

後述する行列でも記述できる 

`$\binom{3}{2}$` → $\binom{3}{2}$

`$$\binom{3}{2}$$` → $$\binom{3}{2}$$

## 微積分

```
$$
  \begin{align}
    f(x) &= x^2 + 2x + 1 \\
    f'(x) &= \frac{df(x)}{dx} = 2x + 2 \\
    \int f(x) dx &= \frac{x^3}{3} + x^2 + 2x + C \ (Cは積分変数) \\
  \end{align}
$$
```

$$
  \begin{align}
    f(x) &= x^2 + 2x + 1 \\
    f'(x) &= \frac{df(x)}{dx} = 2x + 2 \\
    \int f(x) dx &= \frac{x^3}{3} + x^2 + 2x + C \ (Cは積分変数) \\
  \end{align}
$$

## 総和

$\Sigma$ には `\sum` を使い，上付きと下付きで範囲を指定する．
```
$$
  \sum_{k = 1}^{5} k^2 = 1 + 4 + 9 + 16 + 25
$$
```
$$
  \sum_{k = 1}^{5} k^2 = 1 + 4 + 9 + 16 + 25
$$



## 三角関数，対数

$ \sin x, \cos x, \tan x $ ← `$ \sin x, \cos x, \tan x $`

$ \log x, \ln y, \log_{10} a $← `$ \log x, \ln y, \log_{10} a $`

## 行列

```
$$
    \begin{pmatrix}
        a & b \\
        c & d
    \end{pmatrix}
    \begin{pmatrix}
        x \\
        y
    \end{pmatrix}
    =
    \begin{pmatrix}
        ax + by \\
        cx + dy
    \end{pmatrix}
$$
```
$$
    \begin{pmatrix}
        a & b \\
        c & d
    \end{pmatrix}
    \begin{pmatrix}
        x \\
        y
    \end{pmatrix}
    =
    \begin{pmatrix}
        ax + by \\
        cx + dy
    \end{pmatrix}
$$

### 行列式

```
$$
    \begin{vmatrix}
        a_{11} & a_{12} & a_{13} \\
        a_{21} & a_{22} & a_{23} \\
        a_{31} & a_{32} & a_{33} \\
    \end{vmatrix}
    =
    \begin{matrix}
    a_{11}a_{22}a_{33}
    + a_{12}a_{23}a_{31}
    + a_{13}a_{21}a_{32}\\
    - a_{11}a_{23}a_{32}
    - a_{12}a_{21}a_{33}
    - a_{13}a_{22}a_{31}
    \end{matrix}
$$
```

$$
    \begin{vmatrix}
        a_{11} & a_{12} & a_{13} \\
        a_{21} & a_{22} & a_{23} \\
        a_{31} & a_{32} & a_{33} \\
    \end{vmatrix}
    =
    \begin{matrix}
    a_{11}a_{22}a_{33}
    + a_{12}a_{23}a_{31}
    + a_{13}a_{21}a_{32}\\
    - a_{11}a_{23}a_{32}
    - a_{12}a_{21}a_{33}
    - a_{13}a_{22}a_{31}
    \end{matrix}
$$