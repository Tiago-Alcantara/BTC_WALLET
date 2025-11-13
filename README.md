# 🪙 BTC Wallet Generator (Node.js)

Este projeto gera automaticamente uma **carteira Bitcoin HD (Hierarchical Deterministic)** usando as bibliotecas `bip32`, `bip39` e `bitcoinjs-lib`.

Ele cria:
- Um **mnemônico (12 palavras)**;
- A **chave privada (WIF)**;
- O **endereço Bitcoin** (P2SH-P2WPKH);
- Tudo funcionando na **testnet** por padrão (rede de testes do Bitcoin).

---

## 🚀 Tecnologias utilizadas

- [Node.js](https://nodejs.org/)
- [bitcoinjs-lib](https://github.com/bitcoinjs/bitcoinjs-lib)
- [bip32](https://github.com/bitcoinjs/bip32)
- [bip39](https://github.com/bitcoinjs/bip39)

---

## 📦 Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/BTC_WALLET.git
   cd BTC_WALLET

2. **Instale as dependências:**
   ```bash
      npm install bip32 bip39 bitcoinjs-lib
 3. *Execute o script:**
   ```bash
     node src/createWallet.js

## ⚙️ O que o script faz

1. Gera uma frase mnemônica (12 palavras) via BIP39.  
2. Cria uma seed a partir do mnemônico.  
3. Deriva as chaves (privada e pública) via BIP32.  
4. Gera um **endereço P2SH-P2WPKH** (compatível com carteiras SegWit).  
5. Exibe no terminal:

```yaml
✅ Carteira gerada com sucesso!
🧠 Mnemônico: ...
📬 Endereço BTC: ...
🔑 Chave Privada WIF: ...
