---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
### description
- A triplet of algorithms (Gen, Enc, Dec), a message space M, and a key space K
- Gen: Alice and Bob first need to meet in advance to generate and agree on a secret key k ← K.
- Enc: Alice has a private message m ∈ M for Bob, she sends c = Enck (m) over the insecure channel.
- Dec: Once Bob receives the cipher-text c, he decrypts it by running m = Deck(c) to read the original message.