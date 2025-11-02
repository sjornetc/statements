# 📘 Enunciats de `lliurator`

Aquest repositori conté els **enunciats** d’activitats del projecte `lliurator`, escrits en format Markdown (`.md`) i publicats sota llicència **[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.ca)**.

Cada arxiu correspon a una activitat concreta i es troba a la ruta:

```
<modul>/<apartat>/.../<nom>.md
```

Per exemple:
```
0369/RA3/2/a1.md
```

## ✏️ Format dels arxius

Els fitxers segueixen una sintaxi Markdown amb algunes **notacions pròpies** per indicar blocs d’informació o tipus de resposta esperada.

### 🪄 Blocs especials

| Notació | Significat | Exemple |
|----------|-------------|----------|
| `>i [text]` | Bloc **informatiu** o aclaridor. | `>i Aquest apartat no es puntua.` |
| `>w [text]` | Bloc d’**advertència** o error comú. | `>w Compte: no editis aquest arxiu directament.` |

*(poden renderitzar-se amb estils diferents al lliurator)*

### ❓ Indicadors de resposta esperada

Cada activitat pot contenir línies que comencen amb `?`, que indiquen el **tipus de resposta** i la **puntuació** assignada.

```
? <tipus_de_resposta> <puntuació>[/<penalització>]
```

on `<penalització>` és la resta de punts si la resposta és incorrecta (opcional).

#### 🔤 Tipus de resposta

| Tipus | Descripció |
|--------|-------------|
| `tf` | Pregunta de **true/false**. |
| `choice` | Pregunta de **selecció múltiple** (vegeu exemple). |
| `txt` | Resposta escrita breu o paràgraf. |
| `num` | Resposta numèrica (admet decimals). |
| `link` | Enllaç o URL com a resposta. |
| `code:<llenguatge>` | Bloc de codi d’un llenguatge concret (p. ex. `code:python`). |
| `file` | S’espera un **arxiu adjunt** (codi, imatge, etc.). |
| `img` | S’espera una imatge (captura, gràfic, etc.). |
| `bash` | Resposta **interactiva**: comanda o script Bash. |


##### Exemple `choice`
```
? choice 1/0.333
<Opció a>
<Opció b>
<Opció c>
```

## 📂 Estructura recomanada

```
<modul>/
 ├─ RA1/
 │   ├─ 1/
 │   │   └─ a1.md
 │   └─ 2/
 │       └─ a2.md
 └─ RA2/
     └─ ...
```

Les carpetes `<modul>` han de correspondre al codi del mòdul, és a dir, quatre números (`[0-9]{4}`)

La estructura interna depen de les necessitats del mòdul, sols es poden fer servir lletres i números a les carpetes i noms d'enunciats (`[A-Za-z0-9]+`).

Cada enunciat té un codi identificatiu que es fa servir a `lliurator` i que correspon a la ruta fins a l'enunciat fent servir `_` en lloc de `/` i sense extensió (`^[0-9]{4}(_[A-Za-z0-9]+)+$`)

```
0369/RA3/2/a1.md
    ↓   ↓ ↓   ↓
0369_RA3_2_a1
```

## 🪪 Llicència

Tot el contingut d’aquest repositori està sota llicència **Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)**. 

El contingut està creat per Sara Jornet Calomarde, tret que l'enunciat indiqui el contrari

## 💬 Contribucions

Les propostes de nous enunciats o correccions són benvingudes mitjançant *pull requests*.

---

💛 *Fet amb la convicció de que l’educació pública i oberta només és real quan el coneixement és compartit i tothom hi pot accedir sense barreres.*
