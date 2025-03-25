Keyword spotting is a crucial aspect of hearing assistive devices, enabling them to detect and respond to specific spoken words or phrases.

Dataset
Google Speech Command Dataset:
Recorded by 1,881 speakers, this first version
consists of 64,727 one-second (or less) long
speech segments covering one word each
out of 30 possible different words.
The dataset is designed to help train and
evaluate keyword spotting systems. Its
primary goal is to provide a way to build and
test small models that detect when a single
word is spoken, from a set of ten target
words, with as few false positives as possible
from background noise or unrelated speech


KWT(Keyword Transformer)
A fully self-attentional architecture inspired by ViT
that can be used as a drop-in replacement for
existing keyword spotting models and visualize the
effect of the learned attention masks and positional
embeddings.
Architecture
Audio is preprocessed into a mel-scale spectrogram, which
is partitioned into non-overlapping patches in the time
domain.
Together with a learned class token, these form the input
tokens for a multilayer Transformer encoder.
A learned position embedding is added to each token.
The output of the class token is passed through a linear
head and used to make the final class prediction.

![Screenshot 2024-06-30 at 19 00 26](https://github.com/ShubhranshuMehta/Keyword-Spotting/assets/93399368/d6670dd1-d7da-46e5-b1c4-341297fbb487)
