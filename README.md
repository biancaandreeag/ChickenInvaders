> _Academic project developed as part of a university course._
___
# 🐔 Chicken Invaders

Implementare în **C++** a jocului clasic *Chicken Invaders*, rulat în consolă (terminal).

## 🎮 Controale

| Tastă     | Acțiune                                     |
| --------- | ------------------------------------------- |
| `a` / `d` | Mută nava la stânga / dreapta               |
| `Enter`   | Trage cu proiectil simplu                   |
| `o`       | Trage cu proiectil dublu (de la nivelul 2)  |
| `l`       | Trage cu laser (de la nivelul 6)            |
| `Space`   | Pauză                                       |
| `x`       | Ieșire din joc                              |

## 🎯 Dificultăți

| Mod       | Proiectile inamice simultane |
| --------- | :--------------------------: |
| EASY      | 3                            |
| MEDIUM    | 6                            |
| HARD      | 9                            |

## 🏆 Mecanici

- **10 nivele**, fiecare cu poziționare și proiectile diferite.
- **Nivelul 5 — Boss Level**: inamic special care generează random proiectile și coboară treptat (rezistă la 30 de proiectile).
- **Infinity Mode**: după nivelul 10, ultimul nivel se regenerează la infinit până când nava e atinsă.
- **Scor**: 10 puncte / găină distrusă.

## 🛠️ Implementare

- Scena e o singură matrice afișată în consolă, cu chenar și HUD (scor + nivel).
- Funcția `select_level` construiește nivelele într-un `switch`.
- Funcția `game_keys` gestionează input-ul.
- Proiectilele inamice sunt generate cu `rand()`, doar din găinile fără alta dedesubt (`ExistChicken`).
- Cursivitatea jocului a fost îmbunătățită înlocuind `system("cls")` cu o funcție de redesenare optimizată.
