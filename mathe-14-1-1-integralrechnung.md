# Partielle Integration (Produktintegration)

Idee aus der Produktregel (Ableitung)

$$
f(x) = u(x) v(x)
$$$$
f'(x) = u'(x) v(x) + u(x) v'(x)
$$$$
f'(x) - u'(x) v(x) = u(x) v'(x) \text{ | integrieren}
$$$$
\int_a^b f'(x) - u'(x) v(x) = \int_a^b u(x) v'(x)
$$$$
\int_a^b f'(x) \mathrm{d}x - \int_a^b u'(x) v(x) \mathrm{d}x = \int_a^b u(x) v'(x) \mathrm{d}x
$$$$
[f(x)]_a^b - \int_a^b u'(x) v(x) \mathrm{d}x = \int_a^b u(x) v'(x) \mathrm{d}x
$$$$
[u(x) v(x)]_a^b - \int_a^b u'(x) v(x) \mathrm{d}x = \int_a^b u(x) v'(x) \mathrm{d}x \text{ (Regel für die partielle Integration)}
$$

## Nebenrechnung

$$
[f(x)]_{x=a}^{x=b} = f(x=b) - f(x=a)
$$$$
[u(x) v(x)]_a^b = u(b) v(b) - u(a) v(a)
$$

## Anwendung

$$
I = \int_a^b x \cos{x} \mathrm{d}x
$$$$
x = u(x)
$$$$
\cos{x} = v'(x)
$$

$$
u(x) = x
$$$$
u'(x) = 1
$$$$
v(x) = \sin{x}
$$$$
v'(x) = \cos{x}
$$

$$
I = [x \sin{x}]_a^b - \int_a^b 1 \cdot \sin{x} \mathrm{d}x
$$$$
I = [x \sin{x}]_a^b - [-\cos{x}]_a^b
$$$$
I = [x \sin{x} + \cos{x}]_a^b
$$

### Nebenrechnung

$$
f(x) = \sin{x}
$$$$
f'(x) = \cos{x}
$$$$
f''(x) = -\sin{x}
$$$$
f'''(x) = -\cos{x}
$$$$
f''''(x) = \sin{x} \text{ usw.}
$$

## Aufgabe 252/4

$$
I = \int_0^\pi x \sin{x} \mathrm{d}x
$$$$
u(x) = x
$$$$
u'(x) = 1
$$$$
v(x) = -\cos{x}
$$$$
v'(x) = \sin{x}
$$$$
I = [x \cdot (-\cos{x})]_0^\pi - \int_a^\pi -\cos{x} \mathrm{d}x
$$$$
I = [x \cdot (-\cos{x})]_0^\pi - [-\sin{x}]_0^\pi
$$$$
I = [x \cdot (-\cos{x}) + \sin{x}]_0^\pi
$$

## Aufgabe 252/5

(partielle Integration mehrfach anwenden)

$$
I = \int_a^b x^2 \cos{x} \mathrm{d}x
$$$$
a = -{\pi \over 2}
$$$$
b = {\pi \over 2}
$$$$
u(x) = x^2
$$$$
u'(x) = 2 x
$$$$
v(x) = \sin{x}
$$$$
v'(x) = \cos{x}
$$$$
I = [x^2 \sin{x}]_a^b - \int_a^b{2 x \sin{x}} \mathrm{d}x
$$$$
I = [x^2 \sin{x}]_a^b - ([2 x (-\cos{x})]_a^b - \int_a^b 2 (-\cos{x}) \mathrm{d}x)
$$$$
I = [x^2 \sin{x}]_a^b - ([2 x (-\cos{x})]_a^b - [2 (-\sin{x})]_a^b)
$$$$
I = [x^2 \sin{x}]_a^b - [2 x (-\cos{x}) - 2 (-\sin{x})]_a^b
$$$$
I = [x^2 \sin{x} - 2 x (-\cos{x}) - 2 (-\sin{x})]_a^b
$$$$
I = [x^2 \sin{x} + 2 x \cos{x} + 2 \sin{x}]_a^b
$$

