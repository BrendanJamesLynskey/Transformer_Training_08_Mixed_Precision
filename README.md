# Transformer Training 08 — Mixed Precision: BF16, FP16, FP8 and Quantised Gradients

Real training computes in 16 and even 8 bits. Exponent against mantissa, BF16 against FP16, FP32 master weights and loss scaling, FP8 with per-tensor scaling, and gradients quantised to a few bits, each emulated on the model and measured.

**Live site:** https://brendanjameslynskey.github.io/Transformer_Training_08_Mixed_Precision/

Floating-point formats and a live rounding calculator; BF16 vs FP16 range; master weights, FP32 accumulation, loss scaling; measured recipes; FP8 with per-tensor scaling; quantised gradients.

## Live, animated companion

This deck is the slide companion to [Training](https://transformer-training-explained.vercel.app/training), the second site of the Foundations track (after Decoder), where the Decoder's model trains in your browser:

- [Chapter 9: Mixed precision](https://transformer-training-explained.vercel.app/training/09-mixed-precision)

## Where the numbers come from

Every measured number on these slides comes from the site's [results.md](https://github.com/BrendanJamesLynskey/transformer-explainer/blob/main/results.md) (seeded NumPy reference runs; CI recomputes them), filled in at build time from its `results.json`. Numbers from papers are cited on the slide with a link. The model is tiny (5,376 parameters, one book, a CPU): its runs show mechanisms, not what happens at scale, and the slides say so where it matters. GPU runs of the site's Colab notebooks are pending; no GPU number appears here.

Part of the [Transformer Training sub-hub](https://github.com/BrendanJamesLynskey/LLM_Hub_Transformer_Training) &middot; [LLMs hub](https://github.com/BrendanJamesLynskey/LLMs)
