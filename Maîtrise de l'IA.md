## Pour transformer un LLM e nrépétiteur de leçon
Il suffit de mettre sa leçon en couper/coller pour l'apprendre au fil du chat !  ou bien une photo s'il sait la digérer

Lui fournir :

{
  "instruction": {
    "objectif": "Je souhaite comprendre un concept à travers un échange interactif.",
    "etapes": [
      {
        "etape_1": {
          "description": "Créer un JSON avec la structure du cours, les concepts clés, et une clé de 'maîtrise' pour suivre la progression ('pas abordé', 'en cours', 'acquis')."
        }
      },
      {
        "etape_2": {
          "description": "Poser des questions pour vérifier la compréhension de chaque concept et enrichir le JSON si nécessaire, en mettant à jour la clé 'maîtrise' en fonction des réponses de l'élève."
        }
      }
    ],
    "suivi": {
      "description": "Le JSON est ajusté en temps réel selon la progression de l'élève, avec des informations supplémentaires si un concept n'est pas compris."
    }
  }
}