----

**17.10.2014**

## Aufgabe 252/6 a)

(partielle Integration mehrfach anwenden)

$$
a = {-{\pi \over 2}}
$$$$
b = {\pi \over 2}
$$$$
I = \int_a^b (\sin{x})^2 \mathrm{d}x
$$$$
I = \int_a^b \sin{x} \sin{x} \mathrm{d}x
$$$$
u(x) = \sin{x}
$$$$
u'(x) = \cos{x}
$$$$
v(x) = -\cos{x}
$$$$
v'(x) = \sin{x}
$$$$
I = [\sin{x} \cdot (-\cos{x})]_a^b - \int_a^b \cos{x} \cdot (-\cos{x}) \mathrm{d}x
$$$$
I = [\cos{x} \cdot (-\sin{x})]_a^b - \int_a^b -(\sin{x}) \cdot (-\sin{x}) \mathrm{d}x
$$$$
I = [\cos{x} \cdot (-\sin{x})]_a^b - [\cos{x} \cdot (-\sin{x})]_a^b - [\cos{x} \cdot \cos{x}]_a^b
$$$$
I = [\cos{x} \cdot (-\sin{x}) - \cos{x} \cdot (-\sin{x}) - \cos{x} \cdot \cos{x}]_a^b
$$$$
I = [- \cos{x} \cdot \sin{x} + \cos{x} \cdot \sin{x} - \cos{x} \cdot \cos{x}]_a^b
$$$$
I = [- (\cos{x})^2 - \cos{x} \cdot \sin{x} + \cos{x} \cdot \sin{x}]_a^b
$$

## Aufgabe 252/7

(Stammfunktion ermitteln)

### a)

$$
f(x) = x \cdot (x - 1)^4
$$$$
u(x) = x
$$$$
u'(x) = 1
$$$$
v(x) = {1 \over 5} (x - 1)^5
$$$$
v'(x) = (x - 1)^4
$$$$
F(x) = x \cdot {1 \over 5} (x - 1)^5 - {1 \over 30} (x - 1)^6
$$

$$
F(x) = {1 \over 5} x (x - 1)^5 - {1 \over 30} (x - 1)^6 \text{ (Musterlösung)}
$$

### b)

$$
f(x) = (2 x + 5) \cdot (x + 2)^8
$$$$
u(x) = (2 x + 5)
$$$$
u'(x) = 1
$$$$
v(x) = {1 \over 9} (x + 2)^9
$$$$
v'(x) = (x + 2)^8
$$$$
F(x) = (2x + 5) {1 \over 9} (x + 2)^9 - {1 \over 90} (x + 2)^{10}
$$

$$
F(x) = (2x + 5) \cdot {1 \over 9} (x + 2)^9 - {2 \over 90} (x + 2)^{10} \text{ (Musterlösung)}
$$

### c)

$$
f(x) = \cos{x} \cdot (x - 1)
$$$$
u(x) = \cos{x}
$$$$
u'(x) = -\sin{x}
$$$$
v(x) = {1 \over 2} (x - 1)^2
$$$$
v'(x) = (x - 1)
$$$$
F(x) = \cos{x} \cdot {1 \over 2} (x - 1)^2 - \int (-\sin{x}) \cdot {1 \over 2} (x - 1)^2 \mathrm{d}x
$$

#### Nebenrechnung

$$
f(x) = (-\sin{x}) \cdot {1 \over 2} (x - 1)^2
$$$$
u(x) = -\sin{x}
$$$$
u'(x) = -\cos{x}
$$$$
v(x) = {1 \over 6} (x - 1)^3
$$$$
v'(x) = {1 \over 2} (x - 1)^2
$$$$
F(x) = (-\sin{x}) {1 \over 6} (x - 1)^3 - \int (-\cos{x}) {1 \over 6} (x - 1)^3 \mathrm{d}x
$$

