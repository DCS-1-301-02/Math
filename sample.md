# マークダウンでの数式の記述のサンプル

プレビューで見ると，左側が数式，右側がその記述になります．

マークダウンの表の中に `$$` で囲んだ数式を入れるときは，**途中で改行せず**一行にする必要があります． 複雑になると読みにくいですが，分けて考えてください．

| 数式 | 記述 |
|----|----|
|$$ x^2+y_1+z_{12} $$|`$$ x^2+y_1+z_{12} $$`|
|$$ sin^{-1}(x) $$|`$$ sin^{-1}(x) $$no`|
|$$ f(x)=\sum_{n=0}^\infty\frac{f^{(n)}(a)}{n!}(x-a)^n $$ | `$$ f(x)=\sum_{n=0}^\infty\frac{f^{(n)}(a)}{n!}(x-a)^n $$` |
|$$ \int_0^1 f(x)dx $$ | `$$ \int_0^1 f(x)dx $$` | 
|$$ x/x=\begin{cases} 1 & \text{if } x \neq 0 \\ \text{undefined} & \text{if } x = 0\end{cases} $$ | `$$ x/x=\begin{cases}1 & \text{if } x \neq 0 \\ \text{undefined} & \text{if } x = 0\end{cases} $$` |
| $$ (a,b]=\{x \in \mathbb{R} \| a < x \le b\} $$ | `$$ (a,b]=\{x \in \mathbb{R} \| a < x \le b\} $$` |

### 等号の位置を揃える

例)

$f(x) = x^3-x^2-3x+3 $ を$[0,2]$の範囲で積分する．

$$
\begin{aligned}
    \int_0^2 f(x) dx 
    &= \int_0^2 (x^3-x^2-3x+3) dx \\
    &= \left[\frac{1}{4} x^4-\frac{1}{3} x^3-\frac{3}{2} x^2+3x\right]_0^2 \\
    &= \left(\frac{1}{4} 2^4-\frac{1}{3} 2^3-\frac{3}{2} 2^2+3\cdot 2\right) 
    - \left(\frac{1}{4} 0^4-\frac{1}{3} 0^3-\frac{3}{2} 0^2+3\cdot 0\right) \\
    &= \left(4 - \frac{8}{3} - 6 + 6\right)\\
    &= \frac{4}{3}
\end{aligned}
$$

```
$$
\begin{aligned}
    \int_0^2 f(x) dx 
    &= \int_0^2 (x^3-x^2-3x+3) dx \\
    &= \left[\frac{1}{4} x^4-\frac{1}{3} x^3-\frac{3}{2} x^2+3x\right]_0^2 \\
    &= \left(\frac{1}{4} 2^4-\frac{1}{3} 2^3-\frac{3}{2} 2^2+3\cdot 2\right) 
    - \left(\frac{1}{4} 0^4-\frac{1}{3} 0^3-\frac{3}{2} 0^2+3\cdot 0\right) \\
    &= \left(4 - \frac{8}{3} - 6 + 6\right)\\
    &= \frac{4}{3}
\end{aligned}
$$
```