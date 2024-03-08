## Usando cloud Vision API
![Screenshot_2](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/05f5f440-4932-493a-bb59-91b11de550b7)

## Acessando a página de testes da API
![Screenshot_6](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/61775316-dc97-4727-bdc0-d768ac42d354)

## Inserindo a primeira imagem para teste:
![Screenshot_7](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/9af064ba-3c00-40df-8ee1-e1dcba2f1ddb)

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
        "content": "(data from b18f70ec427b90e924a39ae4e29f8118.jpg)"
      },
      "imageContext": {
        "cropHintsParams": {
          "aspectRatios": [
            0.8,
            1,
            1.2
          ]

## Arquivo JSON - Response
{
  "cropHintsAnnotation": {
    "cropHints": [
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 147
            },
            {
              "x": 719
            },
            {
              "x": 719,
              "y": 715
            },
            {
              "x": 147,
              "y": 715
            }
          ]
        },
        "confidence": 0.32652104,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 4
            },
            {
              "x": 719
            },
            {
              "x": 719,
              "y": 715
            },
            {
              "x": 4,
              "y": 715
            }
          ]
        },
        "confidence": 0.26121682,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "y": 57
            },
            {
              "x": 719,
              "y": 57
            },
            {
              "x": 719,
              "y": 658
            },
            {
              "y": 658
            }
          ]
        },
        "confidence": 0.30998698,
        "importanceFraction": 1
      }
    ]
  },
  "faceAnnotations": [
    {
      "angerLikelihood": "VERY_UNLIKELY",
      "blurredLikelihood": "VERY_UNLIKELY",
      "boundingPoly": {
        "vertices": [
          {
            "x": 364,
            "y": 13
          },
          {
            "x": 719,
            "y": 13
          },
          {
            "x": 719,
            "y": 553
          },
          {
            "x": 364,
            "y": 553
          }
        ]
      },
      "detectionConfidence": 0.98046875,
      "fdBoundingPoly": {
        "vertices": [
          {
            "x": 407,
            "y": 135
          },
          {
            "x": 719,
            "y": 135
          },
          {
            "x": 719,
            "y": 501
          },
          {
            "x": 407,
            "y": 501
          }
        ]
      },
      "headwearLikelihood": "VERY_UNLIKELY",
      "joyLikelihood": "VERY_UNLIKELY",
      "landmarkingConfidence": 0.58495873,
      "landmarks": [
        {
          "position": {
            "x": 524.3721,
            "y": 267.6605,
            "z": -0.00058317184
          },
          "type": "LEFT_EYE"
        },
        {
          "position": {
            "x": 660.72186,
            "y": 268.18536,
            "z": -3.8767233
          },
          "type": "RIGHT_EYE"
        },
        {
          "position": {
            "x": 478.45294,
            "y": 242.40271,
            "z": 13.543232
          },
          "type": "LEFT_OF_LEFT_EYEBROW"
        },
        {
          "position": {
            "x": 564.7016,
            "y": 236.53119,
            "z": -26.959677
          },
          "type": "RIGHT_OF_LEFT_EYEBROW"
        },
        {
          "position": {
            "x": 625.2295,
            "y": 234.31003,
            "z": -28.599905
          },
          "type": "LEFT_OF_RIGHT_EYEBROW"
        },
        {
          "position": {
            "x": 708.6275,
            "y": 242.84988,
            "z": 7.03328
          },
          "type": "RIGHT_OF_RIGHT_EYEBROW"
        },
        {
          "position": {
            "x": 595.9033,
            "y": 261.92587,
            "z": -30.264456
          },
          "type": "MIDPOINT_BETWEEN_EYES"
        },
        {
          "position": {
            "x": 589.11926,
            "y": 342.74652,
            "z": -72.27574
          },
          "type": "NOSE_TIP"
        },
        {
          "position": {
            "x": 590.32874,
            "y": 402.633,
            "z": -42.96387
          },
          "type": "UPPER_LIP"
        },
        {
          "position": {
            "x": 587.1592,
            "y": 447.79037,
            "z": -34.23557
          },
          "type": "LOWER_LIP"
        },
        {
          "position": {
            "x": 533.19214,
            "y": 424.674,
            "z": -5.4743514
          },
          "type": "MOUTH_LEFT"
        },
        {
          "position": {
            "x": 651.3287,
            "y": 422.1369,
            "z": -8.173853
          },
          "type": "MOUTH_RIGHT"
        },
        {
          "position": {
            "x": 589.5359,
            "y": 419.38577,
            "z": -33.01214
          },
          "type": "MOUTH_CENTER"
        },
        {
          "position": {
            "x": 631.80927,
            "y": 362.69098,
            "z": -23.525894
          },
          "type": "NOSE_BOTTOM_RIGHT"
        },
        {
          "position": {
            "x": 553.8479,
            "y": 360.29333,
            "z": -21.044369
          },
          "type": "NOSE_BOTTOM_LEFT"
        },
        {
          "position": {
            "x": 591.2685,
            "y": 371.61163,
            "z": -42.712772
          },
          "type": "NOSE_BOTTOM_CENTER"
        },
        {
          "position": {
            "x": 523.26385,
            "y": 254.08896,
            "z": -7.5135593
          },
          "type": "LEFT_EYE_TOP_BOUNDARY"
        },
        {
          "position": {
            "x": 553.60846,
            "y": 268.44196,
            "z": -0.9117849
          },
          "type": "LEFT_EYE_RIGHT_CORNER"
        },
        {
          "position": {
            "x": 523.2003,
            "y": 278.45197,
            "z": -1.6834812
          },
          "type": "LEFT_EYE_BOTTOM_BOUNDARY"
        },
        {
          "position": {
            "x": 494.05722,
            "y": 271.36755,
            "z": 13.09617
          },
          "type": "LEFT_EYE_LEFT_CORNER"
        },
        {
          "position": {
            "x": 661.70667,
            "y": 256.1729,
            "z": -11.721596
          },
          "type": "RIGHT_EYE_TOP_BOUNDARY"
        },
        {
          "position": {
            "x": 689.6477,
            "y": 270.66626,
            "z": 7.660874
          },
          "type": "RIGHT_EYE_RIGHT_CORNER"
        },
        {
          "position": {
            "x": 660.983,
            "y": 278.27,
            "z": -5.548498
          },
          "type": "RIGHT_EYE_BOTTOM_BOUNDARY"
        },
        {
          "position": {
            "x": 636.9046,
            "y": 268.18445,
            "z": -3.2243013
          },
          "type": "RIGHT_EYE_LEFT_CORNER"
        },
        {
          "position": {
            "x": 522.0596,
            "y": 225.59036,
            "z": -14.919213
          },
          "type": "LEFT_EYEBROW_UPPER_MIDPOINT"
        },
        {
          "position": {
            "x": 667.3346,
            "y": 224.96542,
            "z": -19.042536
          },
          "type": "RIGHT_EYEBROW_UPPER_MIDPOINT"
        },
        {
          "position": {
            "x": 439.77777,
            "y": 316.8759,
            "z": 173.23656
          },
          "type": "LEFT_EAR_TRAGION"
        },
        {
          "position": {
            "x": 757.07764,
            "y": 320.9482,
            "z": 163.91194
          },
          "type": "RIGHT_EAR_TRAGION"
        },
        {
          "position": {
            "x": 596.5209,
            "y": 232.82169,
            "z": -32.346695
          },
          "type": "FOREHEAD_GLABELLA"
        },
        {
          "position": {
            "x": 587.91296,
            "y": 518.0046,
            "z": -16.488018
          },
          "type": "CHIN_GNATHION"
        },
        {
          "position": {
            "x": 469.91815,
            "y": 442.20074,
            "z": 112.04179
          },
          "type": "CHIN_LEFT_GONION"
        },
        {
          "position": {
            "x": 711.8119,
            "y": 438.76166,
            "z": 105.04334
          },
          "type": "CHIN_RIGHT_GONION"
        },
        {
          "position": {
            "x": 493.7029,
            "y": 365.54132,
            "z": 11.0367775
          },
          "type": "LEFT_CHEEK_CENTER"
        },
        {
          "position": {
            "x": 685.6161,
            "y": 364.21948,
            "z": 5.878686
          },
          "type": "RIGHT_CHEEK_CENTER"
        }
      ],
      "panAngle": -1.6596324,
      "rollAngle": 0.92920595,
      "sorrowLikelihood": "VERY_UNLIKELY",
      "surpriseLikelihood": "VERY_UNLIKELY",
      "tiltAngle": 0.46214604,
      "underExposedLikelihood": "VERY_UNLIKELY"
    }
  ],
  "fullTextAnnotation": {
    "pages": [
      {
        "blocks": [
          {
            "blockType": "TEXT",
            "boundingBox": {
              "vertices": [
                {
                  "x": 34,
                  "y": 104
                },
                {
                  "x": 403,
                  "y": 105
                },
                {
                  "x": 403,
                  "y": 304
                },
                {
                  "x": 34,
                  "y": 303
                }
              ]
            },
            "confidence": 0.9803589,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 75,
                      "y": 104
                    },
                    {
                      "x": 361,
                      "y": 106
                    },
                    {
                      "x": 361,
                      "y": 133
                    },
                    {
                      "x": 75,
                      "y": 131
                    }
                  ]
                },
                "confidence": 0.98631805,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 75,
                          "y": 105
                        },
                        {
                          "x": 89,
                          "y": 105
                        },
                        {
                          "x": 89,
                          "y": 131
                        },
                        {
                          "x": 75,
                          "y": 131
                        }
                      ]
                    },
                    "confidence": 0.9343297,
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
                              "x": 75,
                              "y": 105
                            },
                            {
                              "x": 89,
                              "y": 105
                            },
                            {
                              "x": 89,
                              "y": 131
                            },
                            {
                              "x": 75,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.9343297,
                        "text": "\""
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 86,
                          "y": 104
                        },
                        {
                          "x": 164,
                          "y": 105
                        },
                        {
                          "x": 164,
                          "y": 132
                        },
                        {
                          "x": 86,
                          "y": 131
                        }
                      ]
                    },
                    "confidence": 0.99025226,
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
                              "x": 86,
                              "y": 105
                            },
                            {
                              "x": 105,
                              "y": 105
                            },
                            {
                              "x": 105,
                              "y": 131
                            },
                            {
                              "x": 86,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.98328495,
                        "text": "T"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 102,
                              "y": 105
                            },
                            {
                              "x": 118,
                              "y": 105
                            },
                            {
                              "x": 118,
                              "y": 131
                            },
                            {
                              "x": 102,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.99229974,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 117,
                              "y": 105
                            },
                            {
                              "x": 133,
                              "y": 105
                            },
                            {
                              "x": 133,
                              "y": 131
                            },
                            {
                              "x": 117,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.99310243,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 137,
                              "y": 105
                            },
                            {
                              "x": 152,
                              "y": 105
                            },
                            {
                              "x": 152,
                              "y": 131
                            },
                            {
                              "x": 137,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.9895394,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 153,
                              "y": 105
                            },
                            {
                              "x": 164,
                              "y": 105
                            },
                            {
                              "x": 164,
                              "y": 131
                            },
                            {
                              "x": 153,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.9930348,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 173,
                          "y": 105
                        },
                        {
                          "x": 201,
                          "y": 105
                        },
                        {
                          "x": 201,
                          "y": 131
                        },
                        {
                          "x": 173,
                          "y": 131
                        }
                      ]
                    },
                    "confidence": 0.9748217,
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
                              "x": 173,
                              "y": 105
                            },
                            {
                              "x": 187,
                              "y": 105
                            },
                            {
                              "x": 187,
                              "y": 131
                            },
                            {
                              "x": 173,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.97396845,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 190,
                              "y": 105
                            },
                            {
                              "x": 201,
                              "y": 105
                            },
                            {
                              "x": 201,
                              "y": 131
                            },
                            {
                              "x": 190,
                              "y": 131
                            }
                          ]
                        },
                        "confidence": 0.97567487,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 209,
                          "y": 105
                        },
                        {
                          "x": 361,
                          "y": 106
                        },
                        {
                          "x": 361,
                          "y": 133
                        },
                        {
                          "x": 209,
                          "y": 132
                        }
                      ]
                    },
                    "confidence": 0.9909272,
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
                              "x": 209,
                              "y": 106
                            },
                            {
                              "x": 224,
                              "y": 106
                            },
                            {
                              "x": 224,
                              "y": 132
                            },
                            {
                              "x": 209,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.98783386,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 227,
                              "y": 106
                            },
                            {
                              "x": 232,
                              "y": 106
                            },
                            {
                              "x": 232,
                              "y": 132
                            },
                            {
                              "x": 227,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.99683815,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 235,
                              "y": 106
                            },
                            {
                              "x": 246,
                              "y": 106
                            },
                            {
                              "x": 246,
                              "y": 132
                            },
                            {
                              "x": 235,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.9927163,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 249,
                              "y": 106
                            },
                            {
                              "x": 265,
                              "y": 106
                            },
                            {
                              "x": 265,
                              "y": 132
                            },
                            {
                              "x": 249,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.991078,
                        "text": "p"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 265,
                              "y": 106
                            },
                            {
                              "x": 282,
                              "y": 106
                            },
                            {
                              "x": 282,
                              "y": 132
                            },
                            {
                              "x": 265,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.99012613,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 282,
                              "y": 106
                            },
                            {
                              "x": 295,
                              "y": 106
                            },
                            {
                              "x": 295,
                              "y": 132
                            },
                            {
                              "x": 282,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.9955076,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 295,
                              "y": 106
                            },
                            {
                              "x": 300,
                              "y": 106
                            },
                            {
                              "x": 300,
                              "y": 132
                            },
                            {
                              "x": 295,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.9960291,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 301,
                              "y": 106
                            },
                            {
                              "x": 311,
                              "y": 106
                            },
                            {
                              "x": 311,
                              "y": 132
                            },
                            {
                              "x": 301,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.9961542,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 312,
                              "y": 106
                            },
                            {
                              "x": 317,
                              "y": 106
                            },
                            {
                              "x": 317,
                              "y": 132
                            },
                            {
                              "x": 312,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.99454623,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 317,
                              "y": 106
                            },
                            {
                              "x": 332,
                              "y": 106
                            },
                            {
                              "x": 332,
                              "y": 132
                            },
                            {
                              "x": 317,
                              "y": 132
                            }
                          ]
                        },
                        "confidence": 0.992779,
                        "text": "v"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 333,
                              "y": 107
                            },
                            {
                              "x": 349,
                              "y": 107
                            },
                            {
                              "x": 349,
                              "y": 133
                            },
                            {
                              "x": 333,
                              "y": 133
                            }
                          ]
                        },
                        "confidence": 0.98409986,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 349,
                              "y": 107
                            },
                            {
                              "x": 361,
                              "y": 107
                            },
                            {
                              "x": 361,
                              "y": 133
                            },
                            {
                              "x": 349,
                              "y": 133
                            }
                          ]
                        },
                        "confidence": 0.97341794,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 34,
                      "y": 149
                    },
                    {
                      "x": 403,
                      "y": 149
                    },
                    {
                      "x": 403,
                      "y": 170
                    },
                    {
                      "x": 34,
                      "y": 170
                    }
                  ]
                },
                "confidence": 0.98850787,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 34,
                          "y": 149
                        },
                        {
                          "x": 185,
                          "y": 149
                        },
                        {
                          "x": 185,
                          "y": 170
                        },
                        {
                          "x": 34,
                          "y": 170
                        }
                      ]
                    },
                    "confidence": 0.9887371,
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
                              "x": 34,
                              "y": 149
                            },
                            {
                              "x": 47,
                              "y": 149
                            },
                            {
                              "x": 47,
                              "y": 170
                            },
                            {
                              "x": 34,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.95918405,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 48,
                              "y": 149
                            },
                            {
                              "x": 63,
                              "y": 149
                            },
                            {
                              "x": 63,
                              "y": 170
                            },
                            {
                              "x": 48,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9779008,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 64,
                              "y": 149
                            },
                            {
                              "x": 74,
                              "y": 149
                            },
                            {
                              "x": 74,
                              "y": 170
                            },
                            {
                              "x": 64,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99117947,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 74,
                              "y": 149
                            },
                            {
                              "x": 79,
                              "y": 149
                            },
                            {
                              "x": 79,
                              "y": 170
                            },
                            {
                              "x": 74,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9954876,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 81,
                              "y": 149
                            },
                            {
                              "x": 92,
                              "y": 149
                            },
                            {
                              "x": 92,
                              "y": 170
                            },
                            {
                              "x": 81,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9952066,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 92,
                              "y": 149
                            },
                            {
                              "x": 100,
                              "y": 149
                            },
                            {
                              "x": 100,
                              "y": 170
                            },
                            {
                              "x": 92,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9961472,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 103,
                              "y": 149
                            },
                            {
                              "x": 107,
                              "y": 149
                            },
                            {
                              "x": 107,
                              "y": 170
                            },
                            {
                              "x": 103,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99553967,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 110,
                              "y": 149
                            },
                            {
                              "x": 123,
                              "y": 149
                            },
                            {
                              "x": 123,
                              "y": 170
                            },
                            {
                              "x": 110,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99484503,
                        "text": "c"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 123,
                              "y": 149
                            },
                            {
                              "x": 136,
                              "y": 149
                            },
                            {
                              "x": 136,
                              "y": 170
                            },
                            {
                              "x": 123,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99638313,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 138,
                              "y": 149
                            },
                            {
                              "x": 153,
                              "y": 149
                            },
                            {
                              "x": 153,
                              "y": 170
                            },
                            {
                              "x": 138,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9933558,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 156,
                              "y": 149
                            },
                            {
                              "x": 172,
                              "y": 149
                            },
                            {
                              "x": 172,
                              "y": 170
                            },
                            {
                              "x": 156,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.98756045,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 173,
                              "y": 149
                            },
                            {
                              "x": 185,
                              "y": 149
                            },
                            {
                              "x": 185,
                              "y": 170
                            },
                            {
                              "x": 173,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9820551,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 193,
                          "y": 149
                        },
                        {
                          "x": 208,
                          "y": 149
                        },
                        {
                          "x": 208,
                          "y": 170
                        },
                        {
                          "x": 193,
                          "y": 170
                        }
                      ]
                    },
                    "confidence": 0.9889036,
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
                              "x": 193,
                              "y": 149
                            },
                            {
                              "x": 208,
                              "y": 149
                            },
                            {
                              "x": 208,
                              "y": 170
                            },
                            {
                              "x": 193,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9889036,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "e"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 215,
                          "y": 149
                        },
                        {
                          "x": 260,
                          "y": 149
                        },
                        {
                          "x": 260,
                          "y": 170
                        },
                        {
                          "x": 215,
                          "y": 170
                        }
                      ]
                    },
                    "confidence": 0.988902,
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
                              "x": 215,
                              "y": 149
                            },
                            {
                              "x": 237,
                              "y": 149
                            },
                            {
                              "x": 237,
                              "y": 170
                            },
                            {
                              "x": 215,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9914422,
                        "text": "w"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 237,
                              "y": 149
                            },
                            {
                              "x": 245,
                              "y": 149
                            },
                            {
                              "x": 245,
                              "y": 170
                            },
                            {
                              "x": 237,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99311334,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 243,
                              "y": 149
                            },
                            {
                              "x": 254,
                              "y": 149
                            },
                            {
                              "x": 254,
                              "y": 170
                            },
                            {
                              "x": 243,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.98276895,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 252,
                              "y": 149
                            },
                            {
                              "x": 260,
                              "y": 149
                            },
                            {
                              "x": 260,
                              "y": 170
                            },
                            {
                              "x": 252,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9882834,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "i"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 267,
                          "y": 149
                        },
                        {
                          "x": 302,
                          "y": 149
                        },
                        {
                          "x": 302,
                          "y": 170
                        },
                        {
                          "x": 267,
                          "y": 170
                        }
                      ]
                    },
                    "confidence": 0.97710526,
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
                              "x": 267,
                              "y": 149
                            },
                            {
                              "x": 285,
                              "y": 149
                            },
                            {
                              "x": 285,
                              "y": 170
                            },
                            {
                              "x": 267,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.98285055,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 285,
                              "y": 149
                            },
                            {
                              "x": 302,
                              "y": 149
                            },
                            {
                              "x": 302,
                              "y": 170
                            },
                            {
                              "x": 285,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.97136,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "o"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 310,
                          "y": 149
                        },
                        {
                          "x": 403,
                          "y": 149
                        },
                        {
                          "x": 403,
                          "y": 170
                        },
                        {
                          "x": 310,
                          "y": 170
                        }
                      ]
                    },
                    "confidence": 0.99212426,
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
                              "x": 310,
                              "y": 149
                            },
                            {
                              "x": 333,
                              "y": 149
                            },
                            {
                              "x": 333,
                              "y": 170
                            },
                            {
                              "x": 310,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99153626,
                        "text": "m"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 333,
                              "y": 149
                            },
                            {
                              "x": 349,
                              "y": 149
                            },
                            {
                              "x": 349,
                              "y": 170
                            },
                            {
                              "x": 333,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9914415,
                        "text": "u"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 350,
                              "y": 149
                            },
                            {
                              "x": 367,
                              "y": 149
                            },
                            {
                              "x": 367,
                              "y": 170
                            },
                            {
                              "x": 350,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99350744,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 366,
                              "y": 149
                            },
                            {
                              "x": 385,
                              "y": 149
                            },
                            {
                              "x": 385,
                              "y": 170
                            },
                            {
                              "x": 366,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.9940092,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 385,
                              "y": 149
                            },
                            {
                              "x": 403,
                              "y": 149
                            },
                            {
                              "x": 403,
                              "y": 170
                            },
                            {
                              "x": 385,
                              "y": 170
                            }
                          ]
                        },
                        "confidence": 0.99012697,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "o"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 52,
                      "y": 188
                    },
                    {
                      "x": 386,
                      "y": 191
                    },
                    {
                      "x": 386,
                      "y": 215
                    },
                    {
                      "x": 52,
                      "y": 212
                    }
                  ]
                },
                "confidence": 0.95935553,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 52,
                          "y": 189
                        },
                        {
                          "x": 100,
                          "y": 189
                        },
                        {
                          "x": 100,
                          "y": 212
                        },
                        {
                          "x": 52,
                          "y": 212
                        }
                      ]
                    },
                    "confidence": 0.90196043,
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
                              "x": 52,
                              "y": 189
                            },
                            {
                              "x": 67,
                              "y": 189
                            },
                            {
                              "x": 67,
                              "y": 212
                            },
                            {
                              "x": 52,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.9179534,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 67,
                              "y": 189
                            },
                            {
                              "x": 81,
                              "y": 189
                            },
                            {
                              "x": 81,
                              "y": 212
                            },
                            {
                              "x": 67,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.84858525,
                        "text": "ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 84,
                              "y": 189
                            },
                            {
                              "x": 100,
                              "y": 189
                            },
                            {
                              "x": 100,
                              "y": 212
                            },
                            {
                              "x": 84,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.9393426,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "o"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 106,
                          "y": 189
                        },
                        {
                          "x": 152,
                          "y": 189
                        },
                        {
                          "x": 152,
                          "y": 212
                        },
                        {
                          "x": 106,
                          "y": 212
                        }
                      ]
                    },
                    "confidence": 0.91749173,
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
                              "x": 106,
                              "y": 189
                            },
                            {
                              "x": 120,
                              "y": 189
                            },
                            {
                              "x": 120,
                              "y": 212
                            },
                            {
                              "x": 106,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.9464463,
                        "text": "v"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 120,
                              "y": 189
                            },
                            {
                              "x": 134,
                              "y": 189
                            },
                            {
                              "x": 134,
                              "y": 212
                            },
                            {
                              "x": 120,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.8541843,
                        "text": "ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 136,
                              "y": 189
                            },
                            {
                              "x": 152,
                              "y": 189
                            },
                            {
                              "x": 152,
                              "y": 212
                            },
                            {
                              "x": 136,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.9518445,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "o"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 159,
                          "y": 189
                        },
                        {
                          "x": 224,
                          "y": 190
                        },
                        {
                          "x": 224,
                          "y": 214
                        },
                        {
                          "x": 159,
                          "y": 213
                        }
                      ]
                    },
                    "confidence": 0.9867757,
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
                              "x": 159,
                              "y": 189
                            },
                            {
                              "x": 170,
                              "y": 189
                            },
                            {
                              "x": 170,
                              "y": 212
                            },
                            {
                              "x": 159,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.98447496,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 169,
                              "y": 189
                            },
                            {
                              "x": 183,
                              "y": 189
                            },
                            {
                              "x": 183,
                              "y": 212
                            },
                            {
                              "x": 169,
                              "y": 212
                            }
                          ]
                        },
                        "confidence": 0.97241175,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 183,
                              "y": 190
                            },
                            {
                              "x": 197,
                              "y": 190
                            },
                            {
                              "x": 197,
                              "y": 213
                            },
                            {
                              "x": 183,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.9919638,
                        "text": "z"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 195,
                              "y": 190
                            },
                            {
                              "x": 210,
                              "y": 190
                            },
                            {
                              "x": 210,
                              "y": 213
                            },
                            {
                              "x": 195,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.9923649,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 213,
                              "y": 190
                            },
                            {
                              "x": 224,
                              "y": 190
                            },
                            {
                              "x": 224,
                              "y": 213
                            },
                            {
                              "x": 213,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.9926632,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "r"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 230,
                          "y": 190
                        },
                        {
                          "x": 350,
                          "y": 191
                        },
                        {
                          "x": 350,
                          "y": 214
                        },
                        {
                          "x": 230,
                          "y": 213
                        }
                      ]
                    },
                    "confidence": 0.97439456,
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
                              "x": 230,
                              "y": 190
                            },
                            {
                              "x": 246,
                              "y": 190
                            },
                            {
                              "x": 246,
                              "y": 213
                            },
                            {
                              "x": 230,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.9898527,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 248,
                              "y": 190
                            },
                            {
                              "x": 255,
                              "y": 190
                            },
                            {
                              "x": 255,
                              "y": 213
                            },
                            {
                              "x": 248,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.97299,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 254,
                              "y": 190
                            },
                            {
                              "x": 266,
                              "y": 190
                            },
                            {
                              "x": 266,
                              "y": 213
                            },
                            {
                              "x": 254,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.99270153,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 263,
                              "y": 190
                            },
                            {
                              "x": 280,
                              "y": 190
                            },
                            {
                              "x": 280,
                              "y": 213
                            },
                            {
                              "x": 263,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.99395466,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 278,
                              "y": 190
                            },
                            {
                              "x": 291,
                              "y": 190
                            },
                            {
                              "x": 291,
                              "y": 213
                            },
                            {
                              "x": 278,
                              "y": 213
                            }
                          ]
                        },
                        "confidence": 0.9959775,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 289,
                              "y": 191
                            },
                            {
                              "x": 306,
                              "y": 191
                            },
                            {
                              "x": 306,
                              "y": 214
                            },
                            {
                              "x": 289,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.99248046,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 305,
                              "y": 191
                            },
                            {
                              "x": 320,
                              "y": 191
                            },
                            {
                              "x": 320,
                              "y": 214
                            },
                            {
                              "x": 305,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.9737022,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 320,
                              "y": 191
                            },
                            {
                              "x": 336,
                              "y": 191
                            },
                            {
                              "x": 336,
                              "y": 214
                            },
                            {
                              "x": 320,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.88896525,
                        "text": "ç"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 335,
                              "y": 191
                            },
                            {
                              "x": 350,
                              "y": 191
                            },
                            {
                              "x": 350,
                              "y": 214
                            },
                            {
                              "x": 335,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.9689268,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "a"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 356,
                          "y": 191
                        },
                        {
                          "x": 386,
                          "y": 191
                        },
                        {
                          "x": 386,
                          "y": 214
                        },
                        {
                          "x": 356,
                          "y": 214
                        }
                      ]
                    },
                    "confidence": 0.9720178,
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
                              "x": 356,
                              "y": 191
                            },
                            {
                              "x": 370,
                              "y": 191
                            },
                            {
                              "x": 370,
                              "y": 214
                            },
                            {
                              "x": 356,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.9726787,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 369,
                              "y": 191
                            },
                            {
                              "x": 386,
                              "y": 191
                            },
                            {
                              "x": 386,
                              "y": 214
                            },
                            {
                              "x": 369,
                              "y": 214
                            }
                          ]
                        },
                        "confidence": 0.9713569,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "e"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 79,
                      "y": 230
                    },
                    {
                      "x": 360,
                      "y": 233
                    },
                    {
                      "x": 360,
                      "y": 260
                    },
                    {
                      "x": 79,
                      "y": 257
                    }
                  ]
                },
                "confidence": 0.9784032,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 79,
                          "y": 231
                        },
                        {
                          "x": 127,
                          "y": 231
                        },
                        {
                          "x": 127,
                          "y": 257
                        },
                        {
                          "x": 79,
                          "y": 257
                        }
                      ]
                    },
                    "confidence": 0.9203774,
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
                              "x": 79,
                              "y": 231
                            },
                            {
                              "x": 94,
                              "y": 231
                            },
                            {
                              "x": 94,
                              "y": 257
                            },
                            {
                              "x": 79,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.92590666,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 95,
                              "y": 231
                            },
                            {
                              "x": 108,
                              "y": 231
                            },
                            {
                              "x": 108,
                              "y": 257
                            },
                            {
                              "x": 95,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.88234764,
                        "text": "ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 111,
                              "y": 231
                            },
                            {
                              "x": 127,
                              "y": 231
                            },
                            {
                              "x": 127,
                              "y": 257
                            },
                            {
                              "x": 111,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.95287776,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "o"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 133,
                          "y": 231
                        },
                        {
                          "x": 245,
                          "y": 232
                        },
                        {
                          "x": 245,
                          "y": 259
                        },
                        {
                          "x": 133,
                          "y": 258
                        }
                      ]
                    },
                    "confidence": 0.9870797,
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
                              "x": 133,
                              "y": 231
                            },
                            {
                              "x": 143,
                              "y": 231
                            },
                            {
                              "x": 143,
                              "y": 257
                            },
                            {
                              "x": 133,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.9932943,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 144,
                              "y": 231
                            },
                            {
                              "x": 149,
                              "y": 231
                            },
                            {
                              "x": 149,
                              "y": 257
                            },
                            {
                              "x": 144,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.9946746,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 151,
                              "y": 231
                            },
                            {
                              "x": 165,
                              "y": 231
                            },
                            {
                              "x": 165,
                              "y": 257
                            },
                            {
                              "x": 151,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.994918,
                        "text": "v"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 164,
                              "y": 231
                            },
                            {
                              "x": 179,
                              "y": 231
                            },
                            {
                              "x": 179,
                              "y": 257
                            },
                            {
                              "x": 164,
                              "y": 257
                            }
                          ]
                        },
                        "confidence": 0.99248254,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 181,
                              "y": 232
                            },
                            {
                              "x": 191,
                              "y": 232
                            },
                            {
                              "x": 191,
                              "y": 258
                            },
                            {
                              "x": 181,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.9873283,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 191,
                              "y": 232
                            },
                            {
                              "x": 214,
                              "y": 232
                            },
                            {
                              "x": 214,
                              "y": 258
                            },
                            {
                              "x": 191,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.9890179,
                        "text": "m"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 215,
                              "y": 232
                            },
                            {
                              "x": 231,
                              "y": 232
                            },
                            {
                              "x": 231,
                              "y": 258
                            },
                            {
                              "x": 215,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.9832057,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 232,
                              "y": 232
                            },
                            {
                              "x": 245,
                              "y": 232
                            },
                            {
                              "x": 245,
                              "y": 258
                            },
                            {
                              "x": 232,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.9617161,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 253,
                          "y": 232
                        },
                        {
                          "x": 360,
                          "y": 233
                        },
                        {
                          "x": 360,
                          "y": 260
                        },
                        {
                          "x": 253,
                          "y": 259
                        }
                      ]
                    },
                    "confidence": 0.9933556,
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
                              "x": 253,
                              "y": 232
                            },
                            {
                              "x": 269,
                              "y": 232
                            },
                            {
                              "x": 269,
                              "y": 258
                            },
                            {
                              "x": 253,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.98789597,
                        "text": "g"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 271,
                              "y": 232
                            },
                            {
                              "x": 283,
                              "y": 232
                            },
                            {
                              "x": 283,
                              "y": 258
                            },
                            {
                              "x": 271,
                              "y": 258
                            }
                          ]
                        },
                        "confidence": 0.9919773,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 280,
                              "y": 233
                            },
                            {
                              "x": 296,
                              "y": 233
                            },
                            {
                              "x": 296,
                              "y": 259
                            },
                            {
                              "x": 280,
                              "y": 259
                            }
                          ]
                        },
                        "confidence": 0.99430424,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 296,
                              "y": 233
                            },
                            {
                              "x": 312,
                              "y": 233
                            },
                            {
                              "x": 312,
                              "y": 259
                            },
                            {
                              "x": 296,
                              "y": 259
                            }
                          ]
                        },
                        "confidence": 0.9948801,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 311,
                              "y": 233
                            },
                            {
                              "x": 329,
                              "y": 233
                            },
                            {
                              "x": 329,
                              "y": 259
                            },
                            {
                              "x": 311,
                              "y": 259
                            }
                          ]
                        },
                        "confidence": 0.9946528,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 329,
                              "y": 233
                            },
                            {
                              "x": 346,
                              "y": 233
                            },
                            {
                              "x": 346,
                              "y": 259
                            },
                            {
                              "x": 329,
                              "y": 259
                            }
                          ]
                        },
                        "confidence": 0.99668723,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 345,
                              "y": 233
                            },
                            {
                              "x": 360,
                              "y": 233
                            },
                            {
                              "x": 360,
                              "y": 259
                            },
                            {
                              "x": 345,
                              "y": 259
                            }
                          ]
                        },
                        "confidence": 0.9930912,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  }
                ]
              },
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 92,
                      "y": 277
                    },
                    {
                      "x": 345,
                      "y": 273
                    },
                    {
                      "x": 345,
                      "y": 299
                    },
                    {
                      "x": 92,
                      "y": 303
                    }
                  ]
                },
                "confidence": 0.99109524,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 92,
                          "y": 277
                        },
                        {
                          "x": 240,
                          "y": 275
                        },
                        {
                          "x": 240,
                          "y": 301
                        },
                        {
                          "x": 92,
                          "y": 303
                        }
                      ]
                    },
                    "confidence": 0.99182963,
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
                              "x": 92,
                              "y": 278
                            },
                            {
                              "x": 109,
                              "y": 278
                            },
                            {
                              "x": 109,
                              "y": 303
                            },
                            {
                              "x": 92,
                              "y": 303
                            }
                          ]
                        },
                        "confidence": 0.9795809,
                        "text": "p"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 108,
                              "y": 277
                            },
                            {
                              "x": 119,
                              "y": 277
                            },
                            {
                              "x": 119,
                              "y": 302
                            },
                            {
                              "x": 108,
                              "y": 302
                            }
                          ]
                        },
                        "confidence": 0.9943121,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 118,
                              "y": 277
                            },
                            {
                              "x": 135,
                              "y": 277
                            },
                            {
                              "x": 135,
                              "y": 302
                            },
                            {
                              "x": 118,
                              "y": 302
                            }
                          ]
                        },
                        "confidence": 0.9917989,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 134,
                              "y": 277
                            },
                            {
                              "x": 146,
                              "y": 277
                            },
                            {
                              "x": 146,
                              "y": 302
                            },
                            {
                              "x": 134,
                              "y": 302
                            }
                          ]
                        },
                        "confidence": 0.9942546,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 143,
                              "y": 277
                            },
                            {
                              "x": 157,
                              "y": 277
                            },
                            {
                              "x": 157,
                              "y": 302
                            },
                            {
                              "x": 143,
                              "y": 302
                            }
                          ]
                        },
                        "confidence": 0.9953019,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 159,
                              "y": 277
                            },
                            {
                              "x": 171,
                              "y": 277
                            },
                            {
                              "x": 171,
                              "y": 302
                            },
                            {
                              "x": 159,
                              "y": 302
                            }
                          ]
                        },
                        "confidence": 0.99562746,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 172,
                              "y": 276
                            },
                            {
                              "x": 185,
                              "y": 276
                            },
                            {
                              "x": 185,
                              "y": 301
                            },
                            {
                              "x": 172,
                              "y": 301
                            }
                          ]
                        },
                        "confidence": 0.9940019,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 185,
                              "y": 276
                            },
                            {
                              "x": 201,
                              "y": 276
                            },
                            {
                              "x": 201,
                              "y": 301
                            },
                            {
                              "x": 185,
                              "y": 301
                            }
                          ]
                        },
                        "confidence": 0.9931452,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 202,
                              "y": 276
                            },
                            {
                              "x": 213,
                              "y": 276
                            },
                            {
                              "x": 213,
                              "y": 301
                            },
                            {
                              "x": 202,
                              "y": 301
                            }
                          ]
                        },
                        "confidence": 0.99108076,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 211,
                              "y": 276
                            },
                            {
                              "x": 226,
                              "y": 276
                            },
                            {
                              "x": 226,
                              "y": 301
                            },
                            {
                              "x": 211,
                              "y": 301
                            }
                          ]
                        },
                        "confidence": 0.9931135,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 228,
                              "y": 276
                            },
                            {
                              "x": 240,
                              "y": 276
                            },
                            {
                              "x": 240,
                              "y": 301
                            },
                            {
                              "x": 228,
                              "y": 301
                            }
                          ]
                        },
                        "confidence": 0.9879087,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 247,
                          "y": 275
                        },
                        {
                          "x": 286,
                          "y": 274
                        },
                        {
                          "x": 286,
                          "y": 299
                        },
                        {
                          "x": 247,
                          "y": 300
                        }
                      ]
                    },
                    "confidence": 0.9902721,
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
                              "x": 247,
                              "y": 275
                            },
                            {
                              "x": 262,
                              "y": 275
                            },
                            {
                              "x": 262,
                              "y": 300
                            },
                            {
                              "x": 247,
                              "y": 300
                            }
                          ]
                        },
                        "confidence": 0.9888488,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 265,
                              "y": 275
                            },
                            {
                              "x": 286,
                              "y": 275
                            },
                            {
                              "x": 286,
                              "y": 300
                            },
                            {
                              "x": 265,
                              "y": 300
                            }
                          ]
                        },
                        "confidence": 0.9916954,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "m"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 294,
                          "y": 274
                        },
                        {
                          "x": 345,
                          "y": 273
                        },
                        {
                          "x": 345,
                          "y": 299
                        },
                        {
                          "x": 294,
                          "y": 300
                        }
                      ]
                    },
                    "confidence": 0.9894872,
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
                              "x": 294,
                              "y": 275
                            },
                            {
                              "x": 308,
                              "y": 275
                            },
                            {
                              "x": 308,
                              "y": 300
                            },
                            {
                              "x": 294,
                              "y": 300
                            }
                          ]
                        },
                        "confidence": 0.99235684,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 307,
                              "y": 274
                            },
                            {
                              "x": 321,
                              "y": 274
                            },
                            {
                              "x": 321,
                              "y": 299
                            },
                            {
                              "x": 307,
                              "y": 299
                            }
                          ]
                        },
                        "confidence": 0.98854053,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 322,
                              "y": 274
                            },
                            {
                              "x": 331,
                              "y": 274
                            },
                            {
                              "x": 331,
                              "y": 299
                            },
                            {
                              "x": 322,
                              "y": 299
                            }
                          ]
                        },
                        "confidence": 0.991507,
                        "text": "l"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 330,
                              "y": 274
                            },
                            {
                              "x": 345,
                              "y": 274
                            },
                            {
                              "x": 345,
                              "y": 299
                            },
                            {
                              "x": 330,
                              "y": 299
                            }
                          ]
                        },
                        "confidence": 0.9855442,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "a"
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
                  "x": 165,
                  "y": 319
                },
                {
                  "x": 272,
                  "y": 319
                },
                {
                  "x": 272,
                  "y": 340
                },
                {
                  "x": 165,
                  "y": 340
                }
              ]
            },
            "confidence": 0.97748196,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 165,
                      "y": 319
                    },
                    {
                      "x": 272,
                      "y": 319
                    },
                    {
                      "x": 272,
                      "y": 340
                    },
                    {
                      "x": 165,
                      "y": 340
                    }
                  ]
                },
                "confidence": 0.97748196,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 165,
                          "y": 319
                        },
                        {
                          "x": 200,
                          "y": 319
                        },
                        {
                          "x": 200,
                          "y": 340
                        },
                        {
                          "x": 165,
                          "y": 340
                        }
                      ]
                    },
                    "confidence": 0.9898235,
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
                              "x": 165,
                              "y": 319
                            },
                            {
                              "x": 182,
                              "y": 319
                            },
                            {
                              "x": 182,
                              "y": 340
                            },
                            {
                              "x": 165,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.9867622,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 184,
                              "y": 319
                            },
                            {
                              "x": 200,
                              "y": 319
                            },
                            {
                              "x": 200,
                              "y": 340
                            },
                            {
                              "x": 184,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.9928848,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "e"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 207,
                          "y": 319
                        },
                        {
                          "x": 261,
                          "y": 319
                        },
                        {
                          "x": 261,
                          "y": 340
                        },
                        {
                          "x": 207,
                          "y": 340
                        }
                      ]
                    },
                    "confidence": 0.9890997,
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
                              "x": 207,
                              "y": 319
                            },
                            {
                              "x": 222,
                              "y": 319
                            },
                            {
                              "x": 222,
                              "y": 340
                            },
                            {
                              "x": 207,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.9938749,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 223,
                              "y": 319
                            },
                            {
                              "x": 236,
                              "y": 319
                            },
                            {
                              "x": 236,
                              "y": 340
                            },
                            {
                              "x": 223,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.9910479,
                        "text": "u"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 239,
                              "y": 319
                            },
                            {
                              "x": 247,
                              "y": 319
                            },
                            {
                              "x": 247,
                              "y": 340
                            },
                            {
                              "x": 239,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.9872679,
                        "text": "l"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 246,
                              "y": 319
                            },
                            {
                              "x": 261,
                              "y": 319
                            },
                            {
                              "x": 261,
                              "y": 340
                            },
                            {
                              "x": 246,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.98420805,
                        "text": "a"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 259,
                          "y": 319
                        },
                        {
                          "x": 272,
                          "y": 319
                        },
                        {
                          "x": 272,
                          "y": 340
                        },
                        {
                          "x": 259,
                          "y": 340
                        }
                      ]
                    },
                    "confidence": 0.90632796,
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
                              "x": 259,
                              "y": 319
                            },
                            {
                              "x": 272,
                              "y": 319
                            },
                            {
                              "x": 272,
                              "y": 340
                            },
                            {
                              "x": 259,
                              "y": 340
                            }
                          ]
                        },
                        "confidence": 0.90632796,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "\""
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
                  "x": 140,
                  "y": 381
                },
                {
                  "x": 285,
                  "y": 382
                },
                {
                  "x": 285,
                  "y": 399
                },
                {
                  "x": 140,
                  "y": 398
                }
              ]
            },
            "confidence": 0.99060607,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 140,
                      "y": 381
                    },
                    {
                      "x": 285,
                      "y": 382
                    },
                    {
                      "x": 285,
                      "y": 399
                    },
                    {
                      "x": 140,
                      "y": 398
                    }
                  ]
                },
                "confidence": 0.99060607,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 140,
                          "y": 381
                        },
                        {
                          "x": 206,
                          "y": 381
                        },
                        {
                          "x": 206,
                          "y": 398
                        },
                        {
                          "x": 140,
                          "y": 398
                        }
                      ]
                    },
                    "confidence": 0.99251044,
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 140,
                              "y": 381
                            },
                            {
                              "x": 151,
                              "y": 381
                            },
                            {
                              "x": 151,
                              "y": 398
                            },
                            {
                              "x": 140,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.98883814,
                        "text": "B"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 154,
                              "y": 381
                            },
                            {
                              "x": 164,
                              "y": 381
                            },
                            {
                              "x": 164,
                              "y": 398
                            },
                            {
                              "x": 154,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.99054664,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 165,
                              "y": 381
                            },
                            {
                              "x": 172,
                              "y": 381
                            },
                            {
                              "x": 172,
                              "y": 398
                            },
                            {
                              "x": 165,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.9962677,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 173,
                              "y": 381
                            },
                            {
                              "x": 183,
                              "y": 381
                            },
                            {
                              "x": 183,
                              "y": 398
                            },
                            {
                              "x": 173,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.9951947,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 184,
                              "y": 381
                            },
                            {
                              "x": 193,
                              "y": 381
                            },
                            {
                              "x": 193,
                              "y": 398
                            },
                            {
                              "x": 184,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.9950077,
                        "text": "c"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 195,
                              "y": 381
                            },
                            {
                              "x": 206,
                              "y": 381
                            },
                            {
                              "x": 206,
                              "y": 398
                            },
                            {
                              "x": 195,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.989208,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "k"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 211,
                          "y": 381
                        },
                        {
                          "x": 285,
                          "y": 381
                        },
                        {
                          "x": 285,
                          "y": 398
                        },
                        {
                          "x": 211,
                          "y": 398
                        }
                      ]
                    },
                    "confidence": 0.98832077,
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 211,
                              "y": 381
                            },
                            {
                              "x": 229,
                              "y": 381
                            },
                            {
                              "x": 229,
                              "y": 398
                            },
                            {
                              "x": 211,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.98554945,
                        "text": "O"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 231,
                              "y": 381
                            },
                            {
                              "x": 243,
                              "y": 381
                            },
                            {
                              "x": 243,
                              "y": 398
                            },
                            {
                              "x": 231,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.9878139,
                        "text": "b"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 244,
                              "y": 381
                            },
                            {
                              "x": 253,
                              "y": 381
                            },
                            {
                              "x": 253,
                              "y": 398
                            },
                            {
                              "x": 244,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.99243295,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 256,
                              "y": 381
                            },
                            {
                              "x": 272,
                              "y": 381
                            },
                            {
                              "x": 272,
                              "y": 398
                            },
                            {
                              "x": 256,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.98767185,
                        "text": "m"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 274,
                              "y": 381
                            },
                            {
                              "x": 285,
                              "y": 381
                            },
                            {
                              "x": 285,
                              "y": 398
                            },
                            {
                              "x": 274,
                              "y": 398
                            }
                          ]
                        },
                        "confidence": 0.98813564,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "a"
                      }
                    ]
                  }
                ]
              }
            ]
          }
        ],
        "confidence": 0.9828157,
        "height": 716,
        "property": {
          "detectedLanguages": [
            {
              "confidence": 0.90667087,
              "languageCode": "pt"
            }
          ]
        },
        "width": 720
      }
    ],
    "text": "\"Todos os dispositivos\nsofisticados e wifi do mundo\nnão vão fazer diferença se\nnão tivermos grandes\nprofessores em sala\nde aula\"\nBarack Obama"
  },
  "imagePropertiesAnnotation": {
    "cropHints": [
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 147
            },
            {
              "x": 719
            },
            {
              "x": 719,
              "y": 715
            },
            {
              "x": 147,
              "y": 715
            }
          ]
        },
        "confidence": 0.32652104,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 4
            },
            {
              "x": 719
            },
            {
              "x": 719,
              "y": 715
            },
            {
              "x": 4,
              "y": 715
            }
          ]
        },
        "confidence": 0.26121682,
        "importanceFraction": 1
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "y": 57
            },
            {
              "x": 719,
              "y": 57
            },
            {
              "x": 719,
              "y": 658
            },
            {
              "y": 658
            }
          ]
        },
        "confidence": 0.30998698,
        "importanceFraction": 1
      }
    ],
    "dominantColors": {
      "colors": [
        {
          "color": {
            "blue": 193,
            "green": 188,
            "red": 188
          },
          "hex": "BCBCC1",
          "percent": 46.857335134988595,
          "percentRounded": 47,
          "pixelFraction": 0.50102776,
          "rgb": "188, 188,\n 193",
          "score": 0.41226116
        },
        {
          "color": {
            "blue": 63,
            "green": 81,
            "red": 102
          },
          "hex": "66513F",
          "percent": 8.439279418093594,
          "percentRounded": 8,
          "pixelFraction": 0.050308324,
          "rgb": "102, 81,\n 63",
          "score": 0.07425064
        },
        {
          "color": {
            "blue": 56,
            "green": 51,
            "red": 51
          },
          "hex": "333338",
          "percent": 6.0629613509703,
          "percentRounded": 6,
          "pixelFraction": 0.055395685,
          "rgb": "51, 51,\n 56",
          "score": 0.05334327
        },
        {
          "color": {
            "blue": 96,
            "green": 114,
            "red": 136
          },
          "hex": "887260",
          "percent": 8.0912481260017,
          "percentRounded": 8,
          "pixelFraction": 0.058941416,
          "rgb": "136, 114,\n 96",
          "score": 0.071188584
        },
        {
          "color": {
            "blue": 158,
            "green": 156,
            "red": 159
          },
          "hex": "9F9C9E",
          "percent": 6.765381584509439,
          "percentRounded": 7,
          "pixelFraction": 0.07235355,
          "rgb": "159, 156,\n 158",
          "score": 0.059523318
        },
        {
          "color": {
            "blue": 134,
            "green": 149,
            "red": 172
          },
          "hex": "AC9586",
          "percent": 6.608025216590506,
          "percentRounded": 7,
          "pixelFraction": 0.04208633,
          "rgb": "172, 149,\n 134",
          "score": 0.058138862
        },
        {
          "color": {
            "blue": 218,
            "green": 197,
            "red": 191
          },
          "hex": "BFC5DA",
          "percent": 4.701851091167715,
          "percentRounded": 5,
          "pixelFraction": 0.022816032,
          "rgb": "191, 197,\n 218",
          "score": 0.041367922
        },
        {
          "color": {
            "blue": 28,
            "green": 26,
            "red": 25
          },
          "hex": "191A1C",
          "percent": 4.420184242805212,
          "percentRounded": 4,
          "pixelFraction": 0.04938335,
          "rgb": "25, 26,\n 28",
          "score": 0.038889755
        },
        {
          "color": {
            "blue": 87,
            "green": 80,
            "red": 81
          },
          "hex": "515057",
          "percent": 4.080703088914222,
          "percentRounded": 4,
          "pixelFraction": 0.03504625,
          "rgb": "81, 80,\n 87",
          "score": 0.035902925
        },
        {
          "color": {
            "blue": 33,
            "green": 50,
            "red": 68
          },
          "hex": "443221",
          "percent": 3.9730307459587206,
          "percentRounded": 4,
          "pixelFraction": 0.018499486,
          "rgb": "68, 50,\n 33",
          "score": 0.0349556
        }
      ]
    }
  },
  "labelAnnotations": [
    {
      "description": "Forehead",
      "mid": "/m/025kyy",
      "score": 0.9846564,
      "topicality": 0.9846564
    },
    {
      "description": "Nose",
      "mid": "/m/0k0pj",
      "score": 0.98358303,
      "topicality": 0.98358303
    },
    {
      "description": "Head",
      "mid": "/m/04hgtk",
      "score": 0.9720427,
      "topicality": 0.9720427
    },
    {
      "description": "Chin",
      "mid": "/m/0f9swq",
      "score": 0.9677447,
      "topicality": 0.9677447
    },
    {
      "description": "Eyebrow",
      "mid": "/m/027n3_",
      "score": 0.9466718,
      "topicality": 0.9466718
    },
    {
      "description": "Facial expression",
      "mid": "/m/01k74n",
      "score": 0.9324969,
      "topicality": 0.9324969
    },
    {
      "description": "Jaw",
      "mid": "/m/01k9lj",
      "score": 0.8779433,
      "topicality": 0.8779433
    },
    {
      "description": "Dress shirt",
      "mid": "/m/06hwcd",
      "score": 0.86877877,
      "topicality": 0.86877877
    },
    {
      "description": "Organism",
      "mid": "/m/05nnm",
      "score": 0.853603,
      "topicality": 0.853603
    },
    {
      "description": "Gesture",
      "mid": "/m/0244x1",
      "score": 0.85260487,
      "topicality": 0.85260487
    },
    {
      "description": "Collar",
      "mid": "/m/091410",
      "score": 0.83872765,
      "topicality": 0.83872765
    },
    {
      "description": "Tie",
      "mid": "/m/01rkbr",
      "score": 0.83098453,
      "topicality": 0.83098453
    },
    {
      "description": "Sleeve",
      "mid": "/m/062581",
      "score": 0.8276598,
      "topicality": 0.8276598
    },
    {
      "description": "Ear",
      "mid": "/m/039xj_",
      "score": 0.8085964,
      "topicality": 0.8085964
    },
    {
      "description": "Suit",
      "mid": "/m/01xyhv",
      "score": 0.7968569,
      "topicality": 0.7968569
    },
    {
      "description": "Blazer",
      "mid": "/m/04xz_5",
      "score": 0.7826784,
      "topicality": 0.7826784
    },
    {
      "description": "Formal wear",
      "mid": "/m/02w3_2",
      "score": 0.74291706,
      "topicality": 0.74291706
    },
    {
      "description": "Wrinkle",
      "mid": "/m/02_x63",
      "score": 0.73392516,
      "topicality": 0.73392516
    },
    {
      "description": "White-collar worker",
      "mid": "/m/01kq3x",
      "score": 0.72022545,
      "topicality": 0.72022545
    },
    {
      "description": "Spokesperson",
      "mid": "/m/01xr66",
      "score": 0.7088938,
      "topicality": 0.7088938
    },
    {
      "description": "Font",
      "mid": "/m/03gq5hm",
      "score": 0.7027668,
      "topicality": 0.7027668
    },
    {
      "description": "No expression",
      "mid": "/j/9_bhpn",
      "score": 0.6985359,
      "topicality": 0.6985359
    },
    {
      "description": "Official",
      "mid": "/m/035y33",
      "score": 0.6876356,
      "topicality": 0.6876356
    },
    {
      "description": "Throat",
      "mid": "/m/0mhy4",
      "score": 0.64303124,
      "topicality": 0.64303124
    },
    {
      "description": "Event",
      "mid": "/m/081pkj",
      "score": 0.6414231,
      "topicality": 0.6414231
    },
    {
      "description": "Business",
      "mid": "/m/09s1f",
      "score": 0.57683617,
      "topicality": 0.57683617
    },
    {
      "description": "Happy",
      "mid": "/m/016pp7",
      "score": 0.57619345,
      "topicality": 0.57619345
    },
    {
      "description": "Businessperson",
      "mid": "/m/012t_z",
      "score": 0.5209405,
      "topicality": 0.5209405
    },
    {
      "description": "Portrait photography",
      "mid": "/m/0chml9",
      "score": 0.5112667,
      "topicality": 0.5112667
    },
    {
      "description": "Job",
      "mid": "/m/04115t2",
      "score": 0.50359714,
      "topicality": 0.50359714
    }
  ],
  "localizedObjectAnnotations": [
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.8046875,
            "y": 0.828125
          },
          {
            "x": 0.90625,
            "y": 0.828125
          },
          {
            "x": 0.90625,
            "y": 0.99609375
          },
          {
            "x": 0.8046875,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/01rkbr",
      "name": "Tie",
      "score": 0.9366053
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.14257813,
            "y": 0.038330078
          },
          {
            "x": 0.99609375,
            "y": 0.038330078
          },
          {
            "x": 0.99609375,
            "y": 0.99609375
          },
          {
            "x": 0.14257813,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/01g317",
      "name": "Person",
      "score": 0.92623204
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.15039063,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.99609375
          },
          {
            "x": 0.15039063,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/01xyhv",
      "name": "Suit",
      "score": 0.67373997
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.15039063,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.99609375
          },
          {
            "x": 0.15039063,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/01xygc",
      "name": "Coat",
      "score": 0.6685773
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.609375,
            "y": 0.6015625
          },
          {
            "x": 0.9765625,
            "y": 0.6015625
          },
          {
            "x": 0.9765625,
            "y": 0.99609375
          },
          {
            "x": 0.609375,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/01n4qj",
      "name": "Shirt",
      "score": 0.6236616
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.15039063,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.59765625
          },
          {
            "x": 0.99609375,
            "y": 0.99609375
          },
          {
            "x": 0.15039063,
            "y": 0.99609375
          }
        ]
      },
      "mid": "/m/047vlmn",
      "name": "Outerwear",
      "score": 0.59176666
    }
  ],
  "safeSearchAnnotation": {
    "adult": "VERY_UNLIKELY",
    "medical": "VERY_UNLIKELY",
    "racy": "VERY_UNLIKELY",
    "spoof": "LIKELY",
    "violence": "UNLIKELY"
  },
  "textAnnotations": [
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 34,
            "y": 104
          },
          {
            "x": 403,
            "y": 104
          },
          {
            "x": 403,
            "y": 399
          },
          {
            "x": 34,
            "y": 399
          }
        ]
      },
      "description": "\"Todos os dispositivos\nsofisticados e wifi do mundo\nnão vão fazer diferença se\nnão tivermos grandes\nprofessores em sala\nde aula\"\nBarack Obama",
      "locale": "pt"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 75,
            "y": 105
          },
          {
            "x": 89,
            "y": 105
          },
          {
            "x": 89,
            "y": 131
          },
          {
            "x": 75,
            "y": 131
          }
        ]
      },
      "description": "\""
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 86,
            "y": 104
          },
          {
            "x": 164,
            "y": 105
          },
          {
            "x": 164,
            "y": 132
          },
          {
            "x": 86,
            "y": 131
          }
        ]
      },
      "description": "Todos"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 173,
            "y": 105
          },
          {
            "x": 201,
            "y": 105
          },
          {
            "x": 201,
            "y": 131
          },
          {
            "x": 173,
            "y": 131
          }
        ]
      },
      "description": "os"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 209,
            "y": 105
          },
          {
            "x": 361,
            "y": 106
          },
          {
            "x": 361,
            "y": 133
          },
          {
            "x": 209,
            "y": 132
          }
        ]
      },
      "description": "dispositivos"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 34,
            "y": 149
          },
          {
            "x": 185,
            "y": 149
          },
          {
            "x": 185,
            "y": 170
          },
          {
            "x": 34,
            "y": 170
          }
        ]
      },
      "description": "sofisticados"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 193,
            "y": 149
          },
          {
            "x": 208,
            "y": 149
          },
          {
            "x": 208,
            "y": 170
          },
          {
            "x": 193,
            "y": 170
          }
        ]
      },
      "description": "e"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 215,
            "y": 149
          },
          {
            "x": 260,
            "y": 149
          },
          {
            "x": 260,
            "y": 170
          },
          {
            "x": 215,
            "y": 170
          }
        ]
      },
      "description": "wifi"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 267,
            "y": 149
          },
          {
            "x": 302,
            "y": 149
          },
          {
            "x": 302,
            "y": 170
          },
          {
            "x": 267,
            "y": 170
          }
        ]
      },
      "description": "do"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 310,
            "y": 149
          },
          {
            "x": 403,
            "y": 149
          },
          {
            "x": 403,
            "y": 170
          },
          {
            "x": 310,
            "y": 170
          }
        ]
      },
      "description": "mundo"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 52,
            "y": 189
          },
          {
            "x": 100,
            "y": 189
          },
          {
            "x": 100,
            "y": 212
          },
          {
            "x": 52,
            "y": 212
          }
        ]
      },
      "description": "não"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 106,
            "y": 189
          },
          {
            "x": 152,
            "y": 189
          },
          {
            "x": 152,
            "y": 212
          },
          {
            "x": 106,
            "y": 212
          }
        ]
      },
      "description": "vão"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 159,
            "y": 189
          },
          {
            "x": 224,
            "y": 190
          },
          {
            "x": 224,
            "y": 214
          },
          {
            "x": 159,
            "y": 213
          }
        ]
      },
      "description": "fazer"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 230,
            "y": 190
          },
          {
            "x": 350,
            "y": 191
          },
          {
            "x": 350,
            "y": 214
          },
          {
            "x": 230,
            "y": 213
          }
        ]
      },
      "description": "diferença"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 356,
            "y": 191
          },
          {
            "x": 386,
            "y": 191
          },
          {
            "x": 386,
            "y": 214
          },
          {
            "x": 356,
            "y": 214
          }
        ]
      },
      "description": "se"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 79,
            "y": 231
          },
          {
            "x": 127,
            "y": 231
          },
          {
            "x": 127,
            "y": 257
          },
          {
            "x": 79,
            "y": 257
          }
        ]
      },
      "description": "não"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 133,
            "y": 231
          },
          {
            "x": 245,
            "y": 232
          },
          {
            "x": 245,
            "y": 259
          },
          {
            "x": 133,
            "y": 258
          }
        ]
      },
      "description": "tivermos"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 253,
            "y": 232
          },
          {
            "x": 360,
            "y": 233
          },
          {
            "x": 360,
            "y": 260
          },
          {
            "x": 253,
            "y": 259
          }
        ]
      },
      "description": "grandes"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 92,
            "y": 277
          },
          {
            "x": 240,
            "y": 275
          },
          {
            "x": 240,
            "y": 301
          },
          {
            "x": 92,
            "y": 303
          }
        ]
      },
      "description": "professores"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 247,
            "y": 275
          },
          {
            "x": 286,
            "y": 274
          },
          {
            "x": 286,
            "y": 299
          },
          {
            "x": 247,
            "y": 300
          }
        ]
      },
      "description": "em"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 294,
            "y": 274
          },
          {
            "x": 345,
            "y": 273
          },
          {
            "x": 345,
            "y": 299
          },
          {
            "x": 294,
            "y": 300
          }
        ]
      },
      "description": "sala"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 165,
            "y": 319
          },
          {
            "x": 200,
            "y": 319
          },
          {
            "x": 200,
            "y": 340
          },
          {
            "x": 165,
            "y": 340
          }
        ]
      },
      "description": "de"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 207,
            "y": 319
          },
          {
            "x": 261,
            "y": 319
          },
          {
            "x": 261,
            "y": 340
          },
          {
            "x": 207,
            "y": 340
          }
        ]
      },
      "description": "aula"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 259,
            "y": 319
          },
          {
            "x": 272,
            "y": 319
          },
          {
            "x": 272,
            "y": 340
          },
          {
            "x": 259,
            "y": 340
          }
        ]
      },
      "description": "\""
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 140,
            "y": 381
          },
          {
            "x": 206,
            "y": 381
          },
          {
            "x": 206,
            "y": 398
          },
          {
            "x": 140,
            "y": 398
          }
        ]
      },
      "description": "Barack"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 211,
            "y": 381
          },
          {
            "x": 285,
            "y": 381
          },
          {
            "x": 285,
            "y": 398
          },
          {
            "x": 211,
            "y": 398
          }
        ]
      },
      "description": "Obama"
    }
  ]
}
        }
      }
    }
  ]
}
