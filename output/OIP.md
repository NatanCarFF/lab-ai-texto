## Usando cloud Vision API
![Screenshot_2](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/05f5f440-4932-493a-bb59-91b11de550b7)

## Acessando a página de testes da API
![Screenshot_6](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/61775316-dc97-4727-bdc0-d768ac42d354)

## Inserindo a terceira imagem para teste:
![Screenshot_9](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/11783d2c-0ce9-42ea-b315-0163a7c1607e)

## Arquivo JSON - Request
{
  "requests": [
    {
      "features": [
        {
          "maxResults": 50,
          "type": "LANDMARK_DETECTION"
        },
        {
          "maxResults": 50,
          "type": "FACE_DETECTION"
        },
        {
          "maxResults": 50,
          "model": "builtin/latest",
          "type": "OBJECT_LOCALIZATION"
        },
        {
          "maxResults": 50,
          "model": "builtin/latest",
          "type": "LOGO_DETECTION"
        },
        {
          "maxResults": 50,
          "type": "LABEL_DETECTION"
        },
        {
          "maxResults": 50,
          "model": "builtin/latest",
          "type": "DOCUMENT_TEXT_DETECTION"
        },
        {
          "maxResults": 50,
          "type": "SAFE_SEARCH_DETECTION"
        },
        {
          "maxResults": 50,
          "type": "IMAGE_PROPERTIES"
        },
        {
          "maxResults": 50,
          "type": "CROP_HINTS"
        }
      ],
      "image": {
        "content": "(data from OIP.jpg)"
      },
      "imageContext": {
        "cropHintsParams": {
          "aspectRatios": [
            0.8,
            1,
            1.2
          ]
        }
      }
    }
  ]
}

