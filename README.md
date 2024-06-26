# projet_IA_Detection_Fake_news
Detection of fakes news in football players transfert

## Description

Cette application Flask permet de prédire la véracité des transferts de joueurs de football en utilisant un modèle de machine learning entraîné sur un ensemble de données de transferts. L'utilisateur peut saisir les détails d'un transfert et obtenir un pourcentage de vérité ainsi que les champs probablement faux.

## Fonctionnalités

- Prédiction de la véracité des transferts de joueurs de football.
- Identification des champs potentiellement incorrects dans les détails du transfert fournis par l'utilisateur.

## Prérequis

Avant de commencer, assurez-vous d'avoir installé les éléments suivants :

- Python 3.x
- pip (gestionnaire de paquets Python)

## Installation

1. Clonez ce dépôt :
    ```sh
    git clone https://github.com/WiloSensei07/projet_IA_Detection_Fake_news.git
    cd votre-repository
    ```

2. Créez et activez un environnement virtuel :
    ```sh
    python3 -m venv .venv
    source .venv/bin/activate  # Sur Windows, utilisez `.venv\Scripts\activate`
    ```

3. Installez les dépendances requises :
    ```sh
    pip install -r requirements.txt
    ```

4. Assurez-vous d'avoir le modèle et les encoders sauvegardés :
    ```sh
    # Le modèle et les encoders devraient être sauvegardés dans le répertoire 'model'
    joblib.dump(model, 'model/best_model.pkl')
    joblib.dump(label_encoders, 'model/label_encoders.pkl')
    ```

## Utilisation

1. Exécutez l'application Flask :
    ```sh
    python app.py
    ```

2. Ouvrez votre navigateur et accédez à `http://127.0.0.1:5000/`.

3. Remplissez le formulaire avec les détails du transfert du joueur et soumettez-le pour obtenir le pourcentage de vérité et les champs potentiellement faux.

## Structure des Dossiers

- `app.py` : Le fichier principal de l'application Flask.
- `model/` : Contient le modèle entraîné (`best_model.pkl`) et les encoders (`label_encoders.pkl`).
- `templates/` : Contient le template HTML (`index.html`).

## Contribution

Les contributions sont les bienvenues ! Veuillez soumettre une pull request pour toute amélioration ou correction.

## License

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## Acknowledgements

- Scikit-learn pour les outils de machine learning.
- Flask pour le framework web léger.
- Imbalanced-learn pour la gestion du déséquilibre des classes.

