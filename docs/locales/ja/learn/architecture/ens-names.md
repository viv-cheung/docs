# Noms ENS

Farcaster utilise les noms ENS comme identifiants lisibles par les humains pour les comptes. Deux types de noms ENS sont pris en charge :

- **Noms ENS offchain** : Gérés gratuitement par Farcaster. (ex : @alice) - **Noms ENS onchain** : Payants et gérés par un portefeuille. (ex : @alice.eth)

Les noms ENS ne peuvent être utilisés sur Farcaster que s'ils contiennent uniquement des lettres minuscules, des chiffres et des tirets, et s'ils font 16 caractères ou moins.

![Noms d'utilisateur](/assets/usernames.png)

## Noms ENS onchain

Les utilisateurs peuvent utiliser des noms ENS onchain comme `@alice.eth` sur Farcaster.

Les noms ENS onchain sont émis par ENS, se terminent par .eth et doivent être enregistrés sur la blockchain Ethereum L1. Tout le monde peut enregistrer un nom ENS en utilisant l'[application ENS](https://app.ens.domains/).

L'enregistrement des noms ENS onchain est payant, mais une fois enregistrés, ils sont gérés par l'utilisateur et ne peuvent pas être révoqués.

## Noms ENS offchain (Fnames)

Les utilisateurs peuvent utiliser des noms ENS offchain comme `@alice` sur Farcaster.

Les noms ENS offchain, également appelés noms Farcaster ou fnames, sont conformes à ENS mais sont enregistrés offchain. Les fnames sont gratuits mais doivent respecter une politique d'utilisation pour éviter le squatting et l'usurpation d'identité. Ils doivent également respecter les exigences suivantes :

1. Un compte ne peut posséder qu'un seul fname à la fois. 2. Un compte peut changer de fname tous les 28 jours.

### Politique d'utilisation

L'enregistrement des fnames est gratuit mais doit respecter les politiques suivantes :

1. Les noms associés à des personnalités publiques ou à des organisations peuvent être récupérés (ex : @google). 2. Les noms non utilisés pendant plus de 60 jours peuvent être récupérés. 3. Les noms enregistrés dans le but de les revendre peuvent être récupérés.

Les décisions sont prises par l'équipe Farcaster et nécessitent souvent un jugement humain. Les utilisateurs souhaitant un nom entièrement sous leur contrôle devraient utiliser des noms ENS onchain.

### Registre

Les fnames sont émis comme des noms offchain sous le sous-domaine `fcast.id`.

Bob peut enregistrer le nom ENS offchain `bob.fcast.id` et l'utiliser sur n'importe quelle application Farcaster avec le raccourci `@bob`. Le nom peut être enregistré en faisant une demande signée au serveur de registre Fname. Voir la référence API FName pour plus de détails sur la façon de consulter et de créer des fnames.

Pour en savoir plus sur le fonctionnement des fnames, voir [ENSIP-16](https://docs.ens.domains/ens-improvement-proposals/ensip-16-offchain-metadata) et [ERC-3668](https://eips.ethereum.org/EIPS/eip-3668).