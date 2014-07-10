% Mathematik - Unterichtsmitschriften
% Timm Albers
% 19.06.2014 - 10.07-2014

# Matrizen

## 431/2

**19.06.2014**

### a)

M mit *MA = A*, *AM = A*.

### b)

$$
E_n =
\begin{pmatrix}
  1 & 0 & \cdots & 0 \\
  0 & 1 & \cdots & 0 \\
  \vdots & \vdots & \ddots & \vdots \\
  0 & 0 & \cdots & 1
\end{pmatrix}
$$$$
A = (a_{ij}) = 
\begin{pmatrix}
  a_{11} & a_{12} & \cdots & a_{1m} \\
  a_{21} & a_{22} & \cdots & a_{2m} \\
  \vdots & \vdots & \ddots & \vdots \\
  a_{n1} & a_{n2} & \cdots & a_{nm}
\end{pmatrix}
$$$$
A E_{m} =
\begin{pmatrix}
  a_{11} & a_{12} & \cdots & a_{1m} \\
  a_{21} & a_{22} & \cdots & a_{2m} \\
  \vdots & \vdots & \ddots & \vdots \\
  a_{n1} & a_{n2} & \cdots & a_{nm}
\end{pmatrix} =
A
$$$$
E_{n} A = A \quad \text{(wie oben)}
$$

## 431/3

**19.06.2014**

### a)

$$
A B = B A = E_3 \quad \text{A und B sind zueinander invers}
$$

#### Nebenbetrachtung

##### Addition

$$
a + (-a) = 0  \quad \text{a und (-a) sind zueinander invers; 0 ist das neutrale Element}
$$

##### Multiplikation

$$
a {1 \over a} = 1  \quad \text{a und (1/a) sind zueinander invers; 1 ist das neutrale Element}
$$

### b)

$$
A =
\begin{pmatrix}
  2 & 1 \\
  -1 & -1
\end{pmatrix}
$$$$
B \text{ gesucht mit } A B = E_2
$$$$
B =
\begin{pmatrix}
  a & b \\
  c & d
\end{pmatrix} =
\begin{pmatrix}
  1 & 1 \\
  -1 & -2
\end{pmatrix}
$$$$
A B = E_2
$$$$
A B =
\begin{pmatrix}
  2a+c & 2b+d \\
  -a-c & -b-d
\end{pmatrix} =
\begin{pmatrix}
  1 & 0 \\
  0 & 1
\end{pmatrix}
$$$$
2a+c = 1
$$$$
2b+d = 0
$$$$
-a-c = 0
$$$$
-b-d = 1
$$

=> lösen (z.B. Additionsverfahren)

## Abbildungen mit Matrizen

**19.06.2014**

[Skizze]()

---

$$
f(x) = x \quad \text{(Identität)}
$$$$
y = x
$$$$
\vec{x} = \lambda {(1 \choose 1)}
$$$$
d = d'
$$

---

$$
P(3 | 1)
$$$$
P'(1 | 3)
$$$$
Q(x_1 | y_1)
$$$$
Q'(y_1 | x_1)
$$

---

[Skizze]()

$$
g: \vec{x} = {\lambda {1 \choose 2}} \quad \text{(Ursprungsgerade)}
$$$$
P(4 | 3)
$$$$
P'(0 | 5)
$$

---

$$
P(p_1 | p_2)
$$$$
g: \vec{x} = {\lambda {r_1 \choose r_2}}
$$$$
\text{Lotgerade (duch P und P } \perp \text{ g)}
$$$$
{r_1 \choose r_2} {l_1 \choose l_2} = 0
$$$$
r_1 l_1 + r_2 l_2 = 0
$$

z.B.

$$
l_1 = r_2
$$$$
l_2 = -r_1
$$$$
{r_1 \choose r_2} {r_2 \choose -r_1} = 0
$$$$
({r_2 \choose -r_1} \quad \text{Richtungsvektor für l})
$$$$
l: \vec{x} = {p_1 \choose p_2} + \lambda {r_2 \choose -r_1}
$$

Schnittpunkt F berechnen durch Gleichsetzen

