---
mindmap-plugin: basic
time: 
tags: 
source:
---
# title
### description
- private-key encryption scheme used by Julius Caesar to communicate with his generals, achieved by shifting each alphabet by some fixed amount (the key)
- message space $M = \{A,B,...,Z\}∗$ and key space $K = \{0,1,...,25\}$:
- **Gen** outputs a uniformly random key k from $K = \{0,1,...,25\}$. 
- **Encryption** shifts the alphabet of each letter in the plain-text by *k*: $Enc_k\;(m_1m_2...m_n)=c_1c_2...c_n,\;where\;c_i = m_i +k \mod26$
- **Decryption** shifts each letter back:
$Dec_k(c_1c_2...c_n)=m_1m_2...m_n, where\;m_i =c_i + k \mod26$