$$
F(x) = \cos{x} + (x - 1) \cdot \sin{x} \text{ (Musterlösung)}
$$

# Integration durch Substitution

## Wiederholung

### Ketternregel

Sei $F(x)$ die Stammfunktion von $f(x)$ und $g(x)$ differenzierbar

$$
H(x) = F(g(x))
$$$$
H'(x) = f(g(x)) \cdot g'(x)
$$$$
\int_a^b f(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } [F(g(x))]_{x=a}^{x=b} \text{ | } g(x) = z
$$$$
\text{= } [F(z)]_{g(a)}^{g(b)} = \int_{g(a)}^{g(b)} f(z) \mathrm{d}z
$$

$$
c = g(a)
$$$$
d = g(b)
$$$$
\int_{g(c)}^{g(d)} f(g(x)) \cdot g'(x) \mathrm{d}x
$$

### Beispiel 1

$$
\int_0^2 {4 x \over \sqrt{1 + 2x^2}} \mathrm{d}x
$$$$
\text{= } \int_0^2 f(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } [F(z)]_{g(0)}^{g(2)} = 2 \cdot \sqrt{1 + 2 \cdot 2^2} - 2 \sqrt{1}
$$$$
\text{= } 6 - 2 = 4
$$

#### Nebenrechnung

$$
g(x) = 1 + 2x^2
$$$$
g'(x) = 4x
$$$$
f(g(x)) = f(z) = {1 \over \sqrt{z}} = z^{-{1 \over 2}}
$$$$
F(z) = 2z^{1 \over 2}
$$

### Beispiel 2

$$
h(x) = {x \over {2(1 + x^2)^2}}
$$$$
\int_a^b = {x \over {2(1 + x^2)^2}} \mathrm{d}x
$$$$
\text{= } \int_a^b f(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } {1 \over 4} \int_a^b f(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } {1 \over 4} [F(z)]_{g(a)}^{g(b)}
$$$$
\text{= } {1 \over 4} [- {1 \over {2 (1 + x^2)^2}}]_a^b
$$$$
H(x) = - {1 \over {8 \cdot (1 + x^2)^2}}
$$

#### Nebenrechnung

$$
g(x) = 1 + x^2
$$$$
g'(x) = 2x
$$$$
f(g(x)) = f(z) = {1 \over z^3}
$$$$
g'(x) \cdot f(z) = {2x \over z^3}
$$

## Hausaufgabe 254/3a

