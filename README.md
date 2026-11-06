# Trust Before Talk: interactive companion

An interactive website for the article **“Trust Before Talk: Security and Privacy Trade-offs of Risk-Adaptive Post-Quantum Protection in Agent-to-Agent Systems”** (M. M. Wanniarachchi Kankanamge, N. Yang, H. Zangoti, A. R. Shahid).

## What is on the page

1. **Step by step**: a 17-step walkthrough of one booking, from the user's request to “booking confirmed”, showing which party uses which key (ML-KEM, ML-DSA, HKDF-SHA256, AES-256-GCM) and what a passive observer sees.
2. **Live simulation**: the communication model of Figure 2 running in the browser, with Standard, Fixed and Adaptive protection, the deterministic control layer, padding, and attacks A1–A6 plus a tier-rewrite attack.
3. **Keys and parameters**: FIPS 203/204 sizes, envelope fields and the key ring generated in the browser.
4. **Attack lab**: paired trials that rebuild Figure 3.
5. **Observer lab**: a k-NN classifier that recovers tiers from request lengths.
6. **Costs and lessons**.

ML-KEM and ML-DSA run in the browser through [noble-post-quantum](https://github.com/paulmillr/noble-post-quantum) loaded from jsDelivr; HKDF and AES-GCM use WebCrypto. If the library cannot load, the page falls back to byte-accurate stand-ins and says so in a badge at the top. The language-model assessor and the agents' answers are scripted.



