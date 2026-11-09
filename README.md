# ACT06 · Cartell SE BUSCA

**Pràctica de Git i GitHub · Durada: 1 hora · Treball en equip de sis alumnes**

## Repte

Entre tots creareu un cartell digital de **SE BUSCA**. El grup decidirà quin personatge fictici busca, com és, on se l'ha vist, quina recompensa s'ofereix i quin aspecte tindrà el cartell.

Cada alumne farà **una aportació en una branca pròpia** i l'enviarà a la professora mitjançant una pull request. La professora revisarà i farà el merge. Treballareu per torns: cada persona comença quan la pull request anterior ja s'ha integrat a `main`.

## Abans de començar

- Comprova que la professora t'ha donat permís d'escriptura al repositori.
- Treballa només en la tasca que t'ha tocat i edita el fitxer que s'indica.
- No facis commits directament a `main`.
- El personatge ha de ser inventat o fictici. No feu servir persones o animals reals, fotografies ni dades personals.

## Les sis aportacions

| Torn | Aportació | Fitxer |
|---|---|---|
| 1 | Trieu o inventeu el personatge, poseu-li nom i expliqueu breument per què se'l busca. | `index.html` |
| 2 | Afegiu una descripció amb tres característiques que ajudin a reconèixer-lo. | `index.html` |
| 3 | Inventeu l'últim lloc i moment en què se l'ha vist. | `index.html` |
| 4 | Decidiu una recompensa divertida i no monetària. | `index.html` |
| 5 | Expliqueu què ha de fer qui el trobi. No hi poseu telèfons ni dades personals. | `index.html` |
| 6 | Milloreu el disseny del cartell amb CSS: colors, tipografia, espais i bona lectura en mòbil. | `style.css` |

Abans de cada aportació, parleu breument amb el grup per mantenir una mateixa història. La persona del torn 1 proposa el personatge; les següents poden donar idees i fer comentaris, però cada torn presenta una millora concreta.

## Passos per a cada alumne

### 1. Clona el repositori

Obre un terminal a la carpeta on vols desar el projecte i executa:

```bash
git clone https://github.com/jspJESS/ACT06_CartellSeBusca.git
cd ACT06_CartellSeBusca
```

### 2. Crea la teva branca

Fes servir un nom que indiqui el teu torn i la tasca. Per exemple, per al primer torn:

```bash
git switch -c alumne-01-personatge
```

Adapta el nom al teu torn, per exemple `alumne-02-descripcio` o `alumne-06-disseny`.

### 3. Fes la teva aportació

Edita només la part del fitxer que correspon a la teva tasca. Desa els canvis i comprova'ls:

```bash
git status
```

### 4. Desa els canvis amb un commit

Per a les tasques 1–5:

```bash
git add index.html
git commit -m "Afegeix una millora al cartell"
```

Per a la tasca 6:

```bash
git add style.css
git commit -m "Millora el disseny del cartell"
```

### 5. Puja la branca a GitHub

Canvia el nom de la branca pel que has creat al pas 2:

```bash
git push -u origin alumne-01-personatge
```

### 6. Obre una pull request

A GitHub, obre el repositori i prem **Compare & pull request**. Comprova que:

- **base** sigui `main`;
- **compare** sigui la teva branca;
- el títol expliqui la millora;
- la descripció expliqui què has canviat.

Envia la pull request i espera la revisió de la professora. Si et demana una correcció, fes-la a la mateixa branca, crea un altre commit i torna a fer `git push`. La pull request s'actualitzarà.

## Quan la professora hagi fet el merge

La persona següent ha d'actualitzar `main` abans de crear la seva branca:

```bash
git switch main
git pull origin main
git switch -c alumne-02-descripcio
```

Canvia el nom de la branca pel del teu torn. Així partiràs del cartell actualitzat amb les aportacions acceptades.

## Comprovació final

Quan les sis pull requests estiguin integrades:

1. Obre `index.html` al navegador.
2. Comproveu que el cartell explica una història coherent i no queda cap text entre claudàtors.
3. Reviseu que es llegeixi bé en una pantalla petita.

**La professora és qui fa el merge a `main`.**