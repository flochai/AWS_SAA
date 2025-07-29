IPsec (Internet Protocol Security) is a suite of protocols designed to establish secure, encrypted tunnels over insecure networks such as the public internet. It can securely connect two networks (e.g., a local site and a remote site) by providing authentication, integrity, and data encryption.

⸻

How IPsec Tunnels Work

- An IPsec tunnel is created when interesting traffic—traffic matching pre-defined rules or policies—triggers the connection.
- If no such traffic is detected, the tunnel is torn down to conserve resources.

<img width="2310" height="1192" alt="image" src="https://github.com/user-attachments/assets/de9f1c2f-301c-4f66-b331-d2e5738368d3" />


IPsec establishes secure communication in two phases using IKE (Internet Key Exchange):

1. IKE Phase 1 (Slow and Heavy)

- Authenticates both endpoints.
- Uses asymmetric encryption (e.g., RSA, Diffie-Hellman) to securely exchange keys.
- Establishes a shared symmetric key for faster data encryption.
- Creates the IKE SA (Security Association) tunnel.

<img width="1265" height="618" alt="image" src="https://github.com/user-attachments/assets/1fb1bece-4c9e-4edd-a462-b7d39e902548" />


2. IKE Phase 2 (Fast and Agile)

- Uses the keys from Phase 1 to establish IPsec SAs.
- Provides encryption and integrity for the actual data traffic (via ESP or AH protocols).
- This phase is faster because the heavy cryptographic operations have already been completed.

<img width="1260" height="600" alt="image" src="https://github.com/user-attachments/assets/139084dc-eeaa-48b2-b209-4e93ceed9a03" />
