# NTcyber Main Business Portal

A lightweight, high-performance static web application designed and built from scratch to showcase cybersecurity consulting, infrastructure, and technical management services offered by **NTcyber**.

---

## Architecture & Deployment Model

The portal is hosted entirely on-premises on self-managed infrastructure, routed securely to the public internet using a defense-in-depth DevSecOps architecture:

```text
[ Web Client ] 
      │
      ▼
[ Cloudflare Edge / DNS ] ──( Cloudflare Encrypted Tunnel )──► [ Local Network ]
                                                                      │
                                                                      ▼
                                                            [ Traefik Reverse Proxy ]
                                                                      │
                                                                      ▼
                                                            [ ntcyber-site Engine ]
