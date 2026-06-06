# Bilan — niveau débutant (MFA)

Récapitulatif du **niveau débutant** de la progression *Bonjour Forge MFA*. Ce
niveau couvre les **mécaniques TOTP**, sans base ni session.

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Bonjour Forge MFA](/docs/forge/starters/welcome-mfa/debutant/mfa-welcome/) | Inspecter facteurs, statuts et présence de la clé de chiffrement. |
| 2 — [Secret TOTP et QR](/docs/forge/starters/welcome-mfa/debutant/mfa-secret/) | Générer un secret et son URI `otpauth://` (`generate_totp_secret`). |
| 3 — [Vérifier un code TOTP](/docs/forge/starters/welcome-mfa/debutant/mfa-verify/) | Confronter un code à 6 chiffres au secret (`verify_totp_code`). |

Vous comprenez la base du TOTP : secret partagé, code dérivé du temps, vérification.

## Et ensuite

Place au niveau **intermédiaire** : l'enrôlement d'un vrai facteur, le challenge de
connexion et les codes de récupération.

[Niveau intermédiaire : Enrôler un facteur TOTP](/docs/forge/starters/welcome-mfa/intermediaire/mfa-enroll/)
