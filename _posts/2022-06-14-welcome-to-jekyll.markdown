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
[![](https://mermaid.ink/img/pako:eNp1kc1qwzAQhF9lUS8JJJC4tVt06KH5ubUEXHqxfFCldSwiS0GSCSbk3avUDriQ7mlgvmGH3TMRViKhpNL2JGruAnyumYE4vv3eO36s4Z0rAztnBXrfW0ouJ8VKKzQBcjTSw1Zp9OUU5vPXG5JMctQoAnzgCbbWNTz88R-LYteF2hpYxQqwqrnZox_IsqSUetug0Nz75Tj3VBRf6FTV3UWTMZpOims9eOPiAMFCX7mc9n50evEbXGMFo4WV0po-LF_SzfPiPyoZqDTLFlnCDDNkRhqMpZSMJz1fc4yEGhtkhEYpuTswwswlcu1R8oAbqYJ1hFZce5wR3gabd0YQGlyLN2itePxEM1CXH67jjcc)](https://mermaid.live/edit#pako:eNp1kc1qwzAQhF9lUS8JJJC4tVt06KH5ubUEXHqxfFCldSwiS0GSCSbk3avUDriQ7mlgvmGH3TMRViKhpNL2JGruAnyumYE4vv3eO36s4Z0rAztnBXrfW0ouJ8VKKzQBcjTSw1Zp9OUU5vPXG5JMctQoAnzgCbbWNTz88R-LYteF2hpYxQqwqrnZox_IsqSUetug0Nz75Tj3VBRf6FTV3UWTMZpOims9eOPiAMFCX7mc9n50evEbXGMFo4WV0po-LF_SzfPiPyoZqDTLFlnCDDNkRhqMpZSMJz1fc4yEGhtkhEYpuTswwswlcu1R8oAbqYJ1hFZce5wR3gabd0YQGlyLN2itePxEM1CXH67jjcc)

### Sub-Processes
[![](https://mermaid.ink/img/pako:eNp10VFrwjAQAOC_cmQvFZS1glXzsCFaYTCc6BgM60OWXm0wTUqaTor43xe1VTZYXnJcviPH3ZFwnSChJJX6wDNmLLzPYgXulNXXzrAig6kTMHfv17xIQm8zKQpYIRf4jSXMhcRth1Ja6hy5ZGUZ3Cj0ek_uHnrnimmGfF_CGiVyiwnMtcmZ7bR42OCRt2SmRHjFHeP1WcGLSi9WaHXjo4aPjxNV20yoHUR5YevnUyvGTsBntG5g4HsrLCTjCAdhM1g8Tjq_6OKtlYG3rKz71WpY4OFvo4Hfur63WaNKwLkPNCIV_NLj9k6DG72mnL4Gl0HNMIX71CAVUtKHYDSIhv5_qt-oQRj6YZ90SY6uOZG4JR7PNTGxGeYYE-rChJl9TGJ1cq4qEmYxSoTVhtCUyRK7hFVWr2vFCbWmwhbNBHO7zxt1-gErwaun)](https://mermaid.live/edit#pako:eNp10VFrwjAQAOC_cmQvFZS1glXzsCFaYTCc6BgM60OWXm0wTUqaTor43xe1VTZYXnJcviPH3ZFwnSChJJX6wDNmLLzPYgXulNXXzrAig6kTMHfv17xIQm8zKQpYIRf4jSXMhcRth1Ja6hy5ZGUZ3Cj0ek_uHnrnimmGfF_CGiVyiwnMtcmZ7bR42OCRt2SmRHjFHeP1WcGLSi9WaHXjo4aPjxNV20yoHUR5YevnUyvGTsBntG5g4HsrLCTjCAdhM1g8Tjq_6OKtlYG3rKz71WpY4OFvo4Hfur63WaNKwLkPNCIV_NLj9k6DG72mnL4Gl0HNMIX71CAVUtKHYDSIhv5_qt-oQRj6YZ90SY6uOZG4JR7PNTGxGeYYE-rChJl9TGJ1cq4qEmYxSoTVhtCUyRK7hFVWr2vFCbWmwhbNBHO7zxt1-gErwaun)

[![](https://mermaid.ink/img/pako:eNp1kE9vwjAMxb-KlV2KBBLtoJtymDRRduQwpl0oh5C41CJ_qiQdmhDffWEUbvj0ZP_sZ70Tk04h46zR7ihb4SN8VbWFVKHf7b3oWvhGTw1JEcnZ64hU_pxtPlES_iCs8Air3uzQh-2Icx6cQalFCAVMJm8XeJYtWpQH-CCNAd73gmxIRmg6LSKO7kdnt4V5tlmjVRAdLDShjdsBSs2r-DeosIG7Ww4Nac2f8tf58mX6iCoGal6W07JgY2bQG0EqRXC67NQstmiwZjxJJfyhZrU9J67vVPp1qSg6z3gjdMAxE310618rGY--xxtUkUjJmYE6_wFxoHQw)](https://mermaid.live/edit#pako:eNp1kE9vwjAMxb-KlV2KBBLtoJtymDRRduQwpl0oh5C41CJ_qiQdmhDffWEUbvj0ZP_sZ70Tk04h46zR7ihb4SN8VbWFVKHf7b3oWvhGTw1JEcnZ64hU_pxtPlES_iCs8Air3uzQh-2Icx6cQalFCAVMJm8XeJYtWpQH-CCNAd73gmxIRmg6LSKO7kdnt4V5tlmjVRAdLDShjdsBSs2r-DeosIG7Ww4Nac2f8tf58mX6iCoGal6W07JgY2bQG0EqRXC67NQstmiwZjxJJfyhZrU9J67vVPp1qSg6z3gjdMAxE310618rGY--xxtUkUjJmYE6_wFxoHQw)



### Decision Consequences
- Python tends to be a slow language when working with databases which can impact the programs overall execution.
- If it has to interact with the database, it may have some issues and not have smooth interactions if the legacy data is too complex.