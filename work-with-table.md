# Задание ИТ
**Решите уравнение 𝒂𝒙 ± 𝒃 = 0**
```python
cifra = input('ввод ')
w = cifra.find('x')
g = cifra.find('=')
if w == 0:
    a = 1
elif w == 1 and cifra[0] == '-':
    a = -1
else:
    a = int(cifra[:w])
b = int(cifra[
    (w+1):g])
if a < -1000 or a > 1000 or b < -1000 or b > 1000:
        print('Числа по модулю должно быть меньше 1000')
elif a == 0 and b == 0:
        print ('вывод INF')
elif a == 0 and b != 0:
        print ('вывод NO')
else:
        print ('вывод', -b / a)
```
[гиперссылка Аллы](https://github.com/AngryMoth)
