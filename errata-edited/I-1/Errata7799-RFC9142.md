# Errata 7799 - RFC 9142

- **RFC Title:** Key Exchange (KEX) Method Updates and Recommendations for Secure Shell (SSH)
- **RFC Publication Date:** January 2022

```
Section 1.2.1 says:


+============+=============================+

| Curve Name | Estimated Security Strength |

+============+=============================+

| nistp256   | 128 bits                    |

+------------+-----------------------------+

| nistp384   | 192 bits                    |

+------------+-----------------------------+

| nistp521   | 512 bits                    |

+------------+-----------------------------+

| curve25519 | 128 bits                    |

+------------+-----------------------------+

| curve448   | 224 bits                    |

+------------+-----------------------------+

// state how to fix the above text here

```

## Issue description

The estimated security strength for one of the curve names is incorrectly listed in the table as per Table 1 of Section 6.1.1 of FIPS 186-5 and Section 9 Paragraph 5 of RFC 5656.
