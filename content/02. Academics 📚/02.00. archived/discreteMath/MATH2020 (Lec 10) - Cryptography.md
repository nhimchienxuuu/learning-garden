---

mindmap-plugin: basic

---
# Cryptography
## What is cryptography
- practice and study of techniques for securing communication and data in the presence of adversaried
- 2 types of cryptosystems
	- Private-key cryptography (symmetric cryptography)
	- Public-key cryptography (asymmetric cryptography)
<!--ID: 1708098042099-->


## Private-key encryption scheme
- A triplet of algorithms (Gen, Enc, Dec), a message space M, and a key space K
- Gen: Alice and Bob first need to meet in advance to generate and agree on a secret key k ← K.
- Enc: Alice has a private message m ∈ M for Bob, she sends c = Enck (m) over the insecure channel.
- Dec: Once Bob receives the cipher-text c, he decrypts it by running m = Deck(c) to read the original message.
<!--ID: 1708098042103-->


## Caesar Cipher
- private-key encryption scheme used by Julius Caesar to communicate with his generals, achieved by shifting each alphabet by some fixed amount (the key)
- message space $M = \{A,B,...,Z\}∗$ and key space $K = \{0,1,...,25\}$:
- **Gen** outputs a uniformly random key k from $K = \{0,1,...,25\}$. 
- **Encryption** shifts the alphabet of each letter in the plain-text by *k*: $Enc_k\;(m_1m_2...m_n)=c_1c_2...c_n,\;where\;c_i = m_i +k \mod26$
- **Decryption** shifts each letter back:
$Dec_k(c_1c_2...c_n)=m_1m_2...m_n, where\;m_i =c_i + k \mod26$
<!--ID: 1708098042106-->


### One-time pad scheme
- the key is as long as the message
- 
<!--ID: 1708098042109-->
