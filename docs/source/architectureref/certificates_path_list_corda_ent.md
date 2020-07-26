Certificate Paths on Vault for Corda Enterprise
-----------------------------------------------
All values are Base64 encoded files.

### For CENM

| Path (on Vault secrets)           | Crypto-material         | Type        |
|-----------------------------------|-------------------------|-------------|
| /secrets/cenm/root/certs          | root-key-store.jks                | Root keystore |
| /secrets/cenm/root/certs          | corda-ssl-trust-store.jks         | SSL certificates truststore |
| /secrets/cenm/root/certs          | network-root-truststore.jks       | Network Root certificates truststore |
| /secrets/cenm/root/certs          | corda-ssl-root-keys.jks           | SSL Root keystore |
| /secrets/cenm/root/certs          | tls-crl-signer-key-store.jks      | Keystore containing tlscrlsigner key |
| /secrets/cenm/root/certs          | subordinate-key-store.jks         | Keystore containing subordinateca key |
| /secrets/cenm/signer/certs        | corda-ssl-signer-keys.jks         | Signer keystore |
| /secrets/cenm/signer/certs        | identity-manager-key-store.jks    | Idman keystore |
| /secrets/cenm/signer/certs        | network-map-key-store.jks         | Networkmap keystore |
| /secrets/cenm/networkmap/certs    | corda-ssl-network-map-keys.jks    | Networkmap SSL keystore |
| /secrets/cenm/networkmap/tlscerts | tlscacerts                        | Networkmap Ambassador Certificate |
| /secrets/cenm/networkmap/tlscerts | tlskey                            | Networkmap Ambassador Private key |
| /secrets/cenm/idman/crls          | tls.crl                           | TLS CRL |
| /secrets/cenm/idman/crls          | ssl.crl                           | SSL CRL |
| /secrets/cenm/idman/crls          | root.crl                          | Network Root CRL|
| /secrets/cenm/idman/crls          | subordinate.crl                   | Subordinate CRL |
| /secrets/cenm/idman/certs         | corda-ssl-identity-manager-keys.jks  | Idman SSL keystore |
| /secrets/cenm/idman/tlscerts      | tlscacerts                        | Idman Ambassador Certificate |
| /secrets/cenm/idman/tlscerts      | tlskey                            | Idman Ambassador Private key |
| /secrets/cenm/`notary_service_name`/certs                             | Notary.cer                 | Certificate |
| /secrets/cenm/`notary_service_name`/certs                             | Notary.key                 | Private key |
| /secrets/cenm/`notary_service_name`/certs/idman                       | idman.crt                  | Idman Ambassador Certificate |
| /secrets/cenm/`notary_service_name`/certs/networkmap                  | networkmap.crt             | Networkmap Ambassador Certificate |
| /secrets/cenm/`notary_service_name`/certs/networkmaptruststore        | network-map-truststore     | Certificate |
| /secrets/cenm/`notary_service_name`/certs/nodekeystore                | nodekeystore.jks           | Certificate |
| /secrets/cenm/`notary_service_name`/certs/sslkeystore                 | sslkeystore.jks            | Certificate |
| /secrets/cenm/`notary_service_name`/certs/truststore                  | truststore.jks             | Certificate |
| /secrets/cenm/`notary_service_name`/tlscerts                          | tlscacerts                 | Notary Ambassador Certificate |
| /secrets/cenm/`notary_service_name`/tlscerts                          | tlskey                     | Notary Ambassador Private key |
| /secrets/cenm/`notary_service_name`/nodeInfo                          | nodeInfo                   | Notary node info              |
| /secrets/cenm/`notary_service_name`/nparm                             | network-parameters-initial | Network initial parameters    |

-----

### For Node/Peer Organization WIP

| Path (`orgname_lowercase` crypto material)              | Crypto-material        | Type        |
|--------------------------------------------------|------------------------|-------------|
| /secrets/`orgname_lowercase`/certs                      | `orgname_lowercase`.cer       | Certificate |
| /secrets/`orgname_lowercase`/certs                      | `orgname_lowercase`.key       | Private key |
| /secrets/`orgname_lowercase`/certs/customnodekeystore   | nodekeystore.jks       | Certificate |
| /secrets/`orgname_lowercase`/certs/idman                | idman.crt            | Idman Ambassador Certificate |
| /secrets/`orgname_lowercase`/certs/networkmap           | networkmap.crt         | Networkmap Ambassador Certificate |
| /secrets/`orgname_lowercase`/certs/networkmaptruststore | network-map-truststore | Certificate |
| /secrets/`orgname_lowercase`/certs/nodekeystore         | nodekeystore.jks       | Certificate |
| /secrets/`orgname_lowercase`/certs/sslkeystore          | sslkeystore.jks        | Certificate |
| /secrets/`orgname_lowercase`/certs/truststore           | truststore.jks         | Certificate |
| /secrets/`orgname_lowercase`/tlscerts                   | tlscacerts             | Node Ambassador Certificate |
| /secrets/`orgname_lowercase`/tlscerts                   | tlskey                 | Node Ambassador Private key |