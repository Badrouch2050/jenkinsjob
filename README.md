curl -X 'GET' \
  'http://localhost:8083/api/etatFinancier?page=0&size=10&sort=millesime&direction=ASC' \
  -H 'accept: */*'
  
  {
  "content": [
    {
      "siret": "24791789827674",
      "siren": "247917898",
      "entite": "cnBQs",
      "codeBanque": "08450",
      "codeETB": "6Ky",
      "idClientFederal": "LDZsXflHN8",
      "modeleEF": "2050",
      "codeDevise": "EUR",
      "idClientLocal": "MOr06fQ5q22eJeyGK4WL",
      "dateCRE": "2025-03-19",
      "dureeEX": 10,
      "dateCLO": "2025-03-18",
      "typeEF": "C",
      "anneeEF": 2025,
      "millesime": 2026,
      "periodiciteEF": "A",
      "topConfidentiel": 0,
      "topPublie": 1,
      "unite": "3",
      "statutEF": "v",
      "traitement": "M",
      "raisonSOC": "TKWaogGYmMRGuLC",
      "adresseCLT": "egRwSGZZYgIyEGv",
      "dateFile": "2025-03-18T10:10:54Z",
      "version": 1,
      "id": 266
    }
  ],
  "pageable": {
    "pageNumber": 0,
    "pageSize": 10,
    "sort": {
      "empty": false,
      "sorted": true,
      "unsorted": false
    },
    "offset": 0,
    "paged": true,
    "unpaged": false
  },
  "last": true,
  "totalElements": 1,
  "totalPages": 1,
  "first": true,
  "size": 10,
  "number": 0,
  "sort": {
    "empty": false,
    "sorted": true,
    "unsorted": false
  },
  "numberOfElements": 1,
  "empty": false
}

// Get postes of EtatFinacier 

curl -X 'GET' \
  'http://localhost:8083/api/bilan/etatFinancier/266/poste?page=0&size=10&sort=codePoste&direction=ASC' \
  -H 'accept: */*'

{
  "content": [
    {
      "codePoste": "AA",
      "valeur": 485620,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AB",
      "valeur": 946200,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AC",
      "valeur": 799170,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AF",
      "valeur": 750210,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AG",
      "valeur": 472430,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AH",
      "valeur": 401230,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AI",
      "valeur": 543570,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AJ",
      "valeur": 738300,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AK",
      "valeur": 200890,
      "topRetraitement": 0,
      "commentaire": null
    },
    {
      "codePoste": "AL",
      "valeur": 100990,
      "topRetraitement": 0,
      "commentaire": null
    }
  ],
  "pageable": {
    "pageNumber": 0,
    "pageSize": 10,
    "sort": {
      "empty": false,
      "sorted": true,
      "unsorted": false
    },
    "offset": 0,
    "paged": true,
    "unpaged": false
  },
  "last": false,
  "totalElements": 141,
  "totalPages": 15,
  "first": true,
  "size": 10,
  "number": 0,
  "sort": {
    "empty": false,
    "sorted": true,
    "unsorted": false
  },
  "numberOfElements": 10,
  "empty": false
}


// get idClientLocal par id Financier 

curl -X 'GET' \
  'http://localhost:8083/api/bilan/etatFinancier/266/indicateurlocal?page=0&size=10&sort=CODE_INDICATEUR&direction=ASC' \
  -H 'accept: */*'

{
  "totalElements": 9007199254740991,
  "totalPages": 1073741824,
  "first": true,
  "last": true,
  "size": 1073741824,
  "content": [
    {
      "codeIndicateur": "string",
      "valeur": 0,
      "topRetraitement": 1073741824,
      "commentaire": "string"
    }
  ],
  "number": 1073741824,
  "sort": {
    "empty": true,
    "sorted": true,
    "unsorted": true
  },
  "numberOfElements": 1073741824,
  "pageable": {
    "offset": 9007199254740991,
    "sort": {
      "empty": true,
      "sorted": true,
      "unsorted": true
    },
    "unpaged": true,
    "pageSize": 1073741824,
    "pageNumber": 1073741824,
    "paged": true
  },
  "empty": true
}

// get indicateur centrale par id EtatFiancier 
curl -X 'GET' \
  'http://localhost:8083/api/bilan/etatFinancier/266/indicateurCentral?page=0&size=10&sort=CODE_INDICATEUR&direction=ASC' \
  -H 'accept: */*'

  {
  "content": [
    {
      "codeIndicateur": "ACT_CORP_NET",
      "valeur": -6894455.5,
      "commentaire": null
    },
    {
      "codeIndicateur": "BADWILL",
      "valeur": null,
      "commentaire": null
    },
    {
      "codeIndicateur": "BFR_BRT",
      "valeur": 1954550,
      "commentaire": null
    },
    {
      "codeIndicateur": "BFR_NET",
      "valeur": -2052100,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAF",
      "valeur": 2138370,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAPA_REMBO_CT",
      "valeur": 1.302969,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAPA_REMBO_DFN",
      "valeur": 1.536565,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAPA_REMBO_MLT",
      "valeur": 0.477226,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAPEX_NET",
      "valeur": 11613340,
      "commentaire": null
    },
    {
      "codeIndicateur": "CAP_PER",
      "valeur": 2479515.5,
      "commentaire": null
    }
  ],
  "pageable": {
    "pageNumber": 0,
    "pageSize": 10,
    "sort": {
      "empty": false,
      "sorted": true,
      "unsorted": false
    },
    "offset": 0,
    "paged": true,
    "unpaged": false
  },
  "last": false,
  "totalElements": 120,
  "totalPages": 12,
  "first": true,
  "size": 10,
  "number": 0,
  "sort": {
    "empty": false,
    "sorted": true,
    "unsorted": false
  },
  "numberOfElements": 10,
  "empty": false
}
curl -X 'GET' \
  'http://localhost:8083/api/etatFinancier/266' \
  -H 'accept: */*'
{
  "siret": "24791789827674",
  "siren": "247917898",
  "entite": "cnBQs",
  "codeBanque": "08450",
  "codeETB": "6Ky",
  "idClientFederal": "LDZsXflHN8",
  "modeleEF": "2050",
  "codeDevise": "EUR",
  "idClientLocal": "MOr06fQ5q22eJeyGK4WL",
  "dateCRE": "2025-03-19",
  "dureeEX": 10,
  "dateCLO": "2025-03-18",
  "typeEF": "C",
  "anneeEF": 2025,
  "millesime": 2026,
  "periodiciteEF": "A",
  "topConfidentiel": 0,
  "topPublie": 1,
  "unite": "3",
  "statutEF": "v",
  "traitement": "M",
  "raisonSOC": "TKWaogGYmMRGuLC",
  "adresseCLT": "egRwSGZZYgIyEGv",
  "dateFile": "2025-03-18T10:10:54Z",
  "version": 1,
  "id": 266
}
