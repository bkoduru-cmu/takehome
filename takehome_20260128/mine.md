
1. Learning Rate (lr): Increase lr → Decrease effect. High lr "washes away" the shared initialization too quickly.
2. Weight Initialization Scale (σ): Decrease σ → Decrease effect. Smaller weights provide less "direction" for the gradients to align.
3. Batch Size: Increase batch size → Increase effect. Smoother gradients lead to more stable "alignment" between the teacher's latent features and the student's updates.
4. Optimizer Choice (SGD vs. Adam): Adam → Decrease effect. Adaptive momentum might track noise specific to the student's random data, diverging from the teacher's structure.
5. Data Sparsity (Zero-masking pixels): Increase sparsity → Decrease effect. Less signal makes it harder for the gradient to find the "subliminal" direction.
