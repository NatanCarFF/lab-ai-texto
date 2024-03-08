## Usando cloud Vision API
![Screenshot_2](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/05f5f440-4932-493a-bb59-91b11de550b7)

## Acessando a página de testes da API
![Screenshot_6](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/61775316-dc97-4727-bdc0-d768ac42d354)

## Inserindo a segunda imagem para teste:
![Screenshot_8](https://github.com/NatanCarFF/lab-ai-texto/assets/161735922/f0e7dc87-9490-48ea-9e7b-8875ac4136a7)

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
        "content": "(data from OIP (1).jpg)"
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
            {},
            {
              "x": 284
            },
            {
              "x": 284,
              "y": 354
            },
            {
              "y": 354
            }
          ]
        },
        "confidence": 0.5331619,
        "importanceFraction": 0.58622575
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 71
            },
            {
              "x": 426
            },
            {
              "x": 426,
              "y": 354
            },
            {
              "x": 71,
              "y": 354
            }
          ]
        },
        "confidence": 0.5625,
        "importanceFraction": 0.7731048
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 23
            },
            {
              "x": 450
            },
            {
              "x": 450,
              "y": 354
            },
            {
              "x": 23,
              "y": 354
            }
          ]
        },
        "confidence": 0.5625,
        "importanceFraction": 0.9277256
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
            "x": 267,
            "y": 30
          },
          {
            "x": 473,
            "y": 30
          },
          {
            "x": 473,
            "y": 323
          },
          {
            "x": 267,
            "y": 323
          }
        ]
      },
      "detectionConfidence": 0.98046875,
      "fdBoundingPoly": {
        "vertices": [
          {
            "x": 292,
            "y": 92
          },
          {
            "x": 473,
            "y": 92
          },
          {
            "x": 473,
            "y": 290
          },
          {
            "x": 292,
            "y": 290
          }
        ]
      },
      "headwearLikelihood": "VERY_UNLIKELY",
      "joyLikelihood": "VERY_UNLIKELY",
      "landmarkingConfidence": 0.31918907,
      "landmarks": [
        {
          "position": {
            "x": 362.67096,
            "y": 171.48389,
            "z": 0.00025224686
          },
          "type": "LEFT_EYE"
        },
        {
          "position": {
            "x": 434.37653,
            "y": 174.47702,
            "z": 2.6417456
          },
          "type": "RIGHT_EYE"
        },
        {
          "position": {
            "x": 337.05054,
            "y": 153.17892,
            "z": 3.9035716
          },
          "type": "LEFT_OF_LEFT_EYEBROW"
        },
        {
          "position": {
            "x": 380.8041,
            "y": 153.37459,
            "z": -16.573677
          },
          "type": "RIGHT_OF_LEFT_EYEBROW"
        },
        {
          "position": {
            "x": 417.27075,
            "y": 156.87766,
            "z": -15.219261
          },
          "type": "LEFT_OF_RIGHT_EYEBROW"
        },
        {
          "position": {
            "x": 458.26584,
            "y": 160.56241,
            "z": 8.201211
          },
          "type": "RIGHT_OF_RIGHT_EYEBROW"
        },
        {
          "position": {
            "x": 399.58246,
            "y": 172.64333,
            "z": -15.127405
          },
          "type": "MIDPOINT_BETWEEN_EYES"
        },
        {
          "position": {
            "x": 397.92313,
            "y": 226.06638,
            "z": -32.88411
          },
          "type": "NOSE_TIP"
        },
        {
          "position": {
            "x": 396.41797,
            "y": 253.51317,
            "z": -11.7784
          },
          "type": "UPPER_LIP"
        },
        {
          "position": {
            "x": 395.60837,
            "y": 278.6278,
            "z": -3.3743534
          },
          "type": "LOWER_LIP"
        },
        {
          "position": {
            "x": 364.42722,
            "y": 253.10406,
            "z": 9.081096
          },
          "type": "MOUTH_LEFT"
        },
        {
          "position": {
            "x": 431.8922,
            "y": 258.78894,
            "z": 11.451269
          },
          "type": "MOUTH_RIGHT"
        },
        {
          "position": {
            "x": 399.26987,
            "y": 262.20105,
            "z": -4.8027534
          },
          "type": "MOUTH_CENTER"
        },
        {
          "position": {
            "x": 418.43427,
            "y": 231.41187,
            "z": -2.523764
          },
          "type": "NOSE_BOTTOM_RIGHT"
        },
        {
          "position": {
            "x": 375.0233,
            "y": 228.66074,
            "z": -3.9458537
          },
          "type": "NOSE_BOTTOM_LEFT"
        },
        {
          "position": {
            "x": 397.49658,
            "y": 237.57457,
            "z": -13.920479
          },
          "type": "NOSE_BOTTOM_CENTER"
        },
        {
          "position": {
            "x": 361.31915,
            "y": 163.78645,
            "z": -5.463926
          },
          "type": "LEFT_EYE_TOP_BOUNDARY"
        },
        {
          "position": {
            "x": 378.84933,
            "y": 172.1768,
            "z": 0.5492568
          },
          "type": "LEFT_EYE_RIGHT_CORNER"
        },
        {
          "position": {
            "x": 361.87827,
            "y": 177.76797,
            "z": -0.16034365
          },
          "type": "LEFT_EYE_BOTTOM_BOUNDARY"
        },
        {
          "position": {
            "x": 347.87054,
            "y": 172.5742,
            "z": 6.6022143
          },
          "type": "LEFT_EYE_LEFT_CORNER"
        },
        {
          "position": {
            "x": 435.23306,
            "y": 167.0285,
            "z": -2.7354136
          },
          "type": "RIGHT_EYE_TOP_BOUNDARY"
        },
        {
          "position": {
            "x": 449.6174,
            "y": 175.38156,
            "z": 10.336174
          },
          "type": "RIGHT_EYE_RIGHT_CORNER"
        },
        {
          "position": {
            "x": 435.06857,
            "y": 180.76935,
            "z": 2.5491967
          },
          "type": "RIGHT_EYE_BOTTOM_BOUNDARY"
        },
        {
          "position": {
            "x": 419.46692,
            "y": 176.19748,
            "z": 2.1422677
          },
          "type": "RIGHT_EYE_LEFT_CORNER"
        },
        {
          "position": {
            "x": 358.21738,
            "y": 146.03879,
            "z": -12.090954
          },
          "type": "LEFT_EYEBROW_UPPER_MIDPOINT"
        },
        {
          "position": {
            "x": 438.51782,
            "y": 151.81479,
            "z": -9.268986
          },
          "type": "RIGHT_EYEBROW_UPPER_MIDPOINT"
        },
        {
          "position": {
            "x": 314.4015,
            "y": 196.03275,
            "z": 98.541595
          },
          "type": "LEFT_EAR_TRAGION"
        },
        {
          "position": {
            "x": 468.08075,
            "y": 196.34406,
            "z": 105.34677
          },
          "type": "RIGHT_EAR_TRAGION"
        },
        {
          "position": {
            "x": 399.4132,
            "y": 157.13336,
            "z": -18.602598
          },
          "type": "FOREHEAD_GLABELLA"
        },
        {
          "position": {
            "x": 398.0479,
            "y": 309.0561,
            "z": 11.553262
          },
          "type": "CHIN_GNATHION"
        },
        {
          "position": {
            "x": 332.51453,
            "y": 258.10376,
            "z": 74.86205
          },
          "type": "CHIN_LEFT_GONION"
        },
        {
          "position": {
            "x": 456.31555,
            "y": 259.65417,
            "z": 80.14778
          },
          "type": "CHIN_RIGHT_GONION"
        },
        {
          "position": {
            "x": 347.57263,
            "y": 223.5935,
            "z": 12.616238
          },
          "type": "LEFT_CHEEK_CENTER"
        },
        {
          "position": {
            "x": 449.20966,
            "y": 227.54492,
            "z": 16.31446
          },
          "type": "RIGHT_CHEEK_CENTER"
        }
      ],
      "panAngle": 2.0017195,
      "rollAngle": 1.4757481,
      "sorrowLikelihood": "VERY_UNLIKELY",
      "surpriseLikelihood": "VERY_UNLIKELY",
      "tiltAngle": -7.113986,
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
                  "x": 25,
                  "y": 114
                },
                {
                  "x": 278,
                  "y": 112
                },
                {
                  "x": 279,
                  "y": 254
                },
                {
                  "x": 26,
                  "y": 256
                }
              ]
            },
            "confidence": 0.9801949,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 25,
                      "y": 114
                    },
                    {
                      "x": 261,
                      "y": 113
                    },
                    {
                      "x": 261,
                      "y": 195
                    },
                    {
                      "x": 25,
                      "y": 196
                    }
                  ]
                },
                "confidence": 0.9759712,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 25,
                          "y": 114
                        },
                        {
                          "x": 123,
                          "y": 114
                        },
                        {
                          "x": 123,
                          "y": 135
                        },
                        {
                          "x": 25,
                          "y": 135
                        }
                      ]
                    },
                    "confidence": 0.9800967,
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
                              "x": 25,
                              "y": 114
                            },
                            {
                              "x": 42,
                              "y": 114
                            },
                            {
                              "x": 42,
                              "y": 135
                            },
                            {
                              "x": 25,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.95242184,
                        "text": "P"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 42,
                              "y": 114
                            },
                            {
                              "x": 55,
                              "y": 114
                            },
                            {
                              "x": 55,
                              "y": 135
                            },
                            {
                              "x": 42,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.98296565,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 56,
                              "y": 114
                            },
                            {
                              "x": 67,
                              "y": 114
                            },
                            {
                              "x": 67,
                              "y": 135
                            },
                            {
                              "x": 56,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.98788327,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 69,
                              "y": 114
                            },
                            {
                              "x": 80,
                              "y": 114
                            },
                            {
                              "x": 80,
                              "y": 135
                            },
                            {
                              "x": 69,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.98762393,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 81,
                              "y": 114
                            },
                            {
                              "x": 94,
                              "y": 114
                            },
                            {
                              "x": 94,
                              "y": 135
                            },
                            {
                              "x": 81,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9769244,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 97,
                              "y": 114
                            },
                            {
                              "x": 110,
                              "y": 114
                            },
                            {
                              "x": 110,
                              "y": 135
                            },
                            {
                              "x": 97,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9863316,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 111,
                              "y": 114
                            },
                            {
                              "x": 123,
                              "y": 114
                            },
                            {
                              "x": 123,
                              "y": 135
                            },
                            {
                              "x": 111,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9865263,
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
                          "x": 130,
                          "y": 114
                        },
                        {
                          "x": 161,
                          "y": 114
                        },
                        {
                          "x": 161,
                          "y": 135
                        },
                        {
                          "x": 130,
                          "y": 135
                        }
                      ]
                    },
                    "confidence": 0.99314725,
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
                              "x": 130,
                              "y": 114
                            },
                            {
                              "x": 145,
                              "y": 114
                            },
                            {
                              "x": 145,
                              "y": 135
                            },
                            {
                              "x": 130,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9924617,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 147,
                              "y": 114
                            },
                            {
                              "x": 161,
                              "y": 114
                            },
                            {
                              "x": 161,
                              "y": 135
                            },
                            {
                              "x": 147,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9938329,
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
                          "x": 168,
                          "y": 114
                        },
                        {
                          "x": 261,
                          "y": 114
                        },
                        {
                          "x": 261,
                          "y": 135
                        },
                        {
                          "x": 168,
                          "y": 135
                        }
                      ]
                    },
                    "confidence": 0.99241954,
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
                              "x": 168,
                              "y": 114
                            },
                            {
                              "x": 192,
                              "y": 114
                            },
                            {
                              "x": 192,
                              "y": 135
                            },
                            {
                              "x": 168,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.99370694,
                        "text": "m"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 192,
                              "y": 114
                            },
                            {
                              "x": 206,
                              "y": 114
                            },
                            {
                              "x": 206,
                              "y": 135
                            },
                            {
                              "x": 192,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.99380565,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 208,
                              "y": 114
                            },
                            {
                              "x": 224,
                              "y": 114
                            },
                            {
                              "x": 224,
                              "y": 135
                            },
                            {
                              "x": 208,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9949794,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 224,
                              "y": 114
                            },
                            {
                              "x": 236,
                              "y": 114
                            },
                            {
                              "x": 236,
                              "y": 135
                            },
                            {
                              "x": 224,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.99189025,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 234,
                              "y": 114
                            },
                            {
                              "x": 249,
                              "y": 114
                            },
                            {
                              "x": 249,
                              "y": 135
                            },
                            {
                              "x": 234,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.99172515,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 248,
                              "y": 114
                            },
                            {
                              "x": 261,
                              "y": 114
                            },
                            {
                              "x": 261,
                              "y": 135
                            },
                            {
                              "x": 248,
                              "y": 135
                            }
                          ]
                        },
                        "confidence": 0.9884099,
                        "property": {
                          "detectedBreak": {
                            "type": "EOL_SURE_SPACE"
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
                          "x": 27,
                          "y": 144
                        },
                        {
                          "x": 157,
                          "y": 144
                        },
                        {
                          "x": 157,
                          "y": 164
                        },
                        {
                          "x": 27,
                          "y": 164
                        }
                      ]
                    },
                    "confidence": 0.99167544,
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
                              "x": 27,
                              "y": 144
                            },
                            {
                              "x": 41,
                              "y": 144
                            },
                            {
                              "x": 41,
                              "y": 164
                            },
                            {
                              "x": 27,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.98810613,
                        "text": "b"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 44,
                              "y": 144
                            },
                            {
                              "x": 55,
                              "y": 144
                            },
                            {
                              "x": 55,
                              "y": 164
                            },
                            {
                              "x": 44,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.9781768,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 56,
                              "y": 144
                            },
                            {
                              "x": 62,
                              "y": 144
                            },
                            {
                              "x": 62,
                              "y": 164
                            },
                            {
                              "x": 56,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.9909244,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 64,
                              "y": 144
                            },
                            {
                              "x": 71,
                              "y": 144
                            },
                            {
                              "x": 71,
                              "y": 164
                            },
                            {
                              "x": 64,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.9908052,
                        "text": "l"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 73,
                              "y": 144
                            },
                            {
                              "x": 88,
                              "y": 144
                            },
                            {
                              "x": 88,
                              "y": 164
                            },
                            {
                              "x": 73,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.9943887,
                        "text": "h"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 90,
                              "y": 144
                            },
                            {
                              "x": 103,
                              "y": 144
                            },
                            {
                              "x": 103,
                              "y": 164
                            },
                            {
                              "x": 90,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.992489,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 105,
                              "y": 144
                            },
                            {
                              "x": 119,
                              "y": 144
                            },
                            {
                              "x": 119,
                              "y": 164
                            },
                            {
                              "x": 105,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.99533653,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 122,
                              "y": 144
                            },
                            {
                              "x": 131,
                              "y": 144
                            },
                            {
                              "x": 131,
                              "y": 164
                            },
                            {
                              "x": 122,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.99625623,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 131,
                              "y": 144
                            },
                            {
                              "x": 143,
                              "y": 144
                            },
                            {
                              "x": 143,
                              "y": 164
                            },
                            {
                              "x": 131,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.99721366,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 146,
                              "y": 144
                            },
                            {
                              "x": 157,
                              "y": 144
                            },
                            {
                              "x": 157,
                              "y": 164
                            },
                            {
                              "x": 146,
                              "y": 164
                            }
                          ]
                        },
                        "confidence": 0.9930578,
                        "property": {
                          "detectedBreak": {
                            "type": "EOL_SURE_SPACE"
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
                          "x": 27,
                          "y": 175
                        },
                        {
                          "x": 182,
                          "y": 174
                        },
                        {
                          "x": 182,
                          "y": 195
                        },
                        {
                          "x": 27,
                          "y": 196
                        }
                      ]
                    },
                    "confidence": 0.94697464,
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
                              "x": 27,
                              "y": 176
                            },
                            {
                              "x": 41,
                              "y": 176
                            },
                            {
                              "x": 41,
                              "y": 196
                            },
                            {
                              "x": 27,
                              "y": 196
                            }
                          ]
                        },
                        "confidence": 0.97297096,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 39,
                              "y": 175
                            },
                            {
                              "x": 56,
                              "y": 175
                            },
                            {
                              "x": 56,
                              "y": 195
                            },
                            {
                              "x": 39,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.9587426,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 57,
                              "y": 175
                            },
                            {
                              "x": 70,
                              "y": 175
                            },
                            {
                              "x": 70,
                              "y": 195
                            },
                            {
                              "x": 57,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.96257657,
                        "text": "c"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 71,
                              "y": 175
                            },
                            {
                              "x": 85,
                              "y": 175
                            },
                            {
                              "x": 85,
                              "y": 195
                            },
                            {
                              "x": 71,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.9659662,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 86,
                              "y": 175
                            },
                            {
                              "x": 102,
                              "y": 175
                            },
                            {
                              "x": 102,
                              "y": 195
                            },
                            {
                              "x": 86,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.96961427,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 102,
                              "y": 175
                            },
                            {
                              "x": 113,
                              "y": 175
                            },
                            {
                              "x": 113,
                              "y": 195
                            },
                            {
                              "x": 102,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.98635143,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 112,
                              "y": 175
                            },
                            {
                              "x": 125,
                              "y": 175
                            },
                            {
                              "x": 125,
                              "y": 195
                            },
                            {
                              "x": 112,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.967633,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 125,
                              "y": 175
                            },
                            {
                              "x": 140,
                              "y": 175
                            },
                            {
                              "x": 140,
                              "y": 195
                            },
                            {
                              "x": 125,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.9522153,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 139,
                              "y": 175
                            },
                            {
                              "x": 152,
                              "y": 175
                            },
                            {
                              "x": 152,
                              "y": 195
                            },
                            {
                              "x": 139,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.8708313,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 152,
                              "y": 175
                            },
                            {
                              "x": 165,
                              "y": 175
                            },
                            {
                              "x": 165,
                              "y": 195
                            },
                            {
                              "x": 152,
                              "y": 195
                            }
                          ]
                        },
                        "confidence": 0.844329,
                        "text": "ã"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 167,
                              "y": 174
                            },
                            {
                              "x": 182,
                              "y": 174
                            },
                            {
                              "x": 182,
                              "y": 194
                            },
                            {
                              "x": 167,
                              "y": 194
                            }
                          ]
                        },
                        "confidence": 0.96549016,
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
                      "x": 26,
                      "y": 203
                    },
                    {
                      "x": 196,
                      "y": 202
                    },
                    {
                      "x": 196,
                      "y": 229
                    },
                    {
                      "x": 26,
                      "y": 230
                    }
                  ]
                },
                "confidence": 0.98749536,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 26,
                          "y": 203
                        },
                        {
                          "x": 158,
                          "y": 202
                        },
                        {
                          "x": 158,
                          "y": 229
                        },
                        {
                          "x": 26,
                          "y": 230
                        }
                      ]
                    },
                    "confidence": 0.98701626,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "es"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 26,
                              "y": 204
                            },
                            {
                              "x": 42,
                              "y": 204
                            },
                            {
                              "x": 42,
                              "y": 230
                            },
                            {
                              "x": 26,
                              "y": 230
                            }
                          ]
                        },
                        "confidence": 0.97568554,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 39,
                              "y": 203
                            },
                            {
                              "x": 56,
                              "y": 203
                            },
                            {
                              "x": 56,
                              "y": 229
                            },
                            {
                              "x": 39,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9770867,
                        "text": "p"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 58,
                              "y": 203
                            },
                            {
                              "x": 73,
                              "y": 203
                            },
                            {
                              "x": 73,
                              "y": 229
                            },
                            {
                              "x": 58,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9748852,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 72,
                              "y": 203
                            },
                            {
                              "x": 85,
                              "y": 203
                            },
                            {
                              "x": 85,
                              "y": 229
                            },
                            {
                              "x": 72,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9885668,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 84,
                              "y": 203
                            },
                            {
                              "x": 92,
                              "y": 203
                            },
                            {
                              "x": 92,
                              "y": 229
                            },
                            {
                              "x": 84,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.98816687,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 93,
                              "y": 203
                            },
                            {
                              "x": 105,
                              "y": 203
                            },
                            {
                              "x": 105,
                              "y": 229
                            },
                            {
                              "x": 93,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9955925,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 102,
                              "y": 203
                            },
                            {
                              "x": 118,
                              "y": 203
                            },
                            {
                              "x": 118,
                              "y": 229
                            },
                            {
                              "x": 102,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.994762,
                        "text": "o"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 117,
                              "y": 203
                            },
                            {
                              "x": 130,
                              "y": 203
                            },
                            {
                              "x": 130,
                              "y": 229
                            },
                            {
                              "x": 117,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.9938188,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 130,
                              "y": 203
                            },
                            {
                              "x": 145,
                              "y": 203
                            },
                            {
                              "x": 145,
                              "y": 229
                            },
                            {
                              "x": 130,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.99142724,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 144,
                              "y": 203
                            },
                            {
                              "x": 158,
                              "y": 203
                            },
                            {
                              "x": 158,
                              "y": 229
                            },
                            {
                              "x": 144,
                              "y": 229
                            }
                          ]
                        },
                        "confidence": 0.99017084,
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
                          "x": 163,
                          "y": 202
                        },
                        {
                          "x": 196,
                          "y": 202
                        },
                        {
                          "x": 196,
                          "y": 228
                        },
                        {
                          "x": 163,
                          "y": 228
                        }
                      ]
                    },
                    "confidence": 0.98989093,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "es"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 163,
                              "y": 202
                            },
                            {
                              "x": 180,
                              "y": 202
                            },
                            {
                              "x": 180,
                              "y": 228
                            },
                            {
                              "x": 163,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.9901671,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 180,
                              "y": 202
                            },
                            {
                              "x": 196,
                              "y": 202
                            },
                            {
                              "x": 196,
                              "y": 228
                            },
                            {
                              "x": 180,
                              "y": 228
                            }
                          ]
                        },
                        "confidence": 0.9896147,
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
                      "x": 27,
                      "y": 235
                    },
                    {
                      "x": 279,
                      "y": 232
                    },
                    {
                      "x": 279,
                      "y": 253
                    },
                    {
                      "x": 27,
                      "y": 256
                    }
                  ]
                },
                "confidence": 0.9837753,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 27,
                          "y": 235
                        },
                        {
                          "x": 118,
                          "y": 234
                        },
                        {
                          "x": 118,
                          "y": 255
                        },
                        {
                          "x": 27,
                          "y": 256
                        }
                      ]
                    },
                    "confidence": 0.98922557,
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
                              "x": 27,
                              "y": 236
                            },
                            {
                              "x": 50,
                              "y": 236
                            },
                            {
                              "x": 50,
                              "y": 256
                            },
                            {
                              "x": 27,
                              "y": 256
                            }
                          ]
                        },
                        "confidence": 0.9855372,
                        "text": "m"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 50,
                              "y": 235
                            },
                            {
                              "x": 63,
                              "y": 235
                            },
                            {
                              "x": 63,
                              "y": 255
                            },
                            {
                              "x": 50,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.99369705,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 65,
                              "y": 235
                            },
                            {
                              "x": 80,
                              "y": 235
                            },
                            {
                              "x": 80,
                              "y": 255
                            },
                            {
                              "x": 65,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.99194896,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 81,
                              "y": 235
                            },
                            {
                              "x": 91,
                              "y": 235
                            },
                            {
                              "x": 91,
                              "y": 255
                            },
                            {
                              "x": 81,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.99028003,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 91,
                              "y": 235
                            },
                            {
                              "x": 104,
                              "y": 235
                            },
                            {
                              "x": 104,
                              "y": 255
                            },
                            {
                              "x": 91,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.98320997,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 106,
                              "y": 235
                            },
                            {
                              "x": 118,
                              "y": 235
                            },
                            {
                              "x": 118,
                              "y": 255
                            },
                            {
                              "x": 106,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.99068034,
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
                          "x": 125,
                          "y": 234
                        },
                        {
                          "x": 272,
                          "y": 233
                        },
                        {
                          "x": 272,
                          "y": 254
                        },
                        {
                          "x": 125,
                          "y": 255
                        }
                      ]
                    },
                    "confidence": 0.9892488,
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
                              "x": 125,
                              "y": 235
                            },
                            {
                              "x": 137,
                              "y": 235
                            },
                            {
                              "x": 137,
                              "y": 255
                            },
                            {
                              "x": 125,
                              "y": 255
                            }
                          ]
                        },
                        "confidence": 0.9916033,
                        "text": "f"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 135,
                              "y": 234
                            },
                            {
                              "x": 147,
                              "y": 234
                            },
                            {
                              "x": 147,
                              "y": 254
                            },
                            {
                              "x": 135,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.9946066,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 147,
                              "y": 234
                            },
                            {
                              "x": 161,
                              "y": 234
                            },
                            {
                              "x": 161,
                              "y": 254
                            },
                            {
                              "x": 147,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.992903,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 162,
                              "y": 234
                            },
                            {
                              "x": 174,
                              "y": 234
                            },
                            {
                              "x": 174,
                              "y": 254
                            },
                            {
                              "x": 162,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.99429655,
                        "text": "c"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 175,
                              "y": 234
                            },
                            {
                              "x": 189,
                              "y": 234
                            },
                            {
                              "x": 189,
                              "y": 254
                            },
                            {
                              "x": 175,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.9880945,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 189,
                              "y": 234
                            },
                            {
                              "x": 201,
                              "y": 234
                            },
                            {
                              "x": 201,
                              "y": 254
                            },
                            {
                              "x": 189,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.9912603,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 202,
                              "y": 234
                            },
                            {
                              "x": 214,
                              "y": 234
                            },
                            {
                              "x": 214,
                              "y": 254
                            },
                            {
                              "x": 202,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.9911647,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 214,
                              "y": 234
                            },
                            {
                              "x": 228,
                              "y": 234
                            },
                            {
                              "x": 228,
                              "y": 254
                            },
                            {
                              "x": 214,
                              "y": 254
                            }
                          ]
                        },
                        "confidence": 0.9941368,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 229,
                              "y": 233
                            },
                            {
                              "x": 244,
                              "y": 233
                            },
                            {
                              "x": 244,
                              "y": 253
                            },
                            {
                              "x": 229,
                              "y": 253
                            }
                          ]
                        },
                        "confidence": 0.9937726,
                        "text": "d"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 245,
                              "y": 233
                            },
                            {
                              "x": 260,
                              "y": 233
                            },
                            {
                              "x": 260,
                              "y": 253
                            },
                            {
                              "x": 245,
                              "y": 253
                            }
                          ]
                        },
                        "confidence": 0.98354995,
                        "text": "a"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 259,
                              "y": 233
                            },
                            {
                              "x": 272,
                              "y": 233
                            },
                            {
                              "x": 272,
                              "y": 253
                            },
                            {
                              "x": 259,
                              "y": 253
                            }
                          ]
                        },
                        "confidence": 0.9663485,
                        "text": "s"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 272,
                          "y": 233
                        },
                        {
                          "x": 279,
                          "y": 233
                        },
                        {
                          "x": 279,
                          "y": 253
                        },
                        {
                          "x": 272,
                          "y": 253
                        }
                      ]
                    },
                    "confidence": 0.8908658,
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
                              "x": 272,
                              "y": 233
                            },
                            {
                              "x": 279,
                              "y": 233
                            },
                            {
                              "x": 279,
                              "y": 253
                            },
                            {
                              "x": 272,
                              "y": 253
                            }
                          ]
                        },
                        "confidence": 0.8908658,
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
              }
            ]
          },
          {
            "blockType": "TEXT",
            "boundingBox": {
              "vertices": [
                {
                  "x": 14,
                  "y": 329
                },
                {
                  "x": 82,
                  "y": 329
                },
                {
                  "x": 82,
                  "y": 337
                },
                {
                  "x": 14,
                  "y": 337
                }
              ]
            },
            "confidence": 0.9919463,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 14,
                      "y": 329
                    },
                    {
                      "x": 82,
                      "y": 329
                    },
                    {
                      "x": 82,
                      "y": 337
                    },
                    {
                      "x": 14,
                      "y": 337
                    }
                  ]
                },
                "confidence": 0.9919463,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 14,
                          "y": 329
                        },
                        {
                          "x": 43,
                          "y": 329
                        },
                        {
                          "x": 43,
                          "y": 337
                        },
                        {
                          "x": 14,
                          "y": 337
                        }
                      ]
                    },
                    "confidence": 0.9878979,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "en"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 14,
                              "y": 329
                            },
                            {
                              "x": 21,
                              "y": 329
                            },
                            {
                              "x": 21,
                              "y": 337
                            },
                            {
                              "x": 14,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.9876892,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 20,
                              "y": 329
                            },
                            {
                              "x": 24,
                              "y": 329
                            },
                            {
                              "x": 24,
                              "y": 337
                            },
                            {
                              "x": 20,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.98293626,
                        "text": "l"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 24,
                              "y": 329
                            },
                            {
                              "x": 30,
                              "y": 329
                            },
                            {
                              "x": 30,
                              "y": 337
                            },
                            {
                              "x": 24,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99301976,
                        "text": "b"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 30,
                              "y": 329
                            },
                            {
                              "x": 35,
                              "y": 329
                            },
                            {
                              "x": 35,
                              "y": 337
                            },
                            {
                              "x": 30,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.9935734,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 34,
                              "y": 329
                            },
                            {
                              "x": 39,
                              "y": 329
                            },
                            {
                              "x": 39,
                              "y": 337
                            },
                            {
                              "x": 34,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.98503995,
                        "text": "r"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 38,
                              "y": 329
                            },
                            {
                              "x": 43,
                              "y": 329
                            },
                            {
                              "x": 43,
                              "y": 337
                            },
                            {
                              "x": 38,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.98512846,
                        "property": {
                          "detectedBreak": {
                            "type": "SPACE"
                          }
                        },
                        "text": "t"
                      }
                    ]
                  },
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 44,
                          "y": 329
                        },
                        {
                          "x": 82,
                          "y": 329
                        },
                        {
                          "x": 82,
                          "y": 337
                        },
                        {
                          "x": 44,
                          "y": 337
                        }
                      ]
                    },
                    "confidence": 0.9949826,
                    "property": {
                      "detectedLanguages": [
                        {
                          "confidence": 1,
                          "languageCode": "en"
                        }
                      ]
                    },
                    "symbols": [
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 44,
                              "y": 329
                            },
                            {
                              "x": 50,
                              "y": 329
                            },
                            {
                              "x": 50,
                              "y": 337
                            },
                            {
                              "x": 44,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.9936143,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 51,
                              "y": 329
                            },
                            {
                              "x": 54,
                              "y": 329
                            },
                            {
                              "x": 54,
                              "y": 337
                            },
                            {
                              "x": 51,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99438816,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 54,
                              "y": 329
                            },
                            {
                              "x": 60,
                              "y": 329
                            },
                            {
                              "x": 60,
                              "y": 337
                            },
                            {
                              "x": 54,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.9957594,
                        "text": "n"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 60,
                              "y": 329
                            },
                            {
                              "x": 64,
                              "y": 329
                            },
                            {
                              "x": 64,
                              "y": 337
                            },
                            {
                              "x": 60,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99570686,
                        "text": "s"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 64,
                              "y": 329
                            },
                            {
                              "x": 68,
                              "y": 329
                            },
                            {
                              "x": 68,
                              "y": 337
                            },
                            {
                              "x": 64,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.9960023,
                        "text": "t"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 68,
                              "y": 329
                            },
                            {
                              "x": 73,
                              "y": 329
                            },
                            {
                              "x": 73,
                              "y": 337
                            },
                            {
                              "x": 68,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99518263,
                        "text": "e"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 73,
                              "y": 329
                            },
                            {
                              "x": 76,
                              "y": 329
                            },
                            {
                              "x": 76,
                              "y": 337
                            },
                            {
                              "x": 73,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99595535,
                        "text": "i"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 76,
                              "y": 329
                            },
                            {
                              "x": 82,
                              "y": 329
                            },
                            {
                              "x": 82,
                              "y": 337
                            },
                            {
                              "x": 76,
                              "y": 337
                            }
                          ]
                        },
                        "confidence": 0.99325186,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "n"
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
                  "x": 227,
                  "y": 329
                },
                {
                  "x": 282,
                  "y": 329
                },
                {
                  "x": 282,
                  "y": 336
                },
                {
                  "x": 227,
                  "y": 336
                }
              ]
            },
            "confidence": 0.98918164,
            "paragraphs": [
              {
                "boundingBox": {
                  "vertices": [
                    {
                      "x": 227,
                      "y": 329
                    },
                    {
                      "x": 282,
                      "y": 329
                    },
                    {
                      "x": 282,
                      "y": 336
                    },
                    {
                      "x": 227,
                      "y": 336
                    }
                  ]
                },
                "confidence": 0.98918164,
                "words": [
                  {
                    "boundingBox": {
                      "vertices": [
                        {
                          "x": 227,
                          "y": 329
                        },
                        {
                          "x": 282,
                          "y": 329
                        },
                        {
                          "x": 282,
                          "y": 336
                        },
                        {
                          "x": 227,
                          "y": 336
                        }
                      ]
                    },
                    "confidence": 0.98918164,
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
                              "y": 329
                            },
                            {
                              "x": 234,
                              "y": 329
                            },
                            {
                              "x": 234,
                              "y": 336
                            },
                            {
                              "x": 227,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.97179633,
                        "text": "P"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 234,
                              "y": 329
                            },
                            {
                              "x": 240,
                              "y": 329
                            },
                            {
                              "x": 240,
                              "y": 336
                            },
                            {
                              "x": 234,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.98332286,
                        "text": "E"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 241,
                              "y": 329
                            },
                            {
                              "x": 247,
                              "y": 329
                            },
                            {
                              "x": 247,
                              "y": 336
                            },
                            {
                              "x": 241,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.9931626,
                        "text": "N"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 248,
                              "y": 329
                            },
                            {
                              "x": 254,
                              "y": 329
                            },
                            {
                              "x": 254,
                              "y": 336
                            },
                            {
                              "x": 248,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.9947672,
                        "text": "S"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 253,
                              "y": 329
                            },
                            {
                              "x": 260,
                              "y": 329
                            },
                            {
                              "x": 260,
                              "y": 336
                            },
                            {
                              "x": 253,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.9953936,
                        "text": "A"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 260,
                              "y": 329
                            },
                            {
                              "x": 266,
                              "y": 329
                            },
                            {
                              "x": 266,
                              "y": 336
                            },
                            {
                              "x": 260,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.9948764,
                        "text": "D"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 267,
                              "y": 329
                            },
                            {
                              "x": 274,
                              "y": 329
                            },
                            {
                              "x": 274,
                              "y": 336
                            },
                            {
                              "x": 267,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.99426776,
                        "text": "O"
                      },
                      {
                        "boundingBox": {
                          "vertices": [
                            {
                              "x": 275,
                              "y": 329
                            },
                            {
                              "x": 282,
                              "y": 329
                            },
                            {
                              "x": 282,
                              "y": 336
                            },
                            {
                              "x": 275,
                              "y": 336
                            }
                          ]
                        },
                        "confidence": 0.98586637,
                        "property": {
                          "detectedBreak": {
                            "type": "LINE_BREAK"
                          }
                        },
                        "text": "R"
                      }
                    ]
                  }
                ]
              }
            ]
          }
        ],
        "confidence": 0.9871076,
        "height": 355,
        "property": {
          "detectedLanguages": [
            {
              "confidence": 0.70243806,
              "languageCode": "pt"
            },
            {
              "confidence": 0.16055816,
              "languageCode": "en"
            },
            {
              "confidence": 0.13700376,
              "languageCode": "es"
            }
          ]
        },
        "width": 474
      }
    ],
    "text": "Pessoas de mentes\nbrilhantes\nencontrarão\nopositores de\nmentes fracassadas.\nAlbert Einstein\nPENSADOR"
  },
  "imagePropertiesAnnotation": {
    "cropHints": [
      {
        "boundingPoly": {
          "vertices": [
            {},
            {
              "x": 284
            },
            {
              "x": 284,
              "y": 354
            },
            {
              "y": 354
            }
          ]
        },
        "confidence": 0.5331619,
        "importanceFraction": 0.58622575
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 71
            },
            {
              "x": 426
            },
            {
              "x": 426,
              "y": 354
            },
            {
              "x": 71,
              "y": 354
            }
          ]
        },
        "confidence": 0.5625,
        "importanceFraction": 0.7731048
      },
      {
        "boundingPoly": {
          "vertices": [
            {
              "x": 23
            },
            {
              "x": 450
            },
            {
              "x": 450,
              "y": 354
            },
            {
              "x": 23,
              "y": 354
            }
          ]
        },
        "confidence": 0.5625,
        "importanceFraction": 0.9277256
      }
    ],
    "dominantColors": {
      "colors": [
        {
          "color": {
            "blue": 249,
            "green": 249,
            "red": 249
          },
          "hex": "F9F9F9",
          "percent": 41.2022892171565,
          "percentRounded": 41,
          "pixelFraction": 0.4046192,
          "rgb": "249, 249,\n 249",
          "score": 0.4120229
        },
        {
          "color": {
            "blue": 79,
            "green": 79,
            "red": 79
          },
          "hex": "4F4F4F",
          "percent": 21.751823586715346,
          "percentRounded": 22,
          "pixelFraction": 0.22592504,
          "rgb": "79, 79,\n 79",
          "score": 0.21751824
        },
        {
          "color": {
            "blue": 9,
            "green": 9,
            "red": 9
          },
          "hex": "090909",
          "percent": 13.498459743529262,
          "percentRounded": 13,
          "pixelFraction": 0.13234237,
          "rgb": "9, 9,\n 9",
          "score": 0.1349846
        },
        {
          "color": {
            "blue": 196,
            "green": 196,
            "red": 196
          },
          "hex": "C4C4C4",
          "percent": 7.643126854780588,
          "percentRounded": 8,
          "pixelFraction": 0.0771198,
          "rgb": "196, 196,\n 196",
          "score": 0.07643127
        },
        {
          "color": {
            "blue": 120,
            "green": 120,
            "red": 120
          },
          "hex": "787878",
          "percent": 6.535023375834554,
          "percentRounded": 7,
          "pixelFraction": 0.065771595,
          "rgb": "120, 120,\n 120",
          "score": 0.065350235
        },
        {
          "color": {
            "blue": 156,
            "green": 156,
            "red": 156
          },
          "hex": "9C9C9C",
          "percent": 5.383968297704601,
          "percentRounded": 5,
          "pixelFraction": 0.0544234,
          "rgb": "156, 156,\n 156",
          "score": 0.053839684
        },
        {
          "color": {
            "blue": 54,
            "green": 54,
            "red": 54
          },
          "hex": "363636",
          "percent": 3.9853089242791295,
          "percentRounded": 4,
          "pixelFraction": 0.03979861,
          "rgb": "54, 54,\n 54",
          "score": 0.03985309
        }
      ]
    }
  },
  "labelAnnotations": [
    {
      "description": "Nose",
      "mid": "/m/0k0pj",
      "score": 0.98358303,
      "topicality": 0.98358303
    },
    {
      "description": "Jaw",
      "mid": "/m/01k9lj",
      "score": 0.879953,
      "topicality": 0.879953
    },
    {
      "description": "Physicist",
      "mid": "/m/05snw",
      "score": 0.86131215,
      "topicality": 0.86131215
    },
    {
      "description": "Organism",
      "mid": "/m/05nnm",
      "score": 0.85207516,
      "topicality": 0.85207516
    },
    {
      "description": "Ear",
      "mid": "/m/039xj_",
      "score": 0.8203277,
      "topicality": 0.8203277
    },
    {
      "description": "Wrinkle",
      "mid": "/m/02_x63",
      "score": 0.7986288,
      "topicality": 0.7986288
    },
    {
      "description": "Adaptation",
      "mid": "/m/03r_vp",
      "score": 0.7920562,
      "topicality": 0.7920562
    },
    {
      "description": "Font",
      "mid": "/m/03gq5hm",
      "score": 0.7697395,
      "topicality": 0.7697395
    },
    {
      "description": "Photo caption",
      "mid": "/m/0b75wg4",
      "score": 0.6700615,
      "topicality": 0.6700615
    },
    {
      "description": "Moustache",
      "mid": "/m/0bby24z",
      "score": 0.6003817,
      "topicality": 0.6003817
    },
    {
      "description": "Portrait photography",
      "mid": "/m/0chml9",
      "score": 0.56737226,
      "topicality": 0.56737226
    },
    {
      "description": "History",
      "mid": "/m/03g3w",
      "score": 0.56377286,
      "topicality": 0.56377286
    },
    {
      "description": "Facial hair",
      "mid": "/m/0ds5b",
      "score": 0.56143486,
      "topicality": 0.56143486
    },
    {
      "description": "Portrait",
      "mid": "/m/01dv4h",
      "score": 0.5507329,
      "topicality": 0.5507329
    },
    {
      "description": "Brand",
      "mid": "/m/01cd9",
      "score": 0.52599657,
      "topicality": 0.52599657
    },
    {
      "description": "Elder",
      "mid": "/m/027v9wk",
      "score": 0.5182243,
      "topicality": 0.5182243
    },
    {
      "description": "Happy",
      "mid": "/m/016pp7",
      "score": 0.5019729,
      "topicality": 0.5019729
    }
  ],
  "localizedObjectAnnotations": [
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.58984375,
            "y": 0.01965332
          },
          {
            "x": 0.99609375,
            "y": 0.01965332
          },
          {
            "x": 0.99609375,
            "y": 1
          },
          {
            "x": 0.58984375,
            "y": 1
          }
        ]
      },
      "mid": "/m/01g317",
      "name": "Person",
      "score": 0.8483652
    },
    {
      "boundingPoly": {
        "normalizedVertices": [
          {
            "x": 0.61328125,
            "y": 0.6640625
          },
          {
            "x": 0.99609375,
            "y": 0.6640625
          },
          {
            "x": 0.99609375,
            "y": 0.98828125
          },
          {
            "x": 0.61328125,
            "y": 0.98828125
          }
        ]
      },
      "mid": "/m/09j2d",
      "name": "Clothing",
      "score": 0.5340344
    }
  ],
  "safeSearchAnnotation": {
    "adult": "VERY_UNLIKELY",
    "medical": "UNLIKELY",
    "racy": "VERY_UNLIKELY",
    "spoof": "LIKELY",
    "violence": "UNLIKELY"
  },
  "textAnnotations": [
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 14,
            "y": 112
          },
          {
            "x": 282,
            "y": 112
          },
          {
            "x": 282,
            "y": 337
          },
          {
            "x": 14,
            "y": 337
          }
        ]
      },
      "description": "Pessoas de mentes\nbrilhantes\nencontrarão\nopositores de\nmentes fracassadas.\nAlbert Einstein\nPENSADOR",
      "locale": "pt"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 25,
            "y": 114
          },
          {
            "x": 123,
            "y": 114
          },
          {
            "x": 123,
            "y": 135
          },
          {
            "x": 25,
            "y": 135
          }
        ]
      },
      "description": "Pessoas"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 130,
            "y": 114
          },
          {
            "x": 161,
            "y": 114
          },
          {
            "x": 161,
            "y": 135
          },
          {
            "x": 130,
            "y": 135
          }
        ]
      },
      "description": "de"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 168,
            "y": 114
          },
          {
            "x": 261,
            "y": 114
          },
          {
            "x": 261,
            "y": 135
          },
          {
            "x": 168,
            "y": 135
          }
        ]
      },
      "description": "mentes"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 27,
            "y": 144
          },
          {
            "x": 157,
            "y": 144
          },
          {
            "x": 157,
            "y": 164
          },
          {
            "x": 27,
            "y": 164
          }
        ]
      },
      "description": "brilhantes"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 27,
            "y": 175
          },
          {
            "x": 182,
            "y": 174
          },
          {
            "x": 182,
            "y": 195
          },
          {
            "x": 27,
            "y": 196
          }
        ]
      },
      "description": "encontrarão"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 26,
            "y": 203
          },
          {
            "x": 158,
            "y": 202
          },
          {
            "x": 158,
            "y": 229
          },
          {
            "x": 26,
            "y": 230
          }
        ]
      },
      "description": "opositores"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 163,
            "y": 202
          },
          {
            "x": 196,
            "y": 202
          },
          {
            "x": 196,
            "y": 228
          },
          {
            "x": 163,
            "y": 228
          }
        ]
      },
      "description": "de"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 27,
            "y": 235
          },
          {
            "x": 118,
            "y": 234
          },
          {
            "x": 118,
            "y": 255
          },
          {
            "x": 27,
            "y": 256
          }
        ]
      },
      "description": "mentes"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 125,
            "y": 234
          },
          {
            "x": 272,
            "y": 233
          },
          {
            "x": 272,
            "y": 254
          },
          {
            "x": 125,
            "y": 255
          }
        ]
      },
      "description": "fracassadas"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 272,
            "y": 233
          },
          {
            "x": 279,
            "y": 233
          },
          {
            "x": 279,
            "y": 253
          },
          {
            "x": 272,
            "y": 253
          }
        ]
      },
      "description": "."
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 14,
            "y": 329
          },
          {
            "x": 43,
            "y": 329
          },
          {
            "x": 43,
            "y": 337
          },
          {
            "x": 14,
            "y": 337
          }
        ]
      },
      "description": "Albert"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 44,
            "y": 329
          },
          {
            "x": 82,
            "y": 329
          },
          {
            "x": 82,
            "y": 337
          },
          {
            "x": 44,
            "y": 337
          }
        ]
      },
      "description": "Einstein"
    },
    {
      "boundingPoly": {
        "vertices": [
          {
            "x": 227,
            "y": 329
          },
          {
            "x": 282,
            "y": 329
          },
          {
            "x": 282,
            "y": 336
          },
          {
            "x": 227,
            "y": 336
          }
        ]
      },
      "description": "PENSADOR"
    }
  ]
}
