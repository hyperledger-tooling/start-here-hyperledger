---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    Add get channel config endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Endpoint url: `api/v1/channels/:channel_id/config`

Example response 
```
{
    "groups": {},
    "mod_policy": "Admins",
    "policies": {
        "Admins": {
            "mod_policy": "Admins",
            "policy": {
                "type": 1,
                "value": {
                    "identities": [
                        {
                            "principal": {
                                "msp_identifier": "Org2.cello.comMSP",
                                "role": "ADMIN"
                            },
                            "principal_classification": "ROLE"
                        }
                    ],
                    "rule": {
                        "n_out_of": {
                            "n": 1,
                            "rules": [
                                {
                                    "signed_by": 0
                                }
                            ]
                        }
                    },
                    "version": 0
                }
            },
            "version": "0"
        },
        "Endorsement": {
            "mod_policy": "Admins",
            "policy": {
                "type": 1,
                "value": {
                    "identities": [
                        {
                            "principal": {
                                "msp_identifier": "Org2.cello.comMSP",
                                "role": "MEMBER"
                            },
                            "principal_classification": "ROLE"
                        }
                    ],
                    "rule": {
                        "n_out_of": {
                            "n": 1,
                            "rules": [
                                {
                                    "signed_by": 0
                                }
                            ]
                        }
                    },
                    "version": 0
                }
            },
            "version": "0"
        },
        "Readers": {
            "mod_policy": "Admins",
            "policy": {
                "type": 1,
                "value": {
                    "identities": [
                        {
                            "principal": {
                                "msp_identifier": "Org2.cello.comMSP",
                                "role": "MEMBER"
                            },
                            "principal_classification": "ROLE"
                        }
                    ],
                    "rule": {
                        "n_out_of": {
                            "n": 1,
                            "rules": [
                                {
                                    "signed_by": 0
                                }
                            ]
                        }
                    },
                    "version": 0
                }
            },
            "version": "0"
        },
        "Writers": {
            "mod_policy": "Admins",
            "policy": {
                "type": 1,
                "value": {
                    "identities": [
                        {
                            "principal": {
                                "msp_identifier": "Org2.cello.comMSP",
                                "role": "MEMBER"
                            },
                            "principal_classification": "ROLE"
                        }
                    ],
                    "rule": {
                        "n_out_of": {
                            "n": 1,
                            "rules": [
                                {
                                    "signed_by": 0
                                }
                            ]
                        }
                    },
                    "version": 0
                }
            },
            "version": "0"
        }
    },
    "values": {
        "MSP": {
            "mod_policy": "Admins",
            "value": {
                "config": {
                    "admins": [],
                    "crypto_config": {
                        "identity_identifier_hash_function": "SHA256",
                        "signature_hash_family": "SHA2"
                    },
                    "fabric_node_ous": {
                        "admin_ou_identifier": {
                            "certificate": "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNJakNDQWNtZ0F3SUJBZ0lRRXZkT2laL2Y0VTFCTlFXaSt5c2dYakFLQmdncWhrak9QUVFEQWpCY01Rc3cKQ1FZRFZRUUdFd0pEVGpFTE1Ba0dBMVVFQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dgpjbWN5TG1ObGJHeHZMbU52YlRFYU1CZ0dBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd0hoY05Nakl3Ck9EQTRNREV5T1RBd1doY05Nekl3T0RBMU1ERXlPVEF3V2pCY01Rc3dDUVlEVlFRR0V3SkRUakVMTUFrR0ExVUUKQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dmNtY3lMbU5sYkd4dkxtTnZiVEVhTUJnRwpBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd1dUQVRCZ2NxaGtqT1BRSUJCZ2dxaGtqT1BRTUJCd05DCkFBU25EbEsrb0J6OGIvVmpyNTlTdnRQZk95TE9HZDUyMktyMUUzK0xQelVqM2VnaGxLVVFjNnk4OHpVWW9MYmgKZ0hZSjNaek5jNzVmYWRpMVA4ZjdEZUxjbzIwd2F6QU9CZ05WSFE4QkFmOEVCQU1DQWFZd0hRWURWUjBsQkJZdwpGQVlJS3dZQkJRVUhBd0lHQ0NzR0FRVUZCd01CTUE4R0ExVWRFd0VCL3dRRk1BTUJBZjh3S1FZRFZSME9CQ0lFCklGRlNSdFpUSE5YNk1UM242bmt0aVA5WG1ORDdrTXVyckp1bzgzZEFvZ3hHTUFvR0NDcUdTTTQ5QkFNQ0EwY0EKTUVRQ0lIbnNmZ0JHd0RkVVNyaDRFSHJFR2FQK1JCZjA3MVFhMU5wSTlGT0RFUlFnQWlBalloWXptYkFMWC9CbAoydDRXL0NjbFpYTGpLaWtzQllPOGRWeEJEWkQ1d2c9PQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==",
                            "organizational_unit_identifier": "admin"
                        },
                        "client_ou_identifier": {
                            "certificate": "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNJakNDQWNtZ0F3SUJBZ0lRRXZkT2laL2Y0VTFCTlFXaSt5c2dYakFLQmdncWhrak9QUVFEQWpCY01Rc3cKQ1FZRFZRUUdFd0pEVGpFTE1Ba0dBMVVFQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dgpjbWN5TG1ObGJHeHZMbU52YlRFYU1CZ0dBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd0hoY05Nakl3Ck9EQTRNREV5T1RBd1doY05Nekl3T0RBMU1ERXlPVEF3V2pCY01Rc3dDUVlEVlFRR0V3SkRUakVMTUFrR0ExVUUKQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dmNtY3lMbU5sYkd4dkxtTnZiVEVhTUJnRwpBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd1dUQVRCZ2NxaGtqT1BRSUJCZ2dxaGtqT1BRTUJCd05DCkFBU25EbEsrb0J6OGIvVmpyNTlTdnRQZk95TE9HZDUyMktyMUUzK0xQelVqM2VnaGxLVVFjNnk4OHpVWW9MYmgKZ0hZSjNaek5jNzVmYWRpMVA4ZjdEZUxjbzIwd2F6QU9CZ05WSFE4QkFmOEVCQU1DQWFZd0hRWURWUjBsQkJZdwpGQVlJS3dZQkJRVUhBd0lHQ0NzR0FRVUZCd01CTUE4R0ExVWRFd0VCL3dRRk1BTUJBZjh3S1FZRFZSME9CQ0lFCklGRlNSdFpUSE5YNk1UM242bmt0aVA5WG1ORDdrTXVyckp1bzgzZEFvZ3hHTUFvR0NDcUdTTTQ5QkFNQ0EwY0EKTUVRQ0lIbnNmZ0JHd0RkVVNyaDRFSHJFR2FQK1JCZjA3MVFhMU5wSTlGT0RFUlFnQWlBalloWXptYkFMWC9CbAoydDRXL0NjbFpYTGpLaWtzQllPOGRWeEJEWkQ1d2c9PQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==",
                            "organizational_unit_identifier": "client"
                        },
                        "enable": true,
                        "orderer_ou_identifier": {
                            "certificate": "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNJakNDQWNtZ0F3SUJBZ0lRRXZkT2laL2Y0VTFCTlFXaSt5c2dYakFLQmdncWhrak9QUVFEQWpCY01Rc3cKQ1FZRFZRUUdFd0pEVGpFTE1Ba0dBMVVFQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dgpjbWN5TG1ObGJHeHZMbU52YlRFYU1CZ0dBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd0hoY05Nakl3Ck9EQTRNREV5T1RBd1doY05Nekl3T0RBMU1ERXlPVEF3V2pCY01Rc3dDUVlEVlFRR0V3SkRUakVMTUFrR0ExVUUKQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dmNtY3lMbU5sYkd4dkxtTnZiVEVhTUJnRwpBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd1dUQVRCZ2NxaGtqT1BRSUJCZ2dxaGtqT1BRTUJCd05DCkFBU25EbEsrb0J6OGIvVmpyNTlTdnRQZk95TE9HZDUyMktyMUUzK0xQelVqM2VnaGxLVVFjNnk4OHpVWW9MYmgKZ0hZSjNaek5jNzVmYWRpMVA4ZjdEZUxjbzIwd2F6QU9CZ05WSFE4QkFmOEVCQU1DQWFZd0hRWURWUjBsQkJZdwpGQVlJS3dZQkJRVUhBd0lHQ0NzR0FRVUZCd01CTUE4R0ExVWRFd0VCL3dRRk1BTUJBZjh3S1FZRFZSME9CQ0lFCklGRlNSdFpUSE5YNk1UM242bmt0aVA5WG1ORDdrTXVyckp1bzgzZEFvZ3hHTUFvR0NDcUdTTTQ5QkFNQ0EwY0EKTUVRQ0lIbnNmZ0JHd0RkVVNyaDRFSHJFR2FQK1JCZjA3MVFhMU5wSTlGT0RFUlFnQWlBalloWXptYkFMWC9CbAoydDRXL0NjbFpYTGpLaWtzQllPOGRWeEJEWkQ1d2c9PQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==",
                            "organizational_unit_identifier": "orderer"
                        },
                        "peer_ou_identifier": {
                            "certificate": "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNJakNDQWNtZ0F3SUJBZ0lRRXZkT2laL2Y0VTFCTlFXaSt5c2dYakFLQmdncWhrak9QUVFEQWpCY01Rc3cKQ1FZRFZRUUdFd0pEVGpFTE1Ba0dBMVVFQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dgpjbWN5TG1ObGJHeHZMbU52YlRFYU1CZ0dBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd0hoY05Nakl3Ck9EQTRNREV5T1RBd1doY05Nekl3T0RBMU1ERXlPVEF3V2pCY01Rc3dDUVlEVlFRR0V3SkRUakVMTUFrR0ExVUUKQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dmNtY3lMbU5sYkd4dkxtTnZiVEVhTUJnRwpBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd1dUQVRCZ2NxaGtqT1BRSUJCZ2dxaGtqT1BRTUJCd05DCkFBU25EbEsrb0J6OGIvVmpyNTlTdnRQZk95TE9HZDUyMktyMUUzK0xQelVqM2VnaGxLVVFjNnk4OHpVWW9MYmgKZ0hZSjNaek5jNzVmYWRpMVA4ZjdEZUxjbzIwd2F6QU9CZ05WSFE4QkFmOEVCQU1DQWFZd0hRWURWUjBsQkJZdwpGQVlJS3dZQkJRVUhBd0lHQ0NzR0FRVUZCd01CTUE4R0ExVWRFd0VCL3dRRk1BTUJBZjh3S1FZRFZSME9CQ0lFCklGRlNSdFpUSE5YNk1UM242bmt0aVA5WG1ORDdrTXVyckp1bzgzZEFvZ3hHTUFvR0NDcUdTTTQ5QkFNQ0EwY0EKTUVRQ0lIbnNmZ0JHd0RkVVNyaDRFSHJFR2FQK1JCZjA3MVFhMU5wSTlGT0RFUlFnQWlBalloWXptYkFMWC9CbAoydDRXL0NjbFpYTGpLaWtzQllPOGRWeEJEWkQ1d2c9PQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg==",
                            "organizational_unit_identifier": "peer"
                        }
                    },
                    "intermediate_certs": [],
                    "name": "Org2.cello.comMSP",
                    "organizational_unit_identifiers": [],
                    "revocation_list": [],
                    "root_certs": [
                        "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNJakNDQWNtZ0F3SUJBZ0lRRXZkT2laL2Y0VTFCTlFXaSt5c2dYakFLQmdncWhrak9QUVFEQWpCY01Rc3cKQ1FZRFZRUUdFd0pEVGpFTE1Ba0dBMVVFQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dgpjbWN5TG1ObGJHeHZMbU52YlRFYU1CZ0dBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd0hoY05Nakl3Ck9EQTRNREV5T1RBd1doY05Nekl3T0RBMU1ERXlPVEF3V2pCY01Rc3dDUVlEVlFRR0V3SkRUakVMTUFrR0ExVUUKQ0JNQ1ExQXhDekFKQmdOVkJBY1RBa0pLTVJjd0ZRWURWUVFLRXc1dmNtY3lMbU5sYkd4dkxtTnZiVEVhTUJnRwpBMVVFQXhNUlkyRXViM0puTWk1alpXeHNieTVqYjIwd1dUQVRCZ2NxaGtqT1BRSUJCZ2dxaGtqT1BRTUJCd05DCkFBU25EbEsrb0J6OGIvVmpyNTlTdnRQZk95TE9HZDUyMktyMUUzK0xQelVqM2VnaGxLVVFjNnk4OHpVWW9MYmgKZ0hZSjNaek5jNzVmYWRpMVA4ZjdEZUxjbzIwd2F6QU9CZ05WSFE4QkFmOEVCQU1DQWFZd0hRWURWUjBsQkJZdwpGQVlJS3dZQkJRVUhBd0lHQ0NzR0FRVUZCd01CTUE4R0ExVWRFd0VCL3dRRk1BTUJBZjh3S1FZRFZSME9CQ0lFCklGRlNSdFpUSE5YNk1UM242bmt0aVA5WG1ORDdrTXVyckp1bzgzZEFvZ3hHTUFvR0NDcUdTTTQ5QkFNQ0EwY0EKTUVRQ0lIbnNmZ0JHd0RkVVNyaDRFSHJFR2FQK1JCZjA3MVFhMU5wSTlGT0RFUlFnQWlBalloWXptYkFMWC9CbAoydDRXL0NjbFpYTGpLaWtzQllPOGRWeEJEWkQ1d2c9PQotLS0tLUVORCBDRVJUSUZJQ0FURS0tLS0tCg=="
                    ],
                    "signing_identity": null,
                    "tls_intermediate_certs": [],
                    "tls_root_certs": [
                        "LS0tLS1CRUdJTiBDRVJUSUZJQ0FURS0tLS0tCk1JSUNLakNDQWRDZ0F3SUJBZ0lSQUlVS2dBaG5nVFNWMGxXc2RJczJyMTh3Q2dZSUtvWkl6ajBFQXdJd1h6RUwKTUFrR0ExVUVCaE1DUTA0eEN6QUpCZ05WQkFnVEFrTlFNUXN3Q1FZRFZRUUhFd0pDU2pFWE1CVUdBMVVFQ2hNTwpiM0puTWk1alpXeHNieTVqYjIweEhUQWJCZ05WQkFNVEZIUnNjMk5oTG05eVp6SXVZMlZzYkc4dVkyOXRNQjRYCkRUSXlNRGd3T0RBeE1qa3dNRm9YRFRNeU1EZ3dOVEF4TWprd01Gb3dYekVMTUFrR0ExVUVCaE1DUTA0eEN6QUoKQmdOVkJBZ1RBa05RTVFzd0NRWURWUVFIRXdKQ1NqRVhNQlVHQTFVRUNoTU9iM0puTWk1alpXeHNieTVqYjIweApIVEFiQmdOVkJBTVRGSFJzYzJOaExtOXlaekl1WTJWc2JHOHVZMjl0TUZrd0V3WUhLb1pJemowQ0FRWUlLb1pJCnpqMERBUWNEUWdBRWtLQVBIby9IRGI0L2xqQzQ3ZTJLTDlVUXBzNlFZUVFrbkNPTHdGM093UXdqSTVGQkVQNTcKd2pRUFBmQ1E1bWtyMTNCZjNoNmpOeTR1Qi9FSlkrazdNcU50TUdzd0RnWURWUjBQQVFIL0JBUURBZ0dtTUIwRwpBMVVkSlFRV01CUUdDQ3NHQVFVRkJ3TUNCZ2dyQmdFRkJRY0RBVEFQQmdOVkhSTUJBZjhFQlRBREFRSC9NQ2tHCkExVWREZ1FpQkNCc0ZvMlFsSmNZaDJIcEtSTFdHV3ovZ3puNUtKakF2clMydmZlNU9neVczekFLQmdncWhrak8KUFFRREFnTklBREJGQWlFQXI1UlNPeUtjekI1UXhRVzhmU0VJSFRUb3JleEhXV3YzbFFjR1ppcEtIcmNDSUNvRApEUXpqaGJ2anh5Szc4OGJRT0VFRmVBM1pneE9TS20zZ2JtQ1NudDVLCi0tLS0tRU5EIENFUlRJRklDQVRFLS0tLS0K"
                    ]
                },
                "type": 0
            },
            "version": "0"
        }
    },
    "version": "0"
}
```

Signed-off-by: Yuanmao Zhu [yuanmao@ualberta.ca](mailto:yuanmao@ualberta.ca)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 02:58:32 +0000 UTC
    </div>
</div>

