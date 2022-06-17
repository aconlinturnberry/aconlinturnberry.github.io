---
layout: post
title:  "XYC, Inc!"
date:   2022-06-14 15:19:40 -0500
---
XYZ, Inc. collects data feeds about real estate transactions and offers consolidated search, reporting, and other features on the standardize set of data e.g., a core set of metadata and then extensions as a property bag specific to each provider. They want a program that will accept data from their clients and manipulate the data to format it into an industry standard. This is in order to successfully organize data in a readable way for their clients to work with.

# Project
## Context
Our goal is to turn a legacy system format into an industry format (ex. MISMO).

### Decision Overview
- Before converting a file, the user must select the industry format that they would like to have it be in 
- Using the Python coding language, our program will take the legacy file and parse it to collect the info needed. Then our program will convert it into a JSON format following the industry standard chosen by the client.
- Finally, our program will verify the format at the end of the process.

## Flowcharts
### Main process
[![](https://mermaid.ink/img/pako:eNp1kcFqwzAQRH9lUS8OJNC4LQUdeqhd31oCLr3IPijSKhaVpSDJBBPy71ViB1Jo9zQwb9hh90iEk0goUcYdRMd9hM-ysZAmDNud5_sO3rm2sPFOYAiTpeU6Y4XRaCPUaGWAShsM7QJWq5crkmc1GhQRPvAAlfM9j7_8B8Y2Y-ychSJVgKLjdodhJtuWUhpcj8LwENa3uUfGvtBrNf6J5rfoU8bO9eCVi2-IDqbK7WLykzOJS7BEBTcLlTaG3j3fl2VV_UflM1VdprFkSXpMlbRMBz2eUw2JHfbYEJqkRMUHExvS2FNCh73kEd-kjs4TqrgJuCR8iK4erSA0-gGvUKl5ekU_U6cfiHWO3A)](https://mermaid.live/edit#pako:eNp1kcFqwzAQRH9lUS8OJNC4LQUdeqhd31oCLr3IPijSKhaVpSDJBBPy71ViB1Jo9zQwb9hh90iEk0goUcYdRMd9hM-ysZAmDNud5_sO3rm2sPFOYAiTpeU6Y4XRaCPUaGWAShsM7QJWq5crkmc1GhQRPvAAlfM9j7_8B8Y2Y-ychSJVgKLjdodhJtuWUhpcj8LwENa3uUfGvtBrNf6J5rfoU8bO9eCVi2-IDqbK7WLykzOJS7BEBTcLlTaG3j3fl2VV_UflM1VdprFkSXpMlbRMBz2eUw2JHfbYEJqkRMUHExvS2FNCh73kEd-kjs4TqrgJuCR8iK4erSA0-gGvUKl5ekU_U6cfiHWO3A)

### Sub-Processes
[![](https://mermaid.ink/img/pako:eNp10VFrwjAQAOC_cmQvFZRZH6bmYUOshcFwYsdgWB-y5GrD0qQ06UTE_75YW2WD3UvC5Tty3B0JNwIJJZkye56zysFblGrwYevPXcXKHOZeQOzfL3kpHoLNrCxhjVziN1qIpcJtj1JqTYFcMWvDK4XB4NGf4-BcMc-Rf1lIUCF3KCA2VcFcr8PjFk-CFasswgvuGD-cFTzrrLHS6CuftHx6nOmDy6XewaIo3eHp1ImpF_CxSFoYDoM1lopxhL10OSzvZ71fdPnayTBY1c7_6gwscf-30XDYuVGwSVAL8O4dK5lJ3vS4vdHwSi8pry-XZlARZnCbGmRSKXo3HkZRHP-nRq2KmyB9UqBvTgq_xOO5JiUuxwJTQv1VYMZq5VKS6pOndSmYw4WQzlSEZkxZ7BNWO5McNCfUVTV2KJLMr79o1ekHheSthg)](https://mermaid.live/edit#pako:eNp10VFrwjAQAOC_cmQvFZRZH6bmYUOshcFwYsdgWB-y5GrD0qQ06UTE_75YW2WD3UvC5Tty3B0JNwIJJZkye56zysFblGrwYevPXcXKHOZeQOzfL3kpHoLNrCxhjVziN1qIpcJtj1JqTYFcMWvDK4XB4NGf4-BcMc-Rf1lIUCF3KCA2VcFcr8PjFk-CFasswgvuGD-cFTzrrLHS6CuftHx6nOmDy6XewaIo3eHp1ImpF_CxSFoYDoM1lopxhL10OSzvZ71fdPnayTBY1c7_6gwscf-30XDYuVGwSVAL8O4dK5lJ3vS4vdHwSi8pry-XZlARZnCbGmRSKXo3HkZRHP-nRq2KmyB9UqBvTgq_xOO5JiUuxwJTQv1VYMZq5VKS6pOndSmYw4WQzlSEZkxZ7BNWO5McNCfUVTV2KJLMr79o1ekHheSthg)

[![](https://mermaid.ink/img/pako:eNp1kE1rAjEQhv_KkF5WUKjWUsihUFz36EFLL66HmEzcoflY8lEp4n9v1NVb5_Qy88y8w3ti0itknLVOG3-UnQgJPuvWQamY94cg-g6-MJAmKRJ5dxuRmr5U2zVKwh-EFR5hle0eQ9yNOOfRW5RGxDiDyeT9As-rRYfyGxoyGOHjIMjFYoS2NyLh6HF0fl94rbYbdAqSh4UhdGk3QKV5E1eDGjU83KagyRj-9PZc103zHzUbqOZabMwsBitIlRBOl52WpQ4ttowXqVCLbFJb8jkXNPeqvLtUlHxgXAsTccxETn7z6yTjKWS8QzWJEp4dqPMfQC122Q)](https://mermaid.live/edit#pako:eNp1kE1rAjEQhv_KkF5WUKjWUsihUFz36EFLL66HmEzcoflY8lEp4n9v1NVb5_Qy88y8w3ti0itknLVOG3-UnQgJPuvWQamY94cg-g6-MJAmKRJ5dxuRmr5U2zVKwh-EFR5hle0eQ9yNOOfRW5RGxDiDyeT9As-rRYfyGxoyGOHjIMjFYoS2NyLh6HF0fl94rbYbdAqSh4UhdGk3QKV5E1eDGjU83KagyRj-9PZc103zHzUbqOZabMwsBitIlRBOl52WpQ4ttowXqVCLbFJb8jkXNPeqvLtUlHxgXAsTccxETn7z6yTjKWS8QzWJEp4dqPMfQC122Q)

### Decision Consequences
- Python tends to be a slow language when working with databases which can impact the programs overall execution.
- If it has to interact with the database, it may have some issues and not have smooth interactions if the legacy data is too complex.