---
layout: post
title:  "XYC, Inc!"
date:   2022-06-14 15:19:40 -0500
---
XYZ, Inc. collects data feeds about real estate transactions and offers consolidated search, reporting, and other features on the standardize set of data e.g., a core set of metadata and then extensions as a property bag specific to each provider. They want a program that will accept data from their clients and manipulate the data to format it into an industry standard. This is in order to successfully organize data in a readable way for their clients to work with.

## Project

### Context
Our goal is to turn a legacy system format into an industry format (ex. MISMO)

### Decision Overview
- Before converting a file, the user must select the industry format that they would like to have it be in 
- Using the Python coding language, our program will take the legacy file and parse it to collect the info needed. Then our program will convert it into a JSON format following the industry standard chosen by the client.
- Finally, our program will verify the format at the end of the process.

[![](https://mermaid.ink/img/pako:eNptk01vm0AQhv_KaE9YiokX8OehlevEUqXKipKqF_BhA2NYGRYESy1k-b93DCy2o3IBzT4z-847w5mFeYRsxQ5pfgoTUWr4_RIooKeqP-NSFAls8zITGrZEdCcy4pbPbdikEpWGD1RRBVuZYrUfwXj8zVCO5dh0mmKoYYenvtAD4vq-a8Nbo5NcwYakwCYRKsaqh_f7e9rzfc-GP1jKQ_NfYGr5U7sVBD9EeASd9yL3I4PMLH9mw7oo4B1DiX-xk26AoetWzH3Ps-tF9J5b8y5_k2B4rPoGMTLtGX7e8wtrQR2KskL4hbEIW-XwUx1aXOZqyFj0Gcvzkm5QZIpUMbxmhW6-Xwy0JAgaUt2xfGLxiU29FKkIEU5SJ7B7Xo8ecJUbmlucBvdWaxJA5txNZRjtxLAODdnp3SS2tV2GreSbnZwPeBci-ouT94lDmkvFXdvMoBWyq7NPLPsdujKexWncrc3desE6FlJVtKOYUb8abzI8k0QrwKc31Y_jH8TR5sHYbjNmQw3HhNxh4UyEDyE-NTFvqMmeWIbkoozoTzpfwwHTCWYYsBV9RqI8BixQF-LqIiLdr5HUeclWB5FW-MRErfOPRoVspcsaDfQiBRmY9dTlH2-VGSU)](https://mermaid.live/edit#pako:eNptk01vm0AQhv_KaE9YiokX8OehlevEUqXKipKqF_BhA2NYGRYESy1k-b93DCy2o3IBzT4z-847w5mFeYRsxQ5pfgoTUWr4_RIooKeqP-NSFAls8zITGrZEdCcy4pbPbdikEpWGD1RRBVuZYrUfwXj8zVCO5dh0mmKoYYenvtAD4vq-a8Nbo5NcwYakwCYRKsaqh_f7e9rzfc-GP1jKQ_NfYGr5U7sVBD9EeASd9yL3I4PMLH9mw7oo4B1DiX-xk26AoetWzH3Ps-tF9J5b8y5_k2B4rPoGMTLtGX7e8wtrQR2KskL4hbEIW-XwUx1aXOZqyFj0Gcvzkm5QZIpUMbxmhW6-Xwy0JAgaUt2xfGLxiU29FKkIEU5SJ7B7Xo8ecJUbmlucBvdWaxJA5txNZRjtxLAODdnp3SS2tV2GreSbnZwPeBci-ouT94lDmkvFXdvMoBWyq7NPLPsdujKexWncrc3desE6FlJVtKOYUb8abzI8k0QrwKc31Y_jH8TR5sHYbjNmQw3HhNxh4UyEDyE-NTFvqMmeWIbkoozoTzpfwwHTCWYYsBV9RqI8BixQF-LqIiLdr5HUeclWB5FW-MRErfOPRoVspcsaDfQiBRmY9dTlH2-VGSU)


### Decision Consequences
- Python tends to be a slow language when working with databases which can impact the programs overall execution.
- If it has to interact with the database, it may have some issues and not have smooth interactions if the legacy data is too complex.