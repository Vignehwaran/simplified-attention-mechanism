
##simplified-attention-mechanism

Introduction

Before diving into the self-attention layer, it’s useful to experiment with a simplified attention mechanism built from scratch.
This approach helps us understand the core principle of attention—without trainable parameters—before moving on to the more advanced self-attention used in Transformers.

❓ What is the First Principle of Attention?

The first principle of the attention mechanism is the most basic form of attention:

It calculates relevance (similarity) between tokens.

No trainable weights are involved.

The mechanism relies purely on dot products and normalization.

👉 In short: It’s about how one word decides “how much” to attend to another word.

🧪 Why This Experiment?

Builds intuition for how self-attention is derived.

Helps visualize attention weights without the complexity of parameters.

Acts as a foundation for learning scaled dot-product attention and multi-head attention later.

⚙️ Steps of Simplified Attention (No Trainable Parameters)

Input Representation
Convert words into embedding vectors.

Similarity Computation
Measure how similar each word is to others (using dot product).

Normalization
Apply softmax to turn similarity scores into probabilities.

Weighted Sum
Multiply embeddings by attention weights → get the context vector.
