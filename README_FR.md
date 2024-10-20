# 🌌 **Isotope Pathways** — Pisteur des routes invisibles

> **"Y a-t-il quelqu'un dans ce monde capable de voir l'invisible ? Non ? Eh bien, ce programme peut. Il capte les traces radioactives, comme un vieux chaman lisant les cendres, et les affiche sur l'écran – colorées, scintillantes, vivantes."**

---

## 📖 **À propos du projet**

**Isotope Pathways** n'est pas seulement un programme, c'est un monde entier de particules invisibles qui deviennent enfin visibles. Imaginez : vous marchez sur un chemin, et sous vos pieds dansent des isotopes radioactifs. Ce programme vous permet de les voir. Il dessine une carte où chaque isotope laisse sa trace, du vert au rouge, du calme à l'alarme.

Il peut lire les données provenant des fichiers AtomFast et RadiaCode aux formats `.kml`, `.kmz`, `.json` et `.rctrk`, les enregistrer dans sa base de données, pour que, des années plus tard, vous puissiez dire : « À cet endroit, en 2024, il y avait 4.1 µR/h ».

### 🌍 **Sur la base de la nature**

Nous avons pris comme référence le **rayonnement naturel de fond**. Si vous allez dans un endroit pur et intact, vous verrez probablement **3 à 4 microroentgen par heure**. C'est la norme. À chaque altitude, son niveau de radiation, et la Terre semble s'en accommoder.

Tout ce qui dépasse ce fond naturel est considéré comme **étranger**. Nous appelons cela la **contamination radioactive**. Vous pouvez voir sur la carte comment les isotopes se dispersent sur les routes, emportés par le vent, les gens et les véhicules. Ce sont des traces invisibles, comme des empreintes de pas dans la neige fraîche.

---

### 📸 **Démonstration**

<a href="https://jutsa.ru" target="_blank">Cliquez ici pour voir le programme en temps réel.</a>

### 📸 **Captures d'écran**

Dans les années soviétiques, ils construisaient une piscine en plein air dans le parc de Kislovodsk. Peut-être ont-ils utilisé du béton provenant d'une usine à Piatigorsk, où on traitait jadis du minerai radioactif de la montagne Besh-tau. Les camions qui passaient laissaient des traces invisibles sur l'asphalte. Des années ont passé, mais ces traces brillent encore, comme des souvenirs du passé. La poussière s'est déposée autour du chantier, et dans le parc, elle apparaît en jaune sur la carte, comme les feuilles d'automne. Tout le reste du parc est propre, paisible, vert.

<img src="https://repository-images.githubusercontent.com/870016860/11fd6abc-fe8b-4cd8-95c2-df1c631c8762">

---

## 📥 **Télécharger et commencer** 📥

Choisissez la version pour votre plateforme et commencez à suivre les traces des isotopes :

| Plateforme | Lien de téléchargement                                                                                 |
|------------|-------------------------------------------------------------------------------------------------------|
| AIX        | [Télécharger pour AIX](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/aix/)                  |
| Android    | [Télécharger pour Android](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/android/)           |
| Dragonfly  | [Télécharger pour Dragonfly](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/dragonfly/)       |
| FreeBSD    | [Télécharger pour FreeBSD](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/freebsd/)           |
| Illumos    | [Télécharger pour Illumos](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/illumos/)           |
| JavaScript | [Télécharger pour JavaScript](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/js/)             |
| Linux      | [Télécharger pour Linux](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/linux/)               |
| macOS      | [Télécharger pour macOS](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/mac/)                 |
| NetBSD     | [Télécharger pour NetBSD](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/netbsd/)             |
| OpenBSD    | [Télécharger pour OpenBSD](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/openbsd/)           |
| Plan9      | [Télécharger pour Plan9](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/plan9/)               |
| Solaris    | [Télécharger pour Solaris](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/solaris/)           |
| Windows    | [Télécharger pour Windows](http://files.zabiyaka.net/isotope-pathways/latest/no-gui/windows/)           |

Ou compilez-le vous-même :

```bash
git clone https://github.com/matveynator/isotope-pathways.git
cd isotope-pathways
go build isotope-pathways.go
chmod +x ./isotope-pathways
./isotope-pathways
```

---

## 🛠 **Comment utiliser ?**

### Lancer le programme :

```bash
./isotope-pathways
```

Ou avec des options supplémentaires :

```bash
./isotope-pathways --port=8765 --db-type=genji --db-path=./path-to-database-file.8765.genji
```

- `--port` : Le port sur lequel le serveur sera lancé. Par défaut `8765`.  
  _"Envie de changer de port ? Changez-le, et le programme communiquera avec vous autrement."_

- `--db-type` : Type de base de données : `genji` ou `sqlite`. Par défaut `genji`.  
  _"Préférez-vous le classique SQLite ou l'innovant Genji ? Faites votre choix."_

- `--db-path` : Chemin vers le fichier de base de données. Si non précisé, il sera créé dans le répertoire actuel.  
  _"Où cacher les traces ? Dans quel coin du disque ? Indiquez le chemin, et il deviendra leur refuge."_

- `--version` : Affiche la version du programme et quitte.  
  _"Comme un vieux magicien, le programme vous dira de quelle époque il vient."_

### Interface Web :

1. Ouvrez <a href="http://localhost:8765" target="new">http://localhost:8765</a> dans votre navigateur.
2. Téléchargez des données en utilisant le bouton `Upload`.
3. Survolez un marqueur et découvrez un monde invisible. Connaissez la dose de radiation, l'heure de la mesure et l'endroit où les isotopes ont laissé leurs marques.

---

## ☢️ **La radiation et ses traces**

Qu'est-ce que la radiation ? C'est comme le souffle du vent dans les montagnes que personne n'entend, mais qui est bien là. Et notre programme est comme une personne dotée d'une ouïe exceptionnelle. Il voit ce que vous ne pouvez pas voir. Il vous dira où et quand ce microsievert supplémentaire a été là. Il vous montrera comment les isotopes se sont dispersés à travers la ville, comment ils ont atterri dans un étang calme ou se sont perdus dans une vieille forêt. Leur danger réside dans le fait qu'ils ne restent pas simplement sur le sol, comme une pièce de monnaie oubliée. Non, ils pénètrent dans le sol, l'eau, les plantes. Vous vivez paisiblement, mangez des pommes, buvez de l'eau d'un puits, et les isotopes, silencieusement, se faufilent à l'intérieur. Les doses augmentent, petit à petit. Inaperçues, mais dangereuses.

---

> **"Si les isotopes pouvaient parler, ils vous raconteraient leurs histoires. Mais puisqu'ils restent muets, notre programme vous les racontera à leur place."**