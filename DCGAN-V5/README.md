## Key Improvements Made:

1. Better Chaotic Key Generation (v3_part1):

- Uses 1-DEC map from the paper (exponential Chebyshev map)
- Adds tent map for diversity
- Generates 8 keys instead of 4 (matching paper's approach)
- Better initial conditions

2. Stronger Encryption (v3_part2):

- MultiLayerKeyEncryption: 4 separate key-mixing layers
- Each layer uses different key transformations
- Transformer layers (4 heads) for complex encoding
- Stronger non-linear projections

3. Improved Bob & More Powerful Eve (v3_part3):

- Bob mirrors Alice's decryption with key access
- Eve gets 6 transformer layers (vs 4 for Alice/Bob)
- Eve uses 8 attention heads (more capacity)
- Eve has NO access to keys whatsoever

4. Better Training Strategy (v3_part4):

- Stage 1: 150 epochs (up from 100) for perfect reconstruction
- AdamW optimizer with weight decay
- Cosine annealing learning rate schedule
- Early stopping when Bob reaches 95%+ accuracy
- Stage 3: Adversarial loss weight = 0.3 (Alice learns to fool Eve)
- Extended dataset (12 messages)
