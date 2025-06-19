Postes: 
curl -X 'GET' \
  'http://localhost:8083/api/referentiels/refpostes?page=1&size=10&sort=annee&direction=ASC' \
  -H 'accept: */*'
  Response Exemple : 
  "totalPages": 1073741824,
  "totalElements": 9007199254740991,
  "size": 1073741824,
  "content": [
    {
      "annee": 1073741824,
      "modeleEf": "string",
      "codePoste": "string",
      "format": "string",
      "niveau_1": "string",
      "niveau_2": "string",
      "niveau_3": "string",
      "libelle": "string",
      "complement": "string",
      "restrict": "string",
      "equiv_1": "string",
      "equiv_2": "string",
      "criticite": 1073741824
    }
  ],
  "number": 1073741824,
  "sort": {
    "empty": true,
    "sorted": true,
    "unsorted": true
  },
  "pageable": {
    "offset": 9007199254740991,
    "sort": {
      "empty": true,
      "sorted": true,
      "unsorted": true
    },
    "pageSize": 1073741824,
    "pageNumber": 1073741824,
    "paged": true,
    "unpaged": true
  },
  "numberOfElements": 1073741824,
  "first": true,
  "last": true,
  "empty": true
}
Indicateurs:
curl -X 'GET' \
  'http://localhost:8083/api/referentiels/refindicateurs?page=1&size=10&sort=annee&direction=ASC' \
  -H 'accept: */*'
  Response Exemple : 
{
  "totalPages": 1073741824,
  "totalElements": 9007199254740991,
  "size": 1073741824,
  "content": [
    {
      "codeIndicateur": "string",
      "annee": 1073741824,
      "declinaisonModeleEF": "string",
      "libelle": "string",
      "poche": "string",
      "rang": 1073741824,
      "versionNumero": "string",
      "versionCommentaire": "string",
      "versionDate": "2025-06-19T12:20:44.009Z",
      "definitionSuccinte": "string",
      "commentaire": "string",
      "calculTheorique": "string",
      "declinaisonCalculEffectif": "string"
    }
  ],
  "number": 1073741824,
  "sort": {
    "empty": true,
    "sorted": true,
    "unsorted": true
  },
  "pageable": {
    "offset": 9007199254740991,
    "sort": {
      "empty": true,
      "sorted": true,
      "unsorted": true
    },
    "pageSize": 1073741824,
    "pageNumber": 1073741824,
    "paged": true,
    "unpaged": true
  },
  "numberOfElements": 1073741824,
  "first": true,
  "last": true,
  "empty": true
}

