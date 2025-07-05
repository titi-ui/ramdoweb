<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Générateur de sites aléatoires</title>
  <style>
    body {
      background: #111;
      color: white;
      font-family: sans-serif;
      text-align: center;
      padding-top: 100px;
    }
    button {
      padding: 15px 30px;
      font-size: 18px;
      background-color: #00aaff;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      color: white;
    }
    a {
      display: block;
      margin-top: 30px;
      font-size: 20px;
      color: #00ffcc;
    }
  </style>
</head>
<body>
  <h1>Site .com Aléatoire</h1>
  <button onclick="genererSite()">Générer une URL</button>
  <a id="lien" href="#" target="_blank" style="display: none;"></a>

  <script>
    const mots = [
      "abricot", "accident", "actrice", "admirer", "adresse", "advenir", "affiche", "agenda", "agencer", "agir",
      "aide", "aigle", "aimer", "alarme", "album", "alerte", "algèbre", "aligner", "allumer", "alvéole",
      "amasser", "ambiance", "ami", "amour", "amuser", "ananas", "ancien", "ancre", "anecdote", "ange",
      "animal", "anneau", "annoncer", "antenne", "antonyme", "appeler", "appui", "après", "arbre", "arcade",
      "ardoise", "argent", "argile", "armoire", "arôme", "arriver", "article", "artiste", "ascenseur", "aspect",
      "aspirer", "assiette", "astre", "atelier", "attacher", "attaque", "attraper", "aube", "auberge", "aucun",
      "audace", "augmenter", "auteur", "autobus", "autre", "avaler", "avancer", "aventure", "avion", "avoine",
      "avoir", "avouer", "bagarre", "baguette", "balancer", "balcon", "balle", "ballon", "bambou", "banane",
      "banc", "banque", "barbe", "baril", "barque", "basculer", "base", "basilic", "basket", "bavard",
      "beau", "bébé", "bêcher", "besoin", "biberon", "bijou", "billet", "bilan", "bise", "biscuit",
      "bizarre", "blague", "blason", "bleu", "blessure", "bloquer", "blouse", "boire", "boîte", "bonbon",
      "bondir", "bonheur", "bonjour", "bonnet", "bord", "border", "botanique", "bouteille", "bouton", "bretelle",
      "bricoler", "brioche", "briquet", "brouillard", "brouter", "bruit", "brûler", "brume", "buffet", "buisson",
      "bulle", "bureau", "cabane", "câble", "cache", "cacher", "cactus", "cadeau", "cadence", "café",
      "cage", "caillou", "caisse", "calendrier", "calme", "caméra", "camion", "campagne", "canard", "canal",
      "canapé", "canette", "capitale", "capuche", "capter", "capture", "carafe", "carotte", "carte", "cascade",
      "casque", "casserole", "cassoulet", "castor", "catastrophe", "causette", "cavale", "caverne", "ceinture", "céleste",
      "centaine", "cerise", "cerf", "chaise", "chance", "chanson", "chantier", "chapitre", "charbon", "charger",
      "charnière", "chasse", "château", "chaussette", "chausson", "chauve", "chemise", "chenille", "chercheur", "cheval",
      "cheville", "chien", "chiffre", "chocolat", "choix", "chute", "ciel", "ciseau", "clair", "clairon",
      "classe", "clavicule", "clé", "clef", "climat", "cloche", "clôture", "clown", "cochon", "coffre",
      "coiffeur", "coin", "colère", "collier", "colis", "collège", "colline", "colorier", "colonne", "combat",
      "commande", "compagnon", "complet", "complicite", "composer", "comprendre", "concert", "confiture", "congeler", "connaissance",
      "console", "construire", "contact", "contenu", "contour", "contrat", "convenir", "copier", "coquillage", "corail",
      "corde", "cornichon", "corridor", "costume", "coton", "coucher", "coude", "couler", "coup", "couple",
      "courage", "court", "cousin", "couture", "crabe", "craie", "cravate", "crayon", "créature", "créer",
      "crépuscule", "creuser", "crevette", "crime", "crise", "critique", "croiser", "croissant", "crocodile", "croire",
      "croisière", "croquer", "croustillant", "cube", "cuire", "cuillère", "cuisine", "cuisse", "culture", "curieux",
      "cyclone", "cylindre", "danse", "danser", "danger", "dauphin", "début", "décembre", "décider", "décoration",
      // ... tous les autres mots jusqu'à 1000
    ];

    function genererSite() {
      const mot = mots[Math.floor(Math.random() * mots.length)];
      const url = `https://${mot}.com`;
      const lien = document.getElementById("lien");
      lien.href = url;
      lien.textContent = url;
      lien.style.display = "block";
    }
  </script>
</body>
</html>