$$
\lambda_1 {r_1 \choose r_2} = {p_1 \choose p_2} + \lambda_2 {r_2 \choose -r_1}
$$$$
\lambda_1 = {{p_1 r_1 + p_2 r_2} \over {r_1^2 + 2_2^2}}
$$$$
\lambda_2 = {{p_2 r_1 - p_1 r_2} \over {r_1^2 + r_2^2}}
$$$$
\vec{OP'} = {p_1 \choose p_2} + 2 \lambda_2 {r_2 \choose -r_1}
$$$$
\vec{OP'} = {p_1 \choose p_2} + 2 {{p_2 r_1 - p_1 r_2} \over {r_1^2 + r_2^2}} {r_2 \choose -r_1}
$$$$
\vec{OP'} = {1 \over {r_1^2 + r_2^2}} {{(r_1^2 - r_2^2) p_1 + 2 r_1 r_2 p_2} \choose {2 r_1 r_2 p_1 + (r_2^2 - r_1^2) p_2}}
$$$$
\vec{OP'} = {1 \over {r_1^2 + r_2^2}}
\begin{pmatrix}
  r_1^2 - r_2^2 & 2 r_1 r_2 \\
  2 r_1 r_2 & r_2^2 - r_1^2
\end{pmatrix} {p_1 \choose p_2}
$$

$$
({1 \over {r_1^2 + r_2^2}}
\begin{pmatrix}
  r_1^2 - r_2^2 & 2 r_1 r_2 \\
  2 r_1 r_2 & r_2^2 - r_1^2
\end{pmatrix}) \quad (\text{Transformationsmatrix für eine Spiegelung an } \vec{x} = \lambda {r_1 \choose r_2})
$$

**HA:** Rechnung mit allen Zwischenschritten rechnen!

## 435/3

**02.07.2014**

### a)

$$
\vec{OP} = {x \choose y}
$$$$
\vec{OP'} = ? \quad \text{gedreht um 90 Grad}
$$$$
M = ?
$$$$
M * \vec{OP} = \vec{OP'}
$$$$
\vec{OP'} = {-y \choose x}
$$$$
M_{90} = 
\begin{pmatrix}
  {-{y \over x}} & 0 \\
  0 & {x \over y}
\end{pmatrix} =
\begin{pmatrix}
  0 & -1 \\
  1 & 0
\end{pmatrix}
$$

### b)

$$
\vec{OP''} = {-x \choose -y} \quad \text{gedreht um 180 Grad}
$$$$
M_{180} = 
\begin{pmatrix}
  -1 & 0 \\
  0 & -1
\end{pmatrix}
$$

### c)

$$
\vec{OP'''} = {y \choose -x} \quad \text{gedreht um 270 Grad}
$$$$
M_{180} = 
\begin{pmatrix}
  {y \over x} & 0 \\
  0 & {-{x \over y}}
\end{pmatrix} = 
\begin{pmatrix}
  0 & 1 \\
  -1 & 0
\end{pmatrix}
$$

## 435/4

**02.07.2014**

$$
\vec{OP} = {x \choose y} = {r \cos{\alpha} \choose r \sin{\alpha}}
$$$$
M * \vec{OP} = \vec{OP'}
$$$$
x = r \cos{\alpha}
$$$$
y = r \sin{\alpha}
$$$$
\vec{OP'} = {{r (\cos{\alpha + \varphi})} \choose {r (\sin{\alpha + \varphi})}} = {{r (\cos{\alpha} \cos{\varphi} - \sin{\alpha} \sin{\varphi})} \choose r (\sin{\alpha} \cos{\varphi} + \cos{\alpha} \sin{\varphi})}
$$$$
M = 
\begin{pmatrix}
  {r (\cos{\alpha} \cos{\varphi} - \sin{\alpha} \sin{\varphi}) \over r \cos{\alpha}} & 0 \\
  0 & {r (\sin{\alpha} \cos{\varphi} + \cos{\alpha} \sin{\varphi}) \over r \sin{\alpha}}
\end{pmatrix} =
\begin{pmatrix}
  {r (\cos{\alpha + \varphi}) \over r \cos{\alpha}} & 0 \\
  0 & {r (\sin{\alpha + \varphi}) \over r \sin{\alpha}}
\end{pmatrix}
$$$$
\alpha = \tan^{-1} {x \over y}
$$$$
r = \sqrt{x^2 + y^2}
$$$$
M =
\begin{pmatrix}
  {\sqrt{x^2 + y^2} \cos{(\tan^{-1} {x \over y} + \varphi)}} \over {\sqrt{x^2 + y^2} - \cos{(\tan^{-1} {x \over y})}} & 0 \\
  0 & {\sqrt{x^2 + y^2} \sin{(\tan^{-1} {x \over y} + \varphi)}} \over {\sqrt{x^2 + y^2} - \sin{(\tan^{-1} {x \over y})}}
\end{pmatrix}
$$$$
M =
\begin{pmatrix}
  {\cos{(\tan^{-1} {x \over y} + \varphi)}} \over {\cos{(\tan^{-1} {x \over y})}} & 0 \\
  0 & {\sin{(\tan^{-1} {x \over y} + \varphi)}} \over {\sin{(\tan^{-1} {x \over y})}}
\end{pmatrix}
$$$$
M =
\begin{pmatrix}
  {\cos{(\tan^{-1} {x \over y}) \cos{\varphi}} - \sin{(\tan^{-1} {x \over y}) \sin{\varphi}}} \over {\cos{(\tan^{-1} {x \over y})}} & 0 \\
  0 & {\sin{(\tan^{-1} {x \over y}) \cos{\varphi}} - \cos{(\tan^{-1} {x \over y}) \sin{\varphi}}} \over {\sin{(\tan^{-1} {x \over y})}} 
\end{pmatrix}
$$$$
M =
\begin{pmatrix}
  \cos{\varphi} - {{\sin{(\tan^{-1} {x \over y}) \sin{\varphi}} \over \cos{(\tan^{-1} {x \over y})}}} & 0 \\
  0 & \cos{\varphi} - {{\cos{(\tan^{-1} {x \over y}) \sin{\varphi}} \over \sin{(\tan^{-1} {x \over y})}}}
\end{pmatrix}
$$

### Neuer Ansatz

$$
M =
\begin{pmatrix}
  {r \cos{\alpha} \cos{\varphi} - r \sin{\alpha} \sin{\varphi}} \over {r \cos{\alpha}} & 0 \\
  0 & ...
\end{pmatrix}
$$$$
M =
\begin{pmatrix}
  {r \cos{\alpha} \cos{\varphi} - r \sin{\alpha} \sin{\varphi}} \over {r x} & 0 \\
  0 & ...
\end{pmatrix}
$$$$
M =
\begin{pmatrix}
  {x \cos{\varphi} - y \sin{\varphi}} \over {r x} & 0 \\
  0 & {x \sin{\varphi} - y \cos{\varphi}} \over {r y}
\end{pmatrix}
$$$$
\vec{OP'} = {{x \cos{\varphi} - y \sin{\varphi}} \choose {x \sin{\varphi} + y \cos{\varphi}}}
$$$$
M =
\begin{pmatrix}
  \cos{\varphi} & -\sin{\varphi} \\
  \sin{\varphi} & \cos{\varphi}
\end{pmatrix}
$$

# Integralrechnung

## Aufgabe
**08.07.2014**

Bestimmen Sie den Flächeninhalt zwischen 0 und 1 zwischen $$f(x)=x^2$$ und der x-Achse näherungsweise.

(Untersumme)

$$
a = 0 \quad \text{Start}
$$$$
b = 1 \quad \text{Ende}
$$$$
f(x) = x^2 \quad \text{Funktion}
$$$$
n = 10 \quad \text{Anzahl der Rechtecke}
$$$$
h = {b-a \over n}
$$$$
A = h f(0) + h f(h) + h f(2h) + ... + h f((n-1) h)
$$$$
A = h (f(0) + f(h) + f(2h) + ... + f((n-1) h))
$$$$
A = (\sum_{i=0}^{n=1} f(ih)) h
$$

## Bestimmtes Integral

$$
\lim_{n \to \infty} (\sum_{i=0}^{n=1} f(ih)) = \int_a^b f(x) \mathrm{d}x
$$

**gesprochen:** Integral von a bis b über f(x) dx

## Vergleich mit dem Differentialquotienten

$$
\lim_{\Delta x \to 0} {\Delta y \over \Delta x} \quad \text{Grenzwert des Differenzenquotienten}
$$$$
{= \lim_{h \to 0} {f(x) - f(x + h) \over h}}
$$$$
{= {\mathrm{d} f(x) \over \mathrm{d}x}} \quad \text{Differentialquotient (gesprochen d f von x nach dx)}
$$

## Hauptsatz der Differenzial- und Integralrechnung

Ist die Funktion f stetig, so ist die Integralfunktion Ia mit

$$
I_a(x) = \int_a^b f(t) \mathrm{d}t
$$

differenzierbar und die Ableitung ist gleich der Integralfunktion f:

$$
I_a'(x) = f(x)
$$

---

**09.07.2014**

$$
I_a(x) = \int_a^x f(t) \mathrm{d}t
$$$$
I_a'(x) = {\mathrm{d} I_a(x) \over \mathrm{d}x} = f(x)
$$

### Beweis

[Tafelbild](mathe/2014-07-09-tafel-1.jpg)

$$
I_a'(x) = {\lim_{h \to 0} {I_a(x+h) - I_a(x) \over h}}
$$$$
{= \lim_{h \to 0} {\int_a^{x+h} f(t) \mathrm{d}t - \int_a^x f(t) \mathrm{d}t \over h}}
$$$$
{= \lim_{h \to 0} {{\int_x^{x+h} f(t) \mathrm{d}t} \over h} = \lim_{h \to 0} {f(z) h \over h} = \lim_{h \to 0} f(z) = f(x)} \quad \text{q.e.d.}
$$

grobe Näherung für

$$
\int_x^{x+h} f(t) \mathrm{d}t \quad \text{ist} \quad f(z) h
$$

mit

$$
x \leq z \leq x+h
$$

wobei für h gegen 0 dann z gegen x läuft und f(z) gegen f(x).

(siehe Tafelbild)

### Aufgabe 224/2

[Tafelbild](mathe/2014-07-09-tafel-2.jpg)

### Aufgabe 242/5

![Tafelbild](mathe/2014-07-09-aufgabe-1.jpg)

![Tafelbild](mathe/2014-07-09-aufgabe-2.jpg)

## Stammfunktion

**10.07.2014**

### Definition

Die Integralfunktion

$$
I_0(x)
$$

zur Integrantenfunktion

$$
f(x)
$$

wird eine *Stammfunktion* genannt.

### Notation

*F(x)* Stammfunktion zu *f(x)* (d.h. *F'(x) = f(x)*)

### Zusatz

$$
F(x) = I_0(x) + c
$$

(*c* = Integrationskonstante)

weil konstante Summanden beim Ableiten wegfallen:

$$
F'(x) = I_0'(x)
$$

### Aufgabe 242/6

#### a)

$$
f(t) = 2t - 4
$$$$
I_0 = t^2 - 4 t
$$

#### b)

$$
f(t) = 60 t + 200
$$$$
I_0 = 30 t^2 + 200 t
$$

#### c)

$$
f(t) = 3 t^2
$$$$
I_0 = t^3
$$

#### d)

$$
f(t) = 4 t^3
$$$$
I_0 = t^4
$$

### Aufgabe

Bestimmen Sie

$$
A = \int_{-1}^1 f(x) \mathrm{d}x \quad \text{mit } f(x) = x^3 - x
$$$$
F(x) = {1 \over 4} x^4 - {1 \over 2} x^2 + c
$$$$
A = \int_{-1}^1 {x^3 - x \mathrm{d}x}
$$$$
A = [{1 \over 4} x^4 - {1 \over 2} x^2 + c]_{-1}^1
A = {1 \over 4} 1^4 - {1 \over 2} 1^2 + c - {({1 \over 4} (-1)^4 - {1 \over 2} (-1)^2 + c)}
$$$$
A = 0
$$

**Begriff:** orientierter Flächeninhalt (positiv wie negativ)