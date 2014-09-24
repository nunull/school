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