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

[![](https://mermaid.ink/img/pako:eNpVkM-KwkAMxl8l5OSCfYEeBG3Vi6Cgt46H0InOIPOHdMoibd99p5aF3ZyS7_t9IWTANmjGEp9C0cCtVh5ybZvKiO2So-4ORbEZj5zABc_vEXarY4DOhBitf34t_G6GoBpOM8aQjPWvabGqT_7seYS6OVFMId7_OrfvMMK-sReT1_93jHBOHZoHlQ8qWhKoSD4IrtGxOLI6nz7MisJk2LHCMrea5KVQ-SlzfdSUeK9tCoJlkp7XSH0K17dvf-eFqS3lL7hFnH4ABg5bBA)](https://mermaid.live/edit#pako:eNpVkM-KwkAMxl8l5OSCfYEeBG3Vi6Cgt46H0InOIPOHdMoibd99p5aF3ZyS7_t9IWTANmjGEp9C0cCtVh5ybZvKiO2So-4ORbEZj5zABc_vEXarY4DOhBitf34t_G6GoBpOM8aQjPWvabGqT_7seYS6OVFMId7_OrfvMMK-sReT1_93jHBOHZoHlQ8qWhKoSD4IrtGxOLI6nz7MisJk2LHCMrea5KVQ-SlzfdSUeK9tCoJlkp7XSH0K17dvf-eFqS3lL7hFnH4ABg5bBA)


### Decision Consequences
- Python tends to be a slow language when working with databases which can impact the programs overall execution.
- If it has to interact with the database, it may have some issues and not have smooth interactions if the legacy data is too complex.