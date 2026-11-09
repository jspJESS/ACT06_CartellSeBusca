# ACT06 · Cartell SE BUSCA

**Pràctica de Git i GitHub · Durada: 1 hora · Equip de sis alumnes**

## Repte

Entre tots preparareu les idees per a un cartell de **SE BUSCA**. Inventareu un personatge i decidireu què hi apareixerà: com és, on se l'ha vist, quina recompensa s'ofereix i quin aspecte tindrà el cartell.

Cada alumne aportarà idees al fitxer [`idees.md`](idees.md) des de la seva branca i les presentarà en una pull request. La professora revisarà les propostes i farà el merge. Treballareu per torns: cada persona comença quan la pull request anterior ja s'ha integrat a `main`.

L'objectiu de la pràctica és aprendre el flux de branques i pull requests mentre construïu una proposta conjunta. No cal programar ni fer una pàgina web.

## Abans de començar

- Comprova que la professora t'ha donat permís d'escriptura al repositori.
- Treballa només en el torn que t'ha tocat i edita la secció corresponent de `idees.md`.
- No facis commits directament a `main`.
- Inventeu un personatge fictici. No feu servir persones o animals reals, fotografies ni dades personals.
- Poseu-vos d'acord amb el grup perquè cada aportació encaixi amb les anteriors.

## Les sis aportacions

| Torn | Aportació a `idees.md` |
|---|---|
| 1 | Proposa tres personatges ficticis amb una frase sobre cadascun. El grup n'escull un i l'anota com a personatge triat. |
| 2 | Descriu el personatge triat amb tres característiques fàcils de reconèixer. |
| 3 | Inventa l'últim lloc i moment en què se l'ha vist, i una pista sobre què hi feia. |
| 4 | Proposa una recompensa divertida i no monetària. |
| 5 | Escriu un eslògan i indica què ha de fer qui trobi el personatge, sense incloure dades personals. |
| 6 | Proposa el disseny del cartell: colors, distribució, lletres i il·lustració. |

Cada alumne ha de fer una aportació concreta al seu torn. Les decisions es poden comentar entre tots, però l'alumne responsable les escriu al fitxer i les presenta a revisió.

## Passos per a cada alumne

### 1. Clona el repositori

Obre un terminal a la carpeta on vols desar el projecte i executa:

```bash
git clone https://github.com/jspJESS/ACT06_CartellSeBusca.git
cd ACT06_CartellSeBusca
```

### 2. Crea una branca per a la teva aportació

Per exemple, el primer torn pot fer:

```bash
git switch -c alumne-01-personatge
```

Adapta el nom al teu torn, per exemple `alumne-02-descripcio` o `alumne-06-disseny`.

### 3. Edita `idees.md` i comprova els canvis

Completa només la secció del teu torn. Després, comprova què has modificat:

```bash
git status
```

### 4. Crea un commit

```bash
git add idees.md
git commit -m "Afegeix idees per al cartell"
```

### 5. Puja la branca a GitHub

Canvia el nom de la branca pel que has creat al pas 2:

```bash
git push -u origin alumne-01-personatge
```

### 6. Obre una pull request

A GitHub, prem **Compare & pull request**. Comprova que:

- **base** sigui `main`;
- **compare** sigui la teva branca;
- el títol expliqui la teva aportació;
- la descripció expliqui què has afegit a `idees.md`.

Envia la pull request i espera la revisió de la professora. Si et demana una correcció, modifica el mateix fitxer a la mateixa branca, crea un altre commit i torna a fer `git push`. La pull request s'actualitzarà.

## Quan la professora hagi fet el merge

La persona següent actualitza `main` abans de crear la seva branca:

```bash
git switch main
git pull origin main
git switch -c alumne-02-descripcio
```

Canvia el nom de la branca pel del teu torn. Així partiràs de les idees que ja s'han acceptat.

## Comprovació final

Quan les sis pull requests estiguin integrades, llegiu `idees.md` entre tots i comproveu que el cartell té un personatge, una història, una recompensa, un eslògan i una proposta de disseny coherents.

**La professora revisa les pull requests i és qui fa el merge a `main`.**