## Arquivo JSON - Response
{
  "cropHintsAnnotation": {
    "cropHints": [
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 23
            },
            {
              "x": 402
            },
            {
              "x": 402,
              "y": 472
            },
            {
              "x": 23,
              "y": 472
            }
          ]
        },
        "confidence": 0.52845865,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {},
            {
              "x": 473
            },
            {
              "x": 473,
              "y": 472
            },
            {
              "y": 472
            }
          ]
        },
        "confidence": 0.42276692,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "y": 39
            },
            {
              "x": 473,
              "y": 39
            },
            {
              "x": 473,
              "y": 433
            },
            {
              "y": 433
            }
          ]
        },
        "confidence": 0.505182,
        "importanceFraction": 1
      }
    ]
  },
  "fullTextAnnotation": {
    "pages": [
      {
        "blocks": [
          {
            "blockType": "TEXT",
            "boundingBox": {
              "vertices": [
                {
                  "x": 291,
                  "y": 70
                },
                {
                  "x": 372,
                  "y": 71
                },
                {
                  "x": 372,
                  "y": 85
                },
                {
                  "x": 291,
                  "y": 84
                }
              ]
            },
            "confidence": 0.8673531,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 291,
                      "y": 70
                    },
                    {
                      "x": 372,
                      "y": 71
                    },
                    {
                      "x": 372,
                      "y": 85
                    },
                    {
                      "x": 291,
                      "y": 84
                    }
                  ]
                },
                "confidence": 0.8673531,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 291,
                          "y": 70
                        },
                        {
                          "x": 319,
                          "y": 70
                        },
                        {
                          "x": 319,
                          "y": 84
                        },
                        {
                          "x": 291,
                          "y": 84
                        }
                      ]
                    },
                    "confidence": 0.89009017,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 291,
                              "y": 70
                            },
                            {
                              "x": 301,
                              "y": 70
                            },
                            {
                              "x": 301,
                              "y": 84
                            },
                            {
                              "x": 291,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.90447545,
                        "text": "M"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 300,
                              "y": 70
                            },
                            {
                              "x": 306,
                              "y": 70
                            },
                            {
                              "x": 306,
                              "y": 84
                            },
                            {
                              "x": 300,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.9110096,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 303,
                              "y": 70
                            },
                            {
                              "x": 309,
                              "y": 70
                            },
                            {
                              "x": 309,
                              "y": 84
                            },
                            {
                              "x": 303,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.93428874,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 308,
                              "y": 70
                            },
                            {
                              "x": 313,
                              "y": 70
                            },
                            {
                              "x": 313,
                              "y": 84
                            },
                            {
                              "x": 308,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.90293574,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 311,
                              "y": 70
                            },
                            {
                              "x": 317,
                              "y": 70
                            },
                            {
                              "x": 317,
                              "y": 84
                            },
                            {
                              "x": 311,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.84058464,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 315,
                              "y": 70
                            },
                            {
                              "x": 319,
                              "y": 70
                            },
                            {
                              "x": 319,
                              "y": 84
                            },
                            {
                              "x": 315,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.8472468,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "S"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 321,
                          "y": 70
                        },
                        {
                          "x": 372,
                          "y": 71
                        },
                        {
                          "x": 372,
                          "y": 85
                        },
                        {
                          "x": 321,
                          "y": 84
                        }
                      ]
                    },
                    "confidence": 0.8559845,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 321,
                              "y": 70
                            },
                            {
                              "x": 326,
                              "y": 70
                            },
                            {
                              "x": 326,
                              "y": 84
                            },
                            {
                              "x": 321,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.95880103,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 324,
                              "y": 70
                            },
                            {
                              "x": 331,
                              "y": 70
                            },
                            {
                              "x": 331,
                              "y": 84
                            },
                            {
                              "x": 324,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.9623832,
                        "text": "M"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 330,
                              "y": 70
                            },
                            {
                              "x": 335,
                              "y": 70
                            },
                            {
                              "x": 335,
                              "y": 84
                            },
                            {
                              "x": 330,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.97959036,
                        "text": "P"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 335,
                              "y": 70
                            },
                            {
                              "x": 340,
                              "y": 70
                            },
                            {
                              "x": 340,
                              "y": 84
                            },
                            {
                              "x": 335,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.96049386,
                        "text": "L"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 337,
                              "y": 70
                            },
                            {
                              "x": 343,
                              "y": 70
                            },
                            {
                              "x": 343,
                              "y": 84
                            },
                            {
                              "x": 337,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.9208291,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 342,
                              "y": 70
                            },
                            {
                              "x": 347,
                              "y": 70
                            },
                            {
                              "x": 347,
                              "y": 84
                            },
                            {
                              "x": 342,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.9073113,
                        "text": "C"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 346,
                              "y": 70
                            },
                            {
                              "x": 353,
                              "y": 70
                            },
                            {
                              "x": 353,
                              "y": 84
                            },
                            {
                              "x": 346,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.5839426,
                        "text": "Á"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 350,
                              "y": 70
                            },
                            {
                              "x": 357,
                              "y": 70
                            },
                            {
                              "x": 357,
                              "y": 84
                            },
                            {
                              "x": 350,
                              "y": 84
                            }
                          ]
                        },
                        "confidence": 0.83434296,
                        "text": "V"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 355,
                              "y": 71
                            },
                            {
                              "x": 360,
                              "y": 71
                            },
                            {
                              "x": 360,
                              "y": 85
                            },
                            {
                              "x": 355,
                              "y": 85
                            }
                          ]
                        },
                        "confidence": 0.8132446,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 360,
                              "y": 71
                            },
                            {
                              "x": 364,
                              "y": 71
                            },
                            {
                              "x": 364,
                              "y": 85
                            },
                            {
                              "x": 360,
                              "y": 85
                            }
                          ]
                        },
                        "confidence": 0.77997637,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 361,
                              "y": 71
                            },
                            {
                              "x": 366,
                              "y": 71
                            },
                            {
                              "x": 366,
                              "y": 85
                            },
                            {
                              "x": 361,
                              "y": 85
                            }
                          ]
                        },
                        "confidence": 0.9216194,
                        "text": "S"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 367,
                              "y": 71
                            },
                            {
                              "x": 372,
                              "y": 71
                            },
                            {
                              "x": 372,
                              "y": 85
                            },
                            {
                              "x": 367,
                              "y": 85
                            }
                          ]
                        },
                        "confidence": 0.64927953,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "-"
                      }
                    ]
                  }
                ]
              }
            ]
          },
          {
            "blockType": "TEXT",
            "boundingBox": {
              "vertices": [
                {
                  "x": 228,
                  "y": 107
                },
                {
                  "x": 414,
                  "y": 109
                },
                {
                  "x": 411,
                  "y": 412
                },
                {
                  "x": 225,
                  "y": 410
                }
              ]
            },
            "confidence": 0.9699256,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 233,
                      "y": 107
                    },
                    {
                      "x": 403,
                      "y": 110
                    },
                    {
                      "x": 403,
                      "y": 138
                    },
                    {
                      "x": 233,
                      "y": 135
                    }
                  ]
                },
                "confidence": 0.97116077,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 233,
                          "y": 108
                        },
                        {
                          "x": 262,
                          "y": 108
                        },
                        {
                          "x": 262,
                          "y": 135
                        },
                        {
                          "x": 233,
                          "y": 135
                        }
                      ]
                    },
                    "confidence": 0.899305,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 233,
                              "y": 108
                            },
                            {
                              "x": 248,
                              "y": 108
                            },
                            {
                              "x": 248,
                              "y": 135
                            },
                            {
                              "x": 233,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.93492615,
                        "text": "H"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 245,
                              "y": 108
                            },
                            {
                              "x": 262,
                              "y": 108
                            },
                            {
                              "x": 262,
                              "y": 135
                            },
                            {
                              "x": 245,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.8636838,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "Á"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 266,
                          "y": 108
                        },
                        {
                          "x": 350,
                          "y": 109
                        },
                        {
                          "x": 350,
                          "y": 136
                        },
                        {
                          "x": 266,
                          "y": 135
                        }
                      ]
                    },
                    "confidence": 0.98554295,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 266,
                              "y": 108
                            },
                            {
                              "x": 282,
                              "y": 108
                            },
                            {
                              "x": 282,
                              "y": 135
                            },
                            {
                              "x": 266,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9894288,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 282,
                              "y": 108
                            },
                            {
                              "x": 295,
                              "y": 108
                            },
                            {
                              "x": 295,
                              "y": 135
                            },
                            {
                              "x": 282,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9882245,
                        "text": "P"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 295,
                              "y": 108
                            },
                            {
                              "x": 307,
                              "y": 108
                            },
                            {
                              "x": 307,
                              "y": 135
                            },
                            {
                              "x": 295,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9743445,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 308,
                              "y": 109
                            },
                            {
                              "x": 322,
                              "y": 109
                            },
                            {
                              "x": 322,
                              "y": 136
                            },
                            {
                              "x": 308,
                              "y": 136
                            }
                          ]
                        },
                        "confidence": 0.9822977,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 322,
                              "y": 109
                            },
                            {
                              "x": 337,
                              "y": 109
                            },
                            {
                              "x": 337,
                              "y": 136
                            },
                            {
                              "x": 322,
                              "y": 136
                            }
                          ]
                        },
                        "confidence": 0.98512316,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 336,
                              "y": 109
                            },
                            {
                              "x": 350,
                              "y": 109
                            },
                            {
                              "x": 350,
                              "y": 136
                            },
                            {
                              "x": 336,
                              "y": 136
                            }
                          ]
                        },
                        "confidence": 0.99383914,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "S"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 355,
                          "y": 109
                        },
                        {
                          "x": 403,
                          "y": 110
                        },
                        {
                          "x": 403,
                          "y": 138
                        },
                        {
                          "x": 355,
                          "y": 137
                        }
                      ]
                    },
                    "confidence": 0.9903003,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 355,
                              "y": 109
                            },
                            {
                              "x": 368,
                              "y": 109
                            },
                            {
                              "x": 368,
                              "y": 136
                            },
                            {
                              "x": 355,
                              "y": 136
                            }
                          ]
                        },
                        "confidence": 0.99265933,
                        "text": "U"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 370,
                              "y": 110
                            },
                            {
                              "x": 387,
                              "y": 110
                            },
                            {
                              "x": 387,
                              "y": 137
                            },
                            {
                              "x": 370,
                              "y": 137
                            }
                          ]
                        },
                        "confidence": 0.99221015,
                        "text": "M"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 386,
                              "y": 110
                            },
                            {
                              "x": 403,
                              "y": 110
                            },
                            {
                              "x": 403,
                              "y": 137
                            },
                            {
                              "x": 386,
                              "y": 137
                            }
                          ]
                        },
                        "confidence": 0.9860315,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "A"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 254,
                      "y": 158
                    },
                    {
                      "x": 382,
                      "y": 159
                    },
                    {
                      "x": 382,
                      "y": 183
                    },
                    {
                      "x": 254,
                      "y": 182
                    }
                  ]
                },
                "confidence": 0.9920741,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 254,
                          "y": 158
                        },
                        {
                          "x": 348,
                          "y": 158
                        },
                        {
                          "x": 348,
                          "y": 182
                        },
                        {
                          "x": 254,
                          "y": 182
                        }
                      ]
                    },
                    "confidence": 0.9917256,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 254,
                              "y": 158
                            },
                            {
                              "x": 272,
                              "y": 158
                            },
                            {
                              "x": 272,
                              "y": 182
                            },
                            {
                              "x": 254,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.9860347,
                        "text": "M"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 270,
                              "y": 158
                            },
                            {
                              "x": 286,
                              "y": 158
                            },
                            {
                              "x": 286,
                              "y": 182
                            },
                            {
                              "x": 270,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.98960054,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 286,
                              "y": 158
                            },
                            {
                              "x": 300,
                              "y": 158
                            },
                            {
                              "x": 300,
                              "y": 182
                            },
                            {
                              "x": 286,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.9932327,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 301,
                              "y": 158
                            },
                            {
                              "x": 313,
                              "y": 158
                            },
                            {
                              "x": 313,
                              "y": 182
                            },
                            {
                              "x": 301,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.9948129,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 314,
                              "y": 158
                            },
                            {
                              "x": 319,
                              "y": 158
                            },
                            {
                              "x": 319,
                              "y": 182
                            },
                            {
                              "x": 314,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.992703,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 320,
                              "y": 158
                            },
                            {
                              "x": 334,
                              "y": 158
                            },
                            {
                              "x": 334,
                              "y": 182
                            },
                            {
                              "x": 320,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.99257666,
                        "text": "R"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 333,
                              "y": 158
                            },
                            {
                              "x": 348,
                              "y": 158
                            },
                            {
                              "x": 348,
                              "y": 182
                            },
                            {
                              "x": 333,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.993119,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 354,
                          "y": 158
                        },
                        {
                          "x": 382,
                          "y": 158
                        },
                        {
                          "x": 382,
                          "y": 182
                        },
                        {
                          "x": 354,
                          "y": 182
                        }
                      ]
                    },
                    "confidence": 0.99329364,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 354,
                              "y": 158
                            },
                            {
                              "x": 368,
                              "y": 158
                            },
                            {
                              "x": 368,
                              "y": 182
                            },
                            {
                              "x": 354,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.99372065,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 370,
                              "y": 158
                            },
                            {
                              "x": 382,
                              "y": 158
                            },
                            {
                              "x": 382,
                              "y": 182
                            },
                            {
                              "x": 370,
                              "y": 182
                            }
                          ]
                        },
                        "confidence": 0.9928667,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "E"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 227,
                      "y": 201
                    },
                    {
                      "x": 406,
                      "y": 198
                    },
                    {
                      "x": 407,
                      "y": 228
                    },
                    {
                      "x": 228,
                      "y": 231
                    }
                  ]
                },
                "confidence": 0.9717433,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 227,
                          "y": 201
                        },
                        {
                          "x": 300,
                          "y": 200
                        },
                        {
                          "x": 301,
                          "y": 230
                        },
                        {
                          "x": 228,
                          "y": 231
                        }
                      ]
                    },
                    "confidence": 0.9898786,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 227,
                              "y": 202
                            },
                            {
                              "x": 240,
                              "y": 202
                            },
                            {
                              "x": 241,
                              "y": 231
                            },
                            {
                              "x": 228,
                              "y": 231
                            }
                          ]
                        },
                        "confidence": 0.9913828,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 239,
                              "y": 201
                            },
                            {
                              "x": 254,
                              "y": 201
                            },
                            {
                              "x": 255,
                              "y": 230
                            },
                            {
                              "x": 240,
                              "y": 230
                            }
                          ]
                        },
                        "confidence": 0.9951271,
                        "text": "V"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 253,
                              "y": 201
                            },
                            {
                              "x": 260,
                              "y": 201
                            },
                            {
                              "x": 261,
                              "y": 230
                            },
                            {
                              "x": 254,
                              "y": 230
                            }
                          ]
                        },
                        "confidence": 0.99488014,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 260,
                              "y": 201
                            },
                            {
                              "x": 273,
                              "y": 201
                            },
                            {
                              "x": 274,
                              "y": 230
                            },
                            {
                              "x": 261,
                              "y": 230
                            }
                          ]
                        },
                        "confidence": 0.992542,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 271,
                              "y": 201
                            },
                            {
                              "x": 286,
                              "y": 201
                            },
                            {
                              "x": 287,
                              "y": 230
                            },
                            {
                              "x": 272,
                              "y": 230
                            }
                          ]
                        },
                        "confidence": 0.98492074,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 287,
                              "y": 200
                            },
                            {
                              "x": 300,
                              "y": 200
                            },
                            {
                              "x": 301,
                              "y": 229
                            },
                            {
                              "x": 288,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.98041874,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "R"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 304,
                          "y": 200
                        },
                        {
                          "x": 399,
                          "y": 198
                        },
                        {
                          "x": 400,
                          "y": 227
                        },
                        {
                          "x": 305,
                          "y": 229
                        }
                      ]
                    },
                    "confidence": 0.9590441,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 304,
                              "y": 200
                            },
                            {
                              "x": 318,
                              "y": 200
                            },
                            {
                              "x": 319,
                              "y": 229
                            },
                            {
                              "x": 305,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9839496,
                        "text": "C"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 319,
                              "y": 200
                            },
                            {
                              "x": 332,
                              "y": 200
                            },
                            {
                              "x": 333,
                              "y": 229
                            },
                            {
                              "x": 320,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.93823934,
                        "text": "R"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 331,
                              "y": 200
                            },
                            {
                              "x": 343,
                              "y": 200
                            },
                            {
                              "x": 344,
                              "y": 229
                            },
                            {
                              "x": 332,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.8341293,
                        "text": "Í"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 339,
                              "y": 199
                            },
                            {
                              "x": 352,
                              "y": 199
                            },
                            {
                              "x": 353,
                              "y": 228
                            },
                            {
                              "x": 340,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.9599645,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 351,
                              "y": 199
                            },
                            {
                              "x": 357,
                              "y": 199
                            },
                            {
                              "x": 358,
                              "y": 228
                            },
                            {
                              "x": 352,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.9897601,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 358,
                              "y": 199
                            },
                            {
                              "x": 371,
                              "y": 199
                            },
                            {
                              "x": 372,
                              "y": 228
                            },
                            {
                              "x": 359,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.9909112,
                        "text": "C"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 371,
                              "y": 199
                            },
                            {
                              "x": 386,
                              "y": 199
                            },
                            {
                              "x": 387,
                              "y": 228
                            },
                            {
                              "x": 372,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.99241376,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 385,
                              "y": 199
                            },
                            {
                              "x": 399,
                              "y": 199
                            },
                            {
                              "x": 400,
                              "y": 228
                            },
                            {
                              "x": 386,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.98298526,
                        "text": "S"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 399,
                          "y": 198
                        },
                        {
                          "x": 406,
                          "y": 198
                        },
                        {
                          "x": 407,
                          "y": 227
                        },
                        {
                          "x": 400,
                          "y": 227
                        }
                      ]
                    },
                    "confidence": 0.9645244,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 399,
                              "y": 198
                            },
                            {
                              "x": 406,
                              "y": 198
                            },
                            {
                              "x": 407,
                              "y": 227
                            },
                            {
                              "x": 400,
                              "y": 227
                            }
                          ]
                        },
                        "confidence": 0.9645244,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": ":"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 233,
                      "y": 246
                    },
                    {
                      "x": 404,
                      "y": 250
                    },
                    {
                      "x": 403,
                      "y": 281
                    },
                    {
                      "x": 232,
                      "y": 277
                    }
                  ]
                },
                "confidence": 0.9432837,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 233,
                          "y": 246
                        },
                        {
                          "x": 276,
                          "y": 247
                        },
                        {
                          "x": 275,
                          "y": 278
                        },
                        {
                          "x": 232,
                          "y": 277
                        }
                      ]
                    },
                    "confidence": 0.89895093,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 233,
                              "y": 247
                            },
                            {
                              "x": 247,
                              "y": 247
                            },
                            {
                              "x": 246,
                              "y": 277
                            },
                            {
                              "x": 232,
                              "y": 277
                            }
                          ]
                        },
                        "confidence": 0.9331171,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 246,
                              "y": 247
                            },
                            {
                              "x": 263,
                              "y": 247
                            },
                            {
                              "x": 262,
                              "y": 277
                            },
                            {
                              "x": 245,
                              "y": 277
                            }
                          ]
                        },
                        "confidence": 0.79881275,
                        "text": "Ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 261,
                              "y": 247
                            },
                            {
                              "x": 276,
                              "y": 247
                            },
                            {
                              "x": 275,
                              "y": 277
                            },
                            {
                              "x": 260,
                              "y": 277
                            }
                          ]
                        },
                        "confidence": 0.96492296,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "O"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 280,
                          "y": 247
                        },
                        {
                          "x": 336,
                          "y": 248
                        },
                        {
                          "x": 335,
                          "y": 279
                        },
                        {
                          "x": 279,
                          "y": 278
                        }
                      ]
                    },
                    "confidence": 0.93584204,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 280,
                              "y": 248
                            },
                            {
                              "x": 293,
                              "y": 248
                            },
                            {
                              "x": 292,
                              "y": 278
                            },
                            {
                              "x": 279,
                              "y": 278
                            }
                          ]
                        },
                        "confidence": 0.96111745,
                        "text": "F"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 291,
                              "y": 248
                            },
                            {
                              "x": 307,
                              "y": 248
                            },
                            {
                              "x": 306,
                              "y": 278
                            },
                            {
                              "x": 290,
                              "y": 278
                            }
                          ]
                        },
                        "confidence": 0.9239617,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 306,
                              "y": 248
                            },
                            {
                              "x": 321,
                              "y": 248
                            },
                            {
                              "x": 320,
                              "y": 278
                            },
                            {
                              "x": 305,
                              "y": 278
                            }
                          ]
                        },
                        "confidence": 0.87696636,
                        "text": "Ç"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 319,
                              "y": 249
                            },
                            {
                              "x": 336,
                              "y": 249
                            },
                            {
                              "x": 335,
                              "y": 279
                            },
                            {
                              "x": 318,
                              "y": 279
                            }
                          ]
                        },
                        "confidence": 0.9813225,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 340,
                          "y": 249
                        },
                        {
                          "x": 398,
                          "y": 250
                        },
                        {
                          "x": 397,
                          "y": 280
                        },
                        {
                          "x": 339,
                          "y": 279
                        }
                      ]
                    },
                    "confidence": 0.98602355,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 340,
                              "y": 249
                            },
                            {
                              "x": 355,
                              "y": 249
                            },
                            {
                              "x": 354,
                              "y": 279
                            },
                            {
                              "x": 339,
                              "y": 279
                            }
                          ]
                        },
                        "confidence": 0.9924266,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 354,
                              "y": 249
                            },
                            {
                              "x": 371,
                              "y": 249
                            },
                            {
                              "x": 370,
                              "y": 279
                            },
                            {
                              "x": 353,
                              "y": 279
                            }
                          ]
                        },
                        "confidence": 0.9896896,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 368,
                              "y": 250
                            },
                            {
                              "x": 383,
                              "y": 250
                            },
                            {
                              "x": 382,
                              "y": 280
                            },
                            {
                              "x": 367,
                              "y": 280
                            }
                          ]
                        },
                        "confidence": 0.98671424,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 382,
                              "y": 250
                            },
                            {
                              "x": 398,
                              "y": 250
                            },
                            {
                              "x": 397,
                              "y": 280
                            },
                            {
                              "x": 381,
                              "y": 280
                            }
                          ]
                        },
                        "confidence": 0.9752639,
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 397,
                          "y": 250
                        },
                        {
                          "x": 404,
                          "y": 250
                        },
                        {
                          "x": 403,
                          "y": 280
                        },
                        {
                          "x": 396,
                          "y": 280
                        }
                      ]
                    },
                    "confidence": 0.9350887,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 397,
                              "y": 250
                            },
                            {
                              "x": 404,
                              "y": 250
                            },
                            {
                              "x": 403,
                              "y": 280
                            },
                            {
                              "x": 396,
                              "y": 280
                            }
                          ]
                        },
                        "confidence": 0.9350887,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": ","
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 234,
                      "y": 292
                    },
                    {
                      "x": 402,
                      "y": 296
                    },
                    {
                      "x": 401,
                      "y": 325
                    },
                    {
                      "x": 233,
                      "y": 321
                    }
                  ]
                },
                "confidence": 0.964074,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 234,
                          "y": 292
                        },
                        {
                          "x": 278,
                          "y": 293
                        },
                        {
                          "x": 277,
                          "y": 322
                        },
                        {
                          "x": 233,
                          "y": 321
                        }
                      ]
                    },
                    "confidence": 0.9125287,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 234,
                              "y": 293
                            },
                            {
                              "x": 249,
                              "y": 293
                            },
                            {
                              "x": 248,
                              "y": 321
                            },
                            {
                              "x": 233,
                              "y": 321
                            }
                          ]
                        },
                        "confidence": 0.96676934,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 249,
                              "y": 293
                            },
                            {
                              "x": 265,
                              "y": 293
                            },
                            {
                              "x": 264,
                              "y": 321
                            },
                            {
                              "x": 248,
                              "y": 321
                            }
                          ]
                        },
                        "confidence": 0.7893424,
                        "text": "Ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 264,
                              "y": 293
                            },
                            {
                              "x": 278,
                              "y": 293
                            },
                            {
                              "x": 277,
                              "y": 321
                            },
                            {
                              "x": 263,
                              "y": 321
                            }
                          ]
                        },
                        "confidence": 0.9814744,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "O"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 283,
                          "y": 293
                        },
                        {
                          "x": 333,
                          "y": 294
                        },
                        {
                          "x": 332,
                          "y": 323
                        },
                        {
                          "x": 282,
                          "y": 322
                        }
                      ]
                    },
                    "confidence": 0.989326,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 283,
                              "y": 294
                            },
                            {
                              "x": 297,
                              "y": 294
                            },
                            {
                              "x": 296,
                              "y": 322
                            },
                            {
                              "x": 282,
                              "y": 322
                            }
                          ]
                        },
                        "confidence": 0.990908,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 297,
                              "y": 294
                            },
                            {
                              "x": 304,
                              "y": 294
                            },
                            {
                              "x": 303,
                              "y": 322
                            },
                            {
                              "x": 296,
                              "y": 322
                            }
                          ]
                        },
                        "confidence": 0.9882379,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 304,
                              "y": 294
                            },
                            {
                              "x": 318,
                              "y": 294
                            },
                            {
                              "x": 317,
                              "y": 322
                            },
                            {
                              "x": 303,
                              "y": 322
                            }
                          ]
                        },
                        "confidence": 0.9911531,
                        "text": "G"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 317,
                              "y": 295
                            },
                            {
                              "x": 333,
                              "y": 295
                            },
                            {
                              "x": 332,
                              "y": 323
                            },
                            {
                              "x": 316,
                              "y": 323
                            }
                          ]
                        },
                        "confidence": 0.98700505,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 337,
                          "y": 295
                        },
                        {
                          "x": 396,
                          "y": 297
                        },
                        {
                          "x": 395,
                          "y": 326
                        },
                        {
                          "x": 336,
                          "y": 324
                        }
                      ]
                    },
                    "confidence": 0.9841706,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 337,
                              "y": 295
                            },
                            {
                              "x": 352,
                              "y": 295
                            },
                            {
                              "x": 351,
                              "y": 323
                            },
                            {
                              "x": 336,
                              "y": 323
                            }
                          ]
                        },
                        "confidence": 0.9845818,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 351,
                              "y": 296
                            },
                            {
                              "x": 367,
                              "y": 296
                            },
                            {
                              "x": 366,
                              "y": 324
                            },
                            {
                              "x": 350,
                              "y": 324
                            }
                          ]
                        },
                        "confidence": 0.992993,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 366,
                              "y": 296
                            },
                            {
                              "x": 380,
                              "y": 296
                            },
                            {
                              "x": 379,
                              "y": 324
                            },
                            {
                              "x": 365,
                              "y": 324
                            }
                          ]
                        },
                        "confidence": 0.97999984,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 379,
                              "y": 296
                            },
                            {
                              "x": 396,
                              "y": 296
                            },
                            {
                              "x": 395,
                              "y": 324
                            },
                            {
                              "x": 378,
                              "y": 324
                            }
                          ]
                        },
                        "confidence": 0.97910774,
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 395,
                          "y": 297
                        },
                        {
                          "x": 402,
                          "y": 297
                        },
                        {
                          "x": 401,
                          "y": 325
                        },
                        {
                          "x": 394,
                          "y": 325
                        }
                      ]
                    },
                    "confidence": 0.93731517,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 395,
                              "y": 297
                            },
                            {
                              "x": 402,
                              "y": 297
                            },
                            {
                              "x": 401,
                              "y": 325
                            },
                            {
                              "x": 394,
                              "y": 325
                            }
                          ]
                        },
                        "confidence": 0.93731517,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": ","
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 226,
                      "y": 339
                    },
                    {
                      "x": 412,
                      "y": 342
                    },
                    {
                      "x": 411,
                      "y": 371
                    },
                    {
                      "x": 225,
                      "y": 368
                    }
                  ]
                },
                "confidence": 0.97484416,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 226,
                          "y": 340
                        },
                        {
                          "x": 238,
                          "y": 340
                        },
                        {
                          "x": 237,
                          "y": 368
                        },
                        {
                          "x": 225,
                          "y": 368
                        }
                      ]
                    },
                    "confidence": 0.9808602,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 226,
                              "y": 340
                            },
                            {
                              "x": 238,
                              "y": 340
                            },
                            {
                              "x": 237,
                              "y": 368
                            },
                            {
                              "x": 225,
                              "y": 368
                            }
                          ]
                        },
                        "confidence": 0.9808602,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "E"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 244,
                          "y": 339
                        },
                        {
                          "x": 286,
                          "y": 340
                        },
                        {
                          "x": 285,
                          "y": 369
                        },
                        {
                          "x": 243,
                          "y": 368
                        }
                      ]
                    },
                    "confidence": 0.940208,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 244,
                              "y": 340
                            },
                            {
                              "x": 258,
                              "y": 340
                            },
                            {
                              "x": 257,
                              "y": 368
                            },
                            {
                              "x": 243,
                              "y": 368
                            }
                          ]
                        },
                        "confidence": 0.976212,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 256,
                              "y": 340
                            },
                            {
                              "x": 272,
                              "y": 340
                            },
                            {
                              "x": 271,
                              "y": 368
                            },
                            {
                              "x": 255,
                              "y": 368
                            }
                          ]
                        },
                        "confidence": 0.8570393,
                        "text": "Ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 273,
                              "y": 340
                            },
                            {
                              "x": 286,
                              "y": 340
                            },
                            {
                              "x": 285,
                              "y": 368
                            },
                            {
                              "x": 272,
                              "y": 368
                            }
                          ]
                        },
                        "confidence": 0.9873727,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "O"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 291,
                          "y": 340
                        },
                        {
                          "x": 341,
                          "y": 341
                        },
                        {
                          "x": 340,
                          "y": 370
                        },
                        {
                          "x": 290,
                          "y": 369
                        }
                      ]
                    },
                    "confidence": 0.98798656,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 291,
                              "y": 341
                            },
                            {
                              "x": 304,
                              "y": 341
                            },
                            {
                              "x": 303,
                              "y": 369
                            },
                            {
                              "x": 290,
                              "y": 369
                            }
                          ]
                        },
                        "confidence": 0.9887368,
                        "text": "S"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 306,
                              "y": 341
                            },
                            {
                              "x": 318,
                              "y": 341
                            },
                            {
                              "x": 317,
                              "y": 369
                            },
                            {
                              "x": 305,
                              "y": 369
                            }
                          ]
                        },
                        "confidence": 0.9874086,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 317,
                              "y": 341
                            },
                            {
                              "x": 327,
                              "y": 341
                            },
                            {
                              "x": 326,
                              "y": 369
                            },
                            {
                              "x": 316,
                              "y": 369
                            }
                          ]
                        },
                        "confidence": 0.9829715,
                        "text": "J"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 326,
                              "y": 341
                            },
                            {
                              "x": 341,
                              "y": 341
                            },
                            {
                              "x": 340,
                              "y": 369
                            },
                            {
                              "x": 325,
                              "y": 369
                            }
                          ]
                        },
                        "confidence": 0.99282944,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 347,
                          "y": 341
                        },
                        {
                          "x": 405,
                          "y": 342
                        },
                        {
                          "x": 404,
                          "y": 371
                        },
                        {
                          "x": 346,
                          "y": 370
                        }
                      ]
                    },
                    "confidence": 0.9895538,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 347,
                              "y": 342
                            },
                            {
                              "x": 361,
                              "y": 342
                            },
                            {
                              "x": 360,
                              "y": 370
                            },
                            {
                              "x": 346,
                              "y": 370
                            }
                          ]
                        },
                        "confidence": 0.9933763,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 360,
                              "y": 342
                            },
                            {
                              "x": 376,
                              "y": 342
                            },
                            {
                              "x": 375,
                              "y": 370
                            },
                            {
                              "x": 359,
                              "y": 370
                            }
                          ]
                        },
                        "confidence": 0.9939581,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 376,
                              "y": 342
                            },
                            {
                              "x": 390,
                              "y": 342
                            },
                            {
                              "x": 389,
                              "y": 370
                            },
                            {
                              "x": 375,
                              "y": 370
                            }
                          ]
                        },
                        "confidence": 0.9881648,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 389,
                              "y": 343
                            },
                            {
                              "x": 405,
                              "y": 343
                            },
                            {
                              "x": 404,
                              "y": 371
                            },
                            {
                              "x": 388,
                              "y": 371
                            }
                          ]
                        },
                        "confidence": 0.9827159,
                        "text": "A"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 405,
                          "y": 343
                        },
                        {
                          "x": 412,
                          "y": 343
                        },
                        {
                          "x": 411,
                          "y": 371
                        },
                        {
                          "x": 404,
                          "y": 371
                        }
                      ]
                    },
                    "confidence": 0.96132827,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 405,
                              "y": 343
                            },
                            {
                              "x": 412,
                              "y": 343
                            },
                            {
                              "x": 411,
                              "y": 371
                            },
                            {
                              "x": 404,
                              "y": 371
                            }
                          ]
                        },
                        "confidence": 0.96132827,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "."
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 252,
                      "y": 385
                    },
                    {
                      "x": 382,
                      "y": 384
                    },
                    {
                      "x": 382,
                      "y": 409
                    },
                    {
                      "x": 252,
                      "y": 410
                    }
                  ]
                },
                "confidence": 0.97707504,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 252,
                          "y": 386
                        },
                        {
                          "x": 262,
                          "y": 386
                        },
                        {
                          "x": 262,
                          "y": 410
                        },
                        {
                          "x": 252,
                          "y": 410
                        }
                      ]
                    },
                    "confidence": 0.87095356,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 252,
                              "y": 386
                            },
                            {
                              "x": 262,
                              "y": 386
                            },
                            {
                              "x": 262,
                              "y": 410
                            },
                            {
                              "x": 252,
                              "y": 410
                            }
                          ]
                        },
                        "confidence": 0.87095356,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "-"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 263,
                          "y": 385
                        },
                        {
                          "x": 382,
                          "y": 384
                        },
                        {
                          "x": 382,
                          "y": 408
                        },
                        {
                          "x": 263,
                          "y": 409
                        }
                      ]
                    },
                    "confidence": 0.98672247,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "pt"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 263,
                              "y": 385
                            },
                            {
                              "x": 276,
                              "y": 385
                            },
                            {
                              "x": 276,
                              "y": 409
                            },
                            {
                              "x": 263,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99224526,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 276,
                              "y": 385
                            },
                            {
                              "x": 287,
                              "y": 385
                            },
                            {
                              "x": 287,
                              "y": 409
                            },
                            {
                              "x": 276,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.9931239,
                        "text": "R"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 289,
                              "y": 385
                            },
                            {
                              "x": 293,
                              "y": 385
                            },
                            {
                              "x": 293,
                              "y": 409
                            },
                            {
                              "x": 289,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99443436,
                        "text": "I"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 294,
                              "y": 385
                            },
                            {
                              "x": 305,
                              "y": 385
                            },
                            {
                              "x": 305,
                              "y": 409
                            },
                            {
                              "x": 294,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99236584,
                        "text": "S"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 305,
                              "y": 385
                            },
                            {
                              "x": 315,
                              "y": 385
                            },
                            {
                              "x": 315,
                              "y": 409
                            },
                            {
                              "x": 305,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99173087,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 315,
                              "y": 385
                            },
                            {
                              "x": 329,
                              "y": 385
                            },
                            {
                              "x": 329,
                              "y": 409
                            },
                            {
                              "x": 315,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.9199252,
                        "text": "Ó"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 328,
                              "y": 385
                            },
                            {
                              "x": 339,
                              "y": 385
                            },
                            {
                              "x": 339,
                              "y": 409
                            },
                            {
                              "x": 328,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99346024,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 338,
                              "y": 385
                            },
                            {
                              "x": 349,
                              "y": 385
                            },
                            {
                              "x": 349,
                              "y": 409
                            },
                            {
                              "x": 338,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.9943811,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 350,
                              "y": 385
                            },
                            {
                              "x": 360,
                              "y": 385
                            },
                            {
                              "x": 360,
                              "y": 409
                            },
                            {
                              "x": 350,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99455994,
                        "text": "L"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 359,
                              "y": 385
                            },
                            {
                              "x": 369,
                              "y": 385
                            },
                            {
                              "x": 369,
                              "y": 409
                            },
                            {
                              "x": 359,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.99550605,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 370,
                              "y": 385
                            },
                            {
                              "x": 382,
                              "y": 385
                            },
                            {
                              "x": 382,
                              "y": 409
                            },
                            {
                              "x": 370,
                              "y": 409
                            }
                          ]
                        },
                        "confidence": 0.9922144,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "S"
                      }
                    ]
                  }
                ]
              }
            ]
          }
        ],
        "confidence": 0.9186393,
        "height": 473,
        "property": {
          "detectedLanguages": [
            {
              "confidence": 1,
              "languageCode": "pt"
            }
          ]
        },
        "width": 474
      }
    ],
    "text": "MENTES IMPLACÁVEIS-\nHÁ APENAS UMA\nMANEIRA DE\nEVITAR CRÍTICAS:\nNÃO FAÇA NADA,\nNÃO DIGA NADA,\nE NÃO SEJA NADA.\n- ARISTÓTELES"
  },
  "imagePropertiesAnnotation": {
    "cropHints": [
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 23
            },
            {
              "x": 402
            },
            {
              "x": 402,
              "y": 472
            },
            {
              "x": 23,
              "y": 472
            }
          ]
        },
        "confidence": 0.52845865,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {},
            {
              "x": 473
            },
            {
              "x": 473,
              "y": 472
            },
            {
              "y": 472
            }
          ]
        },
        "confidence": 0.42276692,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "y": 39
            },
            {
              "x": 473,
              "y": 39
            },
            {
              "x": 473,
              "y": 433
            },
            {
              "y": 433
            }
          ]
        },
        "confidence": 0.505182,
        "importanceFraction": 1
      }
    ],
    "dominantColors": {
      "colors": [
        {
          "color": {
            "blue": 187,
            "green": 191,
            "red": 201
          },
          "hex": "C9BFBB",
          "percent": 23.269000113711332,
          "percentRounded": 23,
          "pixelFraction": 0.0531819,
          "rgb": "201, 191,\n 187",
          "score": 0.2119083
        },
        {
          "color": {
            "blue": 11,
            "green": 13,
            "red": 14
          },
          "hex": "0E0D0B",
          "percent": 7.474730202028466,
          "percentRounded": 7,
          "pixelFraction": 0.62406105,
          "rgb": "14, 13,\n 11",
          "score": 0.06807157
        },
        {
          "color": {
            "blue": 121,
            "green": 187,
            "red": 187
          },
          "hex": "BBBB79",
          "percent": 0.39062406942915157,
          "percentRounded": 0,
          "pixelFraction": 0.0007211105,
          "rgb": "187, 187,\n 121",
          "score": 0.0035573717
        },
        {
          "color": {
            "blue": 152,
            "green": 156,
            "red": 167
          },
          "hex": "A79C98",
          "percent": 17.25594291464521,
          "percentRounded": 17,
          "pixelFraction": 0.052641068,
          "rgb": "167, 156,\n 152",
          "score": 0.15714803
        },
        {
          "color": {
            "blue": 111,
            "green": 117,
            "red": 126
          },
          "hex": "7E756F",
          "percent": 14.044717175325857,
          "percentRounded": 14,
          "pixelFraction": 0.055886064,
          "rgb": "126, 117,\n 111",
          "score": 0.12790374
        },
        {
          "color": {
            "blue": 229,
            "green": 230,
            "red": 236
          },
          "hex": "ECE6E5",
          "percent": 13.795454343487155,
          "percentRounded": 14,
          "pixelFraction": 0.034192655,
          "rgb": "236, 230,\n 229",
          "score": 0.12563373
        },
        {
          "color": {
            "blue": 78,
            "green": 84,
            "red": 88
          },
          "hex": "58544E",
          "percent": 9.425132992338018,
          "percentRounded": 9,
          "pixelFraction": 0.04759329,
          "rgb": "88, 84,\n 78",
          "score": 0.08583368
        },
        {
          "color": {
            "blue": 50,
            "green": 55,
            "red": 58
          },
          "hex": "3A3732",
          "percent": 6.0397002038119965,
          "percentRounded": 6,
          "pixelFraction": 0.039060153,
          "rgb": "58, 55,\n 50",
          "score": 0.055002905
        },
        {
          "color": {
            "blue": 64,
            "green": 80,
            "red": 90
          },
          "hex": "5A5040",
          "percent": 4.383094532611248,
          "percentRounded": 4,
          "pixelFraction": 0.01886906,
          "rgb": "90, 80,\n 64",
          "score": 0.039916374
        },
        {
          "color": {
            "blue": 99,
            "green": 115,
            "red": 129
          },
          "hex": "817363",
          "percent": 3.921603452611549,
          "percentRounded": 4,
          "pixelFraction": 0.006309717,
          "rgb": "129, 115,\n 99",
          "score": 0.035713624
        }
      ]
    }
  },
  "labelAnnotations": [
    {
      "description": "Jaw",
      "mid": "/m/01k9lj",
      "score": 0.8766561,
      "topicality": 0.8766561
    },
    {
      "description": "Sculpture",
      "mid": "/m/06msq",
      "score": 0.8611944,
      "topicality": 0.8611944
    },
    {
      "description": "Font",
      "mid": "/m/03gq5hm",
      "score": 0.82353973,
      "topicality": 0.82353973
    },
    {
      "description": "Art",
      "mid": "/m/0jjw",
      "score": 0.78026354,
      "topicality": 0.78026354
    },
    {
      "description": "Statue",
      "mid": "/m/013_1c",
      "score": 0.7605675,
      "topicality": 0.7605675
    },
    {
      "description": "Artifact",
      "mid": "/m/02skpt",
      "score": 0.68490624,
      "topicality": 0.68490624
    },
    {
      "description": "Photo caption",
      "mid": "/m/0b75wg4",
      "score": 0.67860115,
      "topicality": 0.67860115
    },
    {
      "description": "Monument",
      "mid": "/m/02ljgl",
      "score": 0.6471326,
      "topicality": 0.6471326
    },
    {
      "description": "No expression",
      "mid": "/j/9_bhpn",
      "score": 0.6450222,
      "topicality": 0.6450222
    },
    {
      "description": "History",
      "mid": "/m/03g3w",
      "score": 0.6134856,
      "topicality": 0.6134856
    },
    {
      "description": "Metal",
      "mid": "/m/04t7l",
      "score": 0.6099177,
      "topicality": 0.6099177
    },
    {
      "description": "Visual arts",
      "mid": "/m/0p9xx",
      "score": 0.60398585,
      "topicality": 0.60398585
    },
    {
      "description": "Moustache",
      "mid": "/m/0bby24z",
      "score": 0.58563507,
      "topicality": 0.58563507
    },
    {
      "description": "Advertising",
      "mid": "/m/011s0",
      "score": 0.52895516,
      "topicality": 0.52895516
    },
    {
      "description": "Classical sculpture",
      "mid": "/m/095yjj",
      "score": 0.52273,
      "topicality": 0.52273
    },
    {
      "description": "Display device",
      "mid": "/m/029zz6",
      "score": 0.5112891,
      "topicality": 0.5112891
    },
    {
      "description": "Wrinkle",
      "mid": "/m/02_x63",
      "score": 0.50407267,
      "topicality": 0.50407267
    },
    {
      "description": "Multimedia",
      "mid": "/m/0541p",
      "score": 0.5036988,
      "topicality": 0.5036988
    }
  ],
  "localizedObjectAnnotations": [
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "y": 0.13964844
          },
          {
            "x": 0.48242188,
            "y": 0.13964844
          },
          {
            "x": 0.48242188,
            "y": 1
          },
          {
            "y": 1
          }
        ]
      },
      "mid": "/m/04yqq2",
      "name": "Bust",
      "score": 0.7978093
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "y": 0.13964844
          },
          {
            "x": 0.48242188,
            "y": 0.13964844
          },
          {
            "x": 0.48242188,
            "y": 1
          },
          {
            "y": 1
          }
        ]
      },
      "mid": "/m/06msq",
      "name": "Sculpture",
      "score": 0.5122475
    }
  ],
  "safeSearchAnnotation": {
    "adult": "VERY_UNLIKELY",
    "medical": "VERY_UNLIKELY",
    "racy": "VERY_UNLIKELY",
    "spoof": "VERY_LIKELY",
    "violence": "UNLIKELY"
  },
  "textAnnotations": [
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 225,
            "y": 70
          },
          {
            "x": 414,
            "y": 70
          },
          {
            "x": 414,
            "y": 412
          },
          {
            "x": 225,
            "y": 412
          }
        ]
      },
      "description": "MENTES IMPLACÁVEIS-\nHÁ APENAS UMA\nMANEIRA DE\nEVITAR CRÍTICAS:\nNÃO FAÇA NADA,\nNÃO DIGA NADA,\nE NÃO SEJA NADA.\n- ARISTÓTELES",
      "locale": "pt"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 291,
            "y": 70
          },
          {
            "x": 319,
            "y": 70
          },
          {
            "x": 319,
            "y": 84
          },
          {
            "x": 291,
            "y": 84
          }
        ]
      },
      "description": "MENTES"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 321,
            "y": 70
          },
          {
            "x": 372,
            "y": 71
          },
          {
            "x": 372,
            "y": 85
          },
          {
            "x": 321,
            "y": 84
          }
        ]
      },
      "description": "IMPLACÁVEIS-"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 233,
            "y": 108
          },
          {
            "x": 262,
            "y": 108
          },
          {
            "x": 262,
            "y": 135
          },
          {
            "x": 233,
            "y": 135
          }
        ]
      },
      "description": "HÁ"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 266,
            "y": 108
          },
          {
            "x": 350,
            "y": 109
          },
          {
            "x": 350,
            "y": 136
          },
          {
            "x": 266,
            "y": 135
          }
        ]
      },
      "description": "APENAS"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 355,
            "y": 109
          },
          {
            "x": 403,
            "y": 110
          },
          {
            "x": 403,
            "y": 138
          },
          {
            "x": 355,
            "y": 137
          }
        ]
      },
      "description": "UMA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 254,
            "y": 158
          },
          {
            "x": 348,
            "y": 158
          },
          {
            "x": 348,
            "y": 182
          },
          {
            "x": 254,
            "y": 182
          }
        ]
      },
      "description": "MANEIRA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 354,
            "y": 158
          },
          {
            "x": 382,
            "y": 158
          },
          {
            "x": 382,
            "y": 182
          },
          {
            "x": 354,
            "y": 182
          }
        ]
      },
      "description": "DE"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 227,
            "y": 201
          },
          {
            "x": 300,
            "y": 200
          },
          {
            "x": 301,
            "y": 230
          },
          {
            "x": 228,
            "y": 231
          }
        ]
      },
      "description": "EVITAR"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 304,
            "y": 200
          },
          {
            "x": 399,
            "y": 198
          },
          {
            "x": 400,
            "y": 227
          },
          {
            "x": 305,
            "y": 229
          }
        ]
      },
      "description": "CRÍTICAS"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 399,
            "y": 198
          },
          {
            "x": 406,
            "y": 198
          },
          {
            "x": 407,
            "y": 227
          },
          {
            "x": 400,
            "y": 227
          }
        ]
      },
      "description": ":"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 233,
            "y": 246
          },
          {
            "x": 276,
            "y": 247
          },
          {
            "x": 275,
            "y": 278
          },
          {
            "x": 232,
            "y": 277
          }
        ]
      },
      "description": "NÃO"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 280,
            "y": 247
          },
          {
            "x": 336,
            "y": 248
          },
          {
            "x": 335,
            "y": 279
          },
          {
            "x": 279,
            "y": 278
          }
        ]
      },
      "description": "FAÇA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 340,
            "y": 249
          },
          {
            "x": 398,
            "y": 250
          },
          {
            "x": 397,
            "y": 280
          },
          {
            "x": 339,
            "y": 279
          }
        ]
      },
      "description": "NADA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 397,
            "y": 250
          },
          {
            "x": 404,
            "y": 250
          },
          {
            "x": 403,
            "y": 280
          },
          {
            "x": 396,
            "y": 280
          }
        ]
      },
      "description": ","
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 234,
            "y": 292
          },
          {
            "x": 278,
            "y": 293
          },
          {
            "x": 277,
            "y": 322
          },
          {
            "x": 233,
            "y": 321
          }
        ]
      },
      "description": "NÃO"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 283,
            "y": 293
          },
          {
            "x": 333,
            "y": 294
          },
          {
            "x": 332,
            "y": 323
          },
          {
            "x": 282,
            "y": 322
          }
        ]
      },
      "description": "DIGA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 337,
            "y": 295
          },
          {
            "x": 396,
            "y": 297
          },
          {
            "x": 395,
            "y": 326
          },
          {
            "x": 336,
            "y": 324
          }
        ]
      },
      "description": "NADA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 395,
            "y": 297
          },
          {
            "x": 402,
            "y": 297
          },
          {
            "x": 401,
            "y": 325
          },
          {
            "x": 394,
            "y": 325
          }
        ]
      },
      "description": ","
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 226,
            "y": 340
          },
          {
            "x": 238,
            "y": 340
          },
          {
            "x": 237,
            "y": 368
          },
          {
            "x": 225,
            "y": 368
          }
        ]
      },
      "description": "E"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 244,
            "y": 339
          },
          {
            "x": 286,
            "y": 340
          },
          {
            "x": 285,
            "y": 369
          },
          {
            "x": 243,
            "y": 368
          }
        ]
      },
      "description": "NÃO"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 291,
            "y": 340
          },
          {
            "x": 341,
            "y": 341
          },
          {
            "x": 340,
            "y": 370
          },
          {
            "x": 290,
            "y": 369
          }
        ]
      },
      "description": "SEJA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 347,
            "y": 341
          },
          {
            "x": 405,
            "y": 342
          },
          {
            "x": 404,
            "y": 371
          },
          {
            "x": 346,
            "y": 370
          }
        ]
      },
      "description": "NADA"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 405,
            "y": 343
          },
          {
            "x": 412,
            "y": 343
          },
          {
            "x": 411,
            "y": 371
          },
          {
            "x": 404,
            "y": 371
          }
        ]
      },
      "description": "."
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 252,
            "y": 386
          },
          {
            "x": 262,
            "y": 386
          },
          {
            "x": 262,
            "y": 410
          },
          {
            "x": 252,
            "y": 410
          }
        ]
      },
      "description": "-"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 263,
            "y": 385
          },
          {
            "x": 382,
            "y": 384
          },
          {
            "x": 382,
            "y": 408
          },
          {
            "x": 263,
            "y": 409
          }
        ]
      },
      "description": "ARISTÓTELES"
    }
  ]
}


