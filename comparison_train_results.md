# Comparison of my training results with official results
## Dex-YCB results

| checkpoints     | MPJPE    | PA-MPJPE  | object(ADD-10) |
|---------|---------|----------|----------------|
| 40 epoch    | 12.697  | 5.473    | 0.2938       |
| official | 12.557  | 5.483    | 0.3039      |

| checkpoints       | object1     | object2     | object3     | object4     | object5     | object6     | object7     | object8     | object9     | object10    | object11    | object12    | object13    | object14    | object15    | object16    | object17    | object18    | object19    | object20    | object21    | simple average     |
|--------------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|
| 40 epoch         | 0.2458  | 0.6793  | 0.3698  | 0.1113  | 0.4948  | 0.0849  | 0.3066  | 0.2454  | 0.2008  | 0.1828  | 0.3818  | 0.3935  | 0.3174  | 0.1582  | 0.4032  | 0.4140  | 0.1709  | 0.0177  |         | 0.4174  | 0.2801  | 0.2938  |
| official   | 0.2385  | 0.6729  | 0.354   | 0.1262  | 0.4824  | 0.0936  | 0.3136  | 0.2675  | 0.2133  | 0.1731  | 0.3735  | 0.4212  | 0.3711  | 0.1709  | 0.4538  | 0.4585  | 0.1377  | 0.0333  |         | 0.4459  | 0.2777  | 0.3039  |

## HO3D results

| checkpoints      | 3D KP AUC | 3D KP Mean Distance | 3D KP PROCRUSTES ALIGNED AUC | 3D KP PROCRUSTES ALIGNED Mean Distance | 3D KP SCALE-TRANSLATION ALIGNED AUC | 3D KP SCALE-TRANSLATION ALIGNED Mean Distance | 3D MESH AUC | 3D MESH Mean Distance | 3D MESH ALIGNED AUC | 3D MESH ALIGNED Mean Distance | F@5.0mm | F_aligned@5.0mm | F@15.0mm | F_aligned@15.0mm |
|-----------------|-----------|---------------------|-------------------------------|---------------------------------------|-----------------------------------------|-------------------------------------------------|-------------|---------------------|---------------------|-----------------------------------------|---------|-----------------|----------|------------------|
| 70 epoch  | 0.488     | 2.92 cm             | 0.814                         | 0.93 cm                               | 0.500                                   | 2.86 cm                                       | 0.501       | 2.82 cm             | 0.817               | 0.92 cm                                 | 0.232   | 0.550           | 0.683    | 0.961            |
| official  | 0.486     | 2.90 cm             | 0.822                         | 0.89 cm                               | 0.497                                   | 2.84 cm                                       | 0.499       | 2.80 cm             | 0.825               | 0.87 cm                                 | 0.231   | 0.575           | 0.688    | 0.965            |

| checkpoints              | REP-5 021_bleach_cleanser | REP-5 006_mustard_bottle | REP-5 010_potted_meat_can | ADD-10 021_bleach_cleanser | ADD-10 006_mustard_bottle |  ADD-10 010_potted_meat_can |
|----------------------|--------------------------|--------------------------|------------------------|---------------------------|----------------------------|----------------------------|
| 70 epoch | 0.8729                   | 0.5539                   | 0.5347                    | 0.8918                     | 0.7697                    | 0.5863                     |
| official | 0.6814                   | 0.6213                   | 0.4738                    | 0.8124                     | 0.8787                     |  0.5216                     |