$$
f(x) = (3x - 4)^4
$$$$
z = g(x) = 3x - 4
$$$$
g'(x) = 3
$$$$
f(z) = z^4
$$$$
F(z) = {1 \over 5} z^5
$$$$
\int_a^b f(x) \mathrm{d}x
$$$$
\text{= } \int_a^b (3x - 4)^4 \mathrm{d}x
$$$$
\text{= } \int_a^b f(g(x) \mathrm{d}x
$$$$
\text{= } {1 \over 3} \cdot 3 \int_a^b f(g(x) \mathrm{d}x
$$$$
\text{= } {1 \over 3} \int_a^b f(g(x) \cdot 3 \mathrm{d}x
$$$$
\text{= } {1 \over 3} \int_a^b f(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } {1 \over 3} [F(z)]_{g(a)}^{g(b)}
$$$$
\text{= } {1 \over 3} [{1 \over 5} z^5]_{g(a)}^{g(b)}
$$$$
\text{= } {1 \over 3} [{1 \over 5} (3x - 4)^5]_a^b
$$$$
\text{= } [{1 \over 15} (3x - 4)^5]_a^b
$$$$
F(x) = {1 \over 15} (3x - 4)^5
$$

----

## Beispiel 3

$$
\int_0^{1 \over 2} {1 \over \sqrt{1 - x^2}} \mathrm{d}x
$$$$
\text{= } \int_0^{\pi \over 6} {1 \over \sqrt{1 - (\sin{t})^2}} \cos{t} \mathrm{d}x
$$$$
\text{= } \int_0^{\pi \over 6} {1 \over \cos{t}} \cdot \cos{t} \mathrm{d}t
$$$$
\text{= } \int_0^{\pi \over 6} 1 \mathrm{d}t = [t]_0^{\pi \over 6}
$$$$
\text{= } {\pi \over 6} - 0 = {\pi \over 6}
$$ 

### Nebenrechnung

$$
x = g(t) = \sin{t}
$$$$
g'(t) = \cos{t}
$$$$
g(t_1) = \sin{t_1} = 0 \rightarrow t_1 = 0
$$$$
g(t_2) = \sin{t_2} = {1 \over 2} \rightarrow t_2 = {\pi \over 6}
$$

### Nebenrechnnung 2

$$
(\sin{x})^2 + (\cos{x})^2 = 1
$$$$
\cos{x} = \sqrt{1 - (\sin{x})^2}
$$

----

**30.09.2014**

## Wiederholung

### Seite 254/3a

$$
f(x) = (3x - 4)^4
$$$$
g(x) = 3x - 4
$$$$
g'(x) = 3
$$$$
f(g(x)) \cdot g'(x)
$$$$
\int_{g(a)}^{g(b)} f(z) \mathrm{d}x = \int_a^b f(g(x)) g'(x) \mathrm{d}x
$$$$
f(x) = {1 \over 3} \int_{g(a)}^{g(b)} (3x-4)^4 \cdot 3 \mathrm{d}x
$$$$
F(z) = {1 \over 3} [{1 \over 5} (3x - 4)^5]_a^b
$$$$
\text{= } [{1 \over 15} (3x - 4)^5]_a^b
$$

## Seite 254/3b

$$
f(x) = {(2 - 5x)^3 \over 3}
$$

gesucht: Stammfunktion

$$
\int_a^b f(x) \mathrm{d}x = \int_a^b h(g(x)) \mathrm{d}x
$$

Form der Substitution noch nicht erreicht... ($g'(x)$ fehlt)

$$
\text{= } -5 \cdot {1 \over -5} \int_a^b h(g(x)) \mathrm{d}x
$$$$
\text{= } {1 \over -5} \int_a^b h(g(x)) \cdot (-5) \mathrm{d}x
$$$$
\text{= } {1 \over -5} \int_a^b h(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } {1 \over -5} \int_{g(a)}^{g(b)} h(z) \mathrm{d}z
$$$$
\text{= } {1 \over -5} \int_{g(a)}^{g(b)} {z^3 \over 3} \mathrm{d}z
$$$$
\text{= } {1 \over -5} [{z^4 \over 12}]_{g(a)}^{g(b)}
$$$$
\text{= } {1 \over -5} [{(2 - 5x)^4 \over 12}]_a^b
$$$$
\text{= } [- {(2 - 5x)^4 \over 60}]_a^b
$$$$
F(x) = - {1 \over 60} \cdot (2 - 5x)^4
$$

### Nebenrechnung

$$
g(x) = 2 - 5x
$$$$
g'(x) = -5
$$$$
h(x) = {x \over 3}
$$$$
f(x) = h(g(x))
$$

## Seite 254/3c

Ergebnis:

$$
F(x) = {2 \over 5 (5x + 1)} = {2 \over 25x + 5}
$$

## Seite 255/10

Bestimmen Sie eine Stammfunktion des Integranden und berechnen Sie damit das Integral. Überprüfen Sie ihr Ergebnis mit dem GTR.

### Vorraussetzung

$$
h(z) = {1 \over z} = z^{-1}
$$$$
H(z) = \ln{z} + c
$$

### a)

$$
\int_0^5 {2x \over 1 + x^2} \mathrm{d}x
$$$$
\text{= } \int_0^5 f(x) \mathrm{d}x
$$$$
\text{= } \int_0^5 h(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } [h(z)]_{g(0)}^{g(5)} = [\ln{1 + x^2}]_0^5
$$$$
\text{= } \ln{1 + 5^2} - \ln{1 + 0^2} = \ln{26} - 0 = \ln{26} \approx 3,26
$$$$
F(x) = \ln{1 + x^2}
$$

#### Nebenrechnung

$$
g(x) = 1 + x^2
$$$$
g'(x) = 2x
$$$$
h(z) = {1 \over z} = z^{-1}
$$$$
H(z) = \ln{z} + c
$$

### b)

$$
\int_1^3 {x^2 \over 1 + x^3} \mathrm{d}x
$$

### c)

$$
\int_1^4 {x - 3 \over x^2 - 6x} \mathrm{d}x
$$

### d)

$$
\int_0^{\pi \over 2} {\cos{x} \over 1 + \sin{x}} \mathrm{d}x
$$

## Seite 255/6a

$$
\int_0^2 \sqrt{4x - 2} \mathrm{d}x
$$$$
\text{= } {1 \over 4} \int_0^2 h(g(x)) \cdot g'(x) \mathrm{d}x
$$$$
\text{= } {1 \over 4} [H(z)]_{g(0)}^{g(2)} = {1 \over 4} [{2 \over 3} z^{3 \over 2}]_{g(0)}^{g(2)}
$$$$
\text{= } [{1 \over 6} z^{3 \over 2}]_{g(0)}^{g(2)}
$$$$
\text{= } {1 \over 6} (4 \cdot 2 - 2)^{3 \over 2} - {1 \over 6} (4 \cdot 0 - 2)^{3 \over 2} \text{ (nicht definiert...)}
$$$$
F(x) = {1 \over 6} {(4x - 2)}^{3 \over 2}
$$

### Nebenrechnung

$$
g(x) = 4x - 2
$$$$
g'(x) = 4
$$$$
h(z) = \sqrt{z} = z^{1 \over 2}
$$$$
H(z) = {2 \over 3} z^{3 \over 2}
$$

## Seite 255/6b

$$
\int_{-2}^{-1} {5 \over (2 - x)^2} \mathrm{d}x
$$$$
\text{= } {1 \over -2x + 4} \int_{-2}^{-1} h(g(x)) \cdot g'(x)
$$$$
\text{= } {1 \over -2x + 4} [H(z)]_{g(-2)}^{g(-1)}  
$$$$
\text{= } {1 \over -2x + 4} [5 \cdot \ln{z}]_{g(-2)}^{g(-1)}
$$$$
\text{= } [{1 \over -2x + 4} (5 \cdot \ln{z})]_{g(-2)}^{g(-1)}
$$$$
\text{= } [{5 \cdot \ln{z} \over -2x + 4}]_{g(-2)}^{g(-1)}
$$$$
F(x) = {5 \cdot \ln{z} \over -2x + 4}
$$$$
\text{= } -{5 \cdot \ln{z} \over 2x + 4}
$$

### Nebenrechnung

$$
g(x) = (2 - x)^2 = 4 + 4x - x^2
$$$$
g'(x) = -2x + 4
$$$$
h(z) = {5 \over z}
$$$$
H(z) = 5 \cdot \ln{z} + c
$$

# Wiederholung: Potenzregeln

$$
a^m \cdot a^n = a^{m+n}
$$$$
a^m \cdot b^m = (a \cdot b)^m
$$$$
(a^m)^n = a^{m \cdot n}
$$$$
a^{-n} = {1 \over a^n}
$$$$
a^{1 \over n} = \sqrt[n]{a}
$$$$
a^{- {1 \over n}} = {1 \over \sqrt[n]{a}}
$$
