# THE-HUNT

## Statement Of Pupose

We would like to create a gaming application for NWMSU which works on iPhone SE, Android device, laptop and an iPad. The main motto behind this idea of creating a gaming application is to bring bearcats of diverse departments onto a common platform which helps students to interact, encourages students to unique and special parts of campus, contributes in developing an attitude towards teamwork.

## Overview

We would like to create an app that can be played on a mobile device. The app would encourage players to complete a 'quest' by encountering a specific list of locations. A player would activate one of the locations in the quest. To score that location, the user must enter the geographic area (as determined by their mobile device). Locations may be explicitly identified (easier) - or described using clues (harder). The quest may require locations to be accessed in a specific order - or in any order as specified by the quest creator.

## Benefits
Improves the ability to think in logical way.
Handling difficult situation with team effort.
Thinking out of the box.

## Roles
* Project Manager - Pruthvi Naskanti
* Back end Developer - Deekshith Maram 
* Back end Developer - Bhaskar Reddy Minupuri
* FrontEnd Developer - Ravichander Reddy Goli
* Database Engineer - Harika Kulkarni
* Test Engineer- Sai Rohith Gorla

## Entity Relationship Diagram:
![title](https://github.com/Dixith1196/THE-HUNT/blob/master/ER%20Diagram.png?raw=true)
### User Entity: 
The User entity has 4 attributes namely:Username,Email,Password,Date last accessed.It stores the username,email,password and last accessed of the user.
A single User may be into one team or multiple teams.User may create and manage a team or join a team and particpate in the quest.

### Team entity:
Team entity has 6 attributes namely:Team number,Team name,creator,Date created,Date last edited,Username of the team members.
The user serves as captain of any team they create and he provides the team name.

### Player Entity:
This entity has two attributes:Player nickname and score of the player.A single user can play with different nicknames and score accordingly.

### TeamPlayer Entity:
TeamPlayer entity is an associative entity that maps between Team and Player.
It contains attributes DateInvited,Date accpeted Invite,date rejectedInvite and Dateleft team.
The captain provides a list of emails of invited members.A user can accept the team invite and become a team player or reject it.
After three days, if not accepted, assume rejection.

### Quest Entity:
This entity has 4 attributes.Quest name,Designer of the quest,Date created and date last accessed.The user serves as designer of any quest they create and they 
provide a quest name.

### QuestLocation mapping:
This entity consists of 2 attributes.Quest name and Location number.

### Location Entity:
This entity consists of Location number,Location clue and Location coordinates.The designer provides a list of locations for the quest.

### Competition Entity:
This entity consists of CompetitionID,Competion name,creator,date created,start time and endtime of the competition.The user serves as the hunt master of the competion.
The hunt master specifies the start date time and end time for the competion.

### CompetitionTeam: 
This entity is also an associative entity that map teams and competitions.It consists of 3 attributes:Competion ID,Team Number,Team score that stores the scores of different team members.


# Sample Data In Excel of Each Entity
### Sample Data Of the Player
![Sample Data Of the Player](https://lh3.googleusercontent.com/GPyYeVyruZ69-vpg4aw7w6Qe2m0XobY4NOtJMVkUUdcN6Oezi1TF93MEycEiQCV8T_cbMAS9dbsZo93qkZlPD2VLn6bnWkY6N6IItO-10lyGpIk_9768FwM-yzhUb9LVfQuu74uCZiv33N2_KgE07eULjc21EpzdICtq9mbNOpkjPRXySmBT5hVdGkLGXWGxRX4ZfyT59ZZ1QzMmSTgNJBM6U9kqlvH09NfOTjIc5dr8BAppIESYYk7d5msWoWK0PcvinlHu2ebVilk5h8vrlXWKP2kGNECB_wRhYB1ZbjvhxOqmReUX36tDtl5xTznwvcHkjKPV3o4KNUoxFo0m6Z1b0YpOqjANRyw0ztLSGkE0KRxiD0mGMm0ukeS3ZKxYD-3_b5fypBwehcAxuR50wIxmOFlJZohP9JZxgdSwzE9U7v9lYHI9K39-28GgUE74IE8JWluZDOBRC0NG_ClETQum3cZ92ya4WCyW70QTBsFjSKVM-ozOWznK1w5rchmyaC32UWubX-TRKLCvVYaIR1Zve7aO_13YvYbyq16ftuemAorqrWjeLnGHEjVndK41SDOa7PioKjk6oRT0t2MGbT3iUBR5wNM5QklyqwzDM976LnqtfIxuFwOYv4dFsbHuFp07RmOG75xUg4iQVKG6qywuEHRsGBxM9qdGNGcfic2IcP7HOexL9Pz8BY6SJA=w1169-h657-no?authuser=1)

### Sample Data of the Team
![Sample Data of the User](https://lh3.googleusercontent.com/_W-uekJY9Kg3ocnloMzRXjsvDEsayYHFGOETRrXkT846mri9vuM0Y0bP4lFeL6J8pcRCxpEt1ybW3D6DaAiawzipt9-0XXjKzbf0Km8LX2U5rXJck6kdnXEqT_SA87AtCB1TfalMdyg_WYzmat_HMICvdL6YxYr2rZ_OYj4iANPArt37KDyCFjigswYiiWKFxQcVrgEtMB6esNIYKJoikomGEptqEmOdxrt0_gpXJxoAgk_BbY7sA8gul_kZP6YNIvizzRbA9sGy-cqDY6o0GfEWJh5gRtAXKNNVGH29LqU0j3ZAsAUpByt5_qJh_kLnbLZwnE-l1i5j6d_ZGQK1xHKSaPyJRr9kL-9mlA97nb-aWsoo-OOVPq2zrYXgvlPOejdY6EqGLQmppfvSYzxzpgZk5NxfiYL49aDntFa-rOaX9pf5rA-K1ZWaVyLLz_r9cZdsFTf7JJmmMP4bLcheAX3PzP8tSv93MNXg2l_Mp9Z2K3sy_POEvgk0YRsQ9qGcLeA1RApjSY-U9zBD6U_Pzp-GSARPbf7w0323N6_-WlT0ZXipPNaUo_y3fCPMPMw-LMQsenhEnd0yceeyor7UY1bBMylEBN_k_TQAC-ceFUqXul8HyJQNCMSblbetVYgYIet_j9dSyMUK43dI_i5qFWPxYY2S3mUw6pUFKl_OJcVW8xCgbPIfOetypGsuZA=w1169-h657-no?authuser=1 )

### Sample Data of the User
![](https://lh3.googleusercontent.com/zrQ4ts2QWuSGKNy3R4VhCV26lNY56ywlQBsdx1ZhSA1KYZSnIrS9mRsb3L_FqJ58oI-NIBskgTf3MLOOiVmEqW4kQeFj3WOGYTFeGLIQkcT-MD4fVRGdJoCAt-I_u10VVQiFKZG9S02G-8ujB8mMZ8KB1tU3M7dTIoxK9r0iDyys2Ot6MCZk5Fvn8lKytZ828kWW-t07UBJSY9II0V1iSo8dpef9QO5uElxX4irJmAV94Oa6tXPrmahwdz4cjEWhlh27URoMRD1kBTo84Zrinbbq1LQBFlvu_cdXMRZrlQPaDvyPYFjib0EmEK52lHTDNueQDR-fvaW2Gc8Nc1fDmu12Up9UtU5W5Sce6db59wEgvi_8VGRuEnOt9tdTKKh1gJTJa8wX10FRPryYGOcRm-uGeCv7Ws-t33er3ZRhgcxF_TtxVHY5_VnTI8mWNf_3Qeo4wrIuFX_cCfqw66xwH6jNe4L5xqawxKc4p_mtbIf8sjab6jXiaXpLbt77KGe7d8wKiNKv5DmA_Rmbxs7BUVSJs1JYiVmgk8eDyk2_BkDwrDJpwxuTQs6s2vd_JQaPdKR6hQEBJ291ikRk-hfenuN7VhfKxp4f2B_ImG7TsrpPuZCjGY6LynwEATXrRqBJKKDilKeeOu2QncdKVk2gV04gw6wtCvUReS9v4-RdIhn87zcTQPd4rwh-CW9IKA=w1169-h657-no?authuser=1)

### Sample Data of the Quest
![](https://lh3.googleusercontent.com/-8KoxxuPXrKB0PYw5Rvo6yffNuFU1FRB7ogdJ7sYUMpdi_oEqFcq9rc16_wC03yoZdLI4P7cTnNHAXyGnB2TNEmhgWdtw8Mc3IPLKeOHa-IkSQoWJZu-09td68O3BCDYjjw7U1gDaVbg1ejax6v5NUoOBWN_L1cU1al0lHsrjEhycPVAhTJbfq5YKXZn4owAnbq_J1-i8vTR2MX1vCWLPCRwi4trKXRsMivcGSd9pcvEwZWLC49jLc-ac1SVGjaTzmdIjyWHgSmDFJ86SAe-CsUlVVuK1ZVsXgYOsaXYeS3reOVLayxl-LaytflRvvF9d8KKlhbhcMagpNJIEzwwX8KrxsfWpSk4EVPz0Pi6ff5vAiKVEAeFf9lKTXGgiGahu4erNKf2hs3qq_OzKh_k0yTzr_cvBhuursi5tPfg3JZE4N6WKd6YqY3LThv5oFxvlRlTNlDN4h-G6P_LF6WGX3LRThjzpGtOKbVIiIBJEM9PB8Bj4mC0luhf1pJB_OcCn61fm1CXEuQdfGueN3nbKRE6zIpF2_QYXj7zjlMS6W7Yuebepove_eGgPDny6RH-IZ98FMCRpL9ajF0hjBfKtJDhuTRw1L6xO1dweTU1lukcgiXYaoVBU5UFfDXUTHnMMKg5bXVR8nY4RUdBshb9tu7p6xxoBNktPIBCCxe1itPzxOJoWgbOZaIBkRfNDQ=w1169-h657-no?authuser=1)

### Sample Data of the Location
![](https://lh3.googleusercontent.com/Lwpr82YUkn7vMbjjnZAjW5_dW4iFgB0WXjPHNaHEWY34iZ3ZVOynGgIpQoCaBt8w5_ty91AJ7n1TH2GdJOryJ5T-A7A-HXJzeuFFtqIBk55yH1JYYczDQJlILvX886xO8mzTH0DpRJEHAxhGvU-Y9Pn1_35fFSZ7IxfO4mnyd-34IDVz6nryzFr-W9fFl3QDrqMHD81kJ8pD0Q69zPWUmgH36p2SBLC3WVLs4dk1zXrqi274ViNr-_2cGUpqnKENkhbfZK9jKjGZXkCFYjj6pcy4SfmhNPlMplWHKy6KGXjL2kTlq59EX_qcFysky5m1jbH-8WrzBlMj3Kv2xWFyjtfqK7CR1St17ygsFIqumnXz2VW4mH0Hw5yacumR24Dc8-SK7bbGiYXOxixGNUAC_RcN20QvcaoIrEPtBvxgI8U8r7F7xavLMMXK4DTsYN3eaymvdOn1Fmf8dfvInpJ48i6oUf0QiOQhYsi5DviZ3QsUZXHXVmKvhVrxZc3h8ZYvpqGUsE0rIbkWtRevCEZk1H2uykZ2RsrDNN4XvXX4Mf6DlLNITfE-C-nHZNADl3sHDCDroyxCjQGl4r9DMN0bAPwIez1JHt2FrkjKGpL6-GQLRo-aazDEaXvqLRVoCU2grA5XzUiJCTpAOerHOCjZXwgZ8AnUbAD3Sy42UnNfvoztDGDaPr3gqtQyPenfog=w1169-h657-no?authuser=1)

### Sample Data of the Teamplayer Mapping
![](https://lh3.googleusercontent.com/rtqntpex_43wsx4qFO9XkwxEU0ID8R_Pnx5-Z3VEV8abv1QJ5U4hHYBsFUTSyQf7gqp3X3A37YFGeOSQ76WrtDhV89OAiDlLiZld5_8LCNqFdr7QUIyKMGsR4EjlfQyT-c7rP0-YglAm8hwYKbGiQr-wQRSd9uDxyjx-a0SfvcztPHqA_cQlXrr6NWElLhJQwxNSil-_UO_Epk62QTA6asdtyenHc_MJhR_VNcJmqXzydRQuWpCGI_l_Au7z5QaWCESmxQbuKi6cyEylUb5YxlMm5pNnlfQkonVO8AVUk6K_pDNVGWtTJT6mY4wArRAZ6QN3_F4VGC1o691GLTvxL4rg2Tc-QlkDWqayRoTxmqWF2nK04QTIdzg8ZG0hqBCFEOdJazARLCI3Mp-bOb57PpRahwso9NIJvykYgdhUrRBL3xXRM2oJoHdsTG4ePQtf7jXvj71v_hQZUf26F-eiVYEFzdBocaGEEdkjn4WQ7-bCnvHCmkf-vck5dlthfqPgqSk-A1rWhuF5YmcsRSt5sJFq7iK0d2HC6gMFdtwgop3fVE7yQXagKRkcA9lAgqogslylwM1czhQ3bISmywRoKN90Q54immHVnH9ayz_srdknyLuwg6cq_CgXrClnXE7UvC-fp0UEEDKcJ2W0MQ7YlCcH_UP1Jrdgbm0oudNPcH0a0bPZ-fK6KLOqd4efCA=w1169-h657-no?authuser=1)

### Sample Data of the Competition
![](https://lh3.googleusercontent.com/Paoj8em6Ob7ovSOPCrKIlFN2txJ7kBhObTcA2xBTUR_U2LuAiayoWqqyR4MmQ_LglcV6IhE3arnnW6lQ0g_QHg2noNxcO7Zc0DDcAktuCpZuvmcjvCBLMmm9-p9Y6oUAuMgnaUo5aO-iEwYVMTjG66unDl7-t2wLkGE2gLQOHt97WZE61Dwcbd4ajU8FlaiOjoO-pxYQAkfTAWNB36Ln4HuBnxeeMpZiqGt1oMRjetwcx7k9DxTQSB-2d9NHVpjNxF3REsDF5IUSrHaC8Ixkp03S-pOk77mcmFMUM_TqbwD_0VnvjqDXi17ASSmjPcnRH6hg5RJHCU5Acc71fyTy3XAoIkFDNmek24bMU8tcL25bnDCknUwW1znlG8pU8VWxssNlfff_PW00qqkqiwqVeNMIG4a0RG4G6iQYr8yT4r9QQQcqa70nc6TOuR9pN8VNlanoOkZqsPL4zTOOZTL3Cz4VKR8QRu8nrAJ9chuR5M0WA4T2dDz3DveW2IL5JOZVSvCJrjkIQYHAIdiXdRPH6EOto8Xsh3uc5IwOOtu3nwujkYAK4o5Psyri20WzgAMVwlHa25maR4cazjalcWfeySRDBmDLavn56_FaWI4n_l2ZkEzEOXeXw1JrRJhfG1PN4af89SIEbAGAPQq-oW5HqzS2yt_s5PKQ5ZT6aYO7iRa7HJq00eD9YEhYvPel0A=w1169-h657-no?authuser=1)

### Sample Data of the Quest Location
![](https://lh3.googleusercontent.com/Qy-NmcVsjGULbIWkV3sO0K0ifCFn7c6Nh8VfUNaGUBfuVbl0tGvVcXwTd-umjJHfbh9QPZvEUkpE8wqhzE2dNiwXOfj2nMkdTT8yqjOrW2EV1T1qmQuMOoEVSScX_hGFulIKZ9FetV_wvah9pXinyagfvwQkhWcTvZWaDuQo8kV3xVEKvkkROb3ahRFJ2AocILokKFJXvIHpwm4AEkSqSnNCowlkcSjAx9xSVP3iT0VQZ2lhwo8xsV7-mFj0sjSV2LK-aMfFPajOfki2dIjHfrLBnrMYRXMQMnYw8G814_Wcqs23SSjyoxR3RMj67UwGm9_OuK7k1IS4F3hIcYCQrxgJaAmvHcz6aYvK5AfWXhUX3WCIhwsFuFcavZ7W5Di4QRWPLeg1QPb4x8MZf4e6BZqhxAyem8t-m-gZi6uyKTJMJyIoo7NPx3x4GMBjVRgsByN5ibGLg33O8oCVEKbTkQjrNatIygRFuPrDob9Br5tVt0b62CI87tYZFghjhculAZYDvV5-GED2Aw_1txKC2nQ6ncpoI-pW0i-YdI7su1GMhQAG6pSfj-hbee7-Hn2YT0bQfvOwPkZ_3dPkjlQaOFkLMe6L2Wqh9eLhFFRpWs_lU28oH7YxFib_caCZRf07oEb_jMq7pQ_fP2lCqac3Ijoai1YUx2ao6mwg2z2WI4vz_1VTM8ZFuV0C5fXVRA=w1169-h657-no?authuser=1)

### Sample Data of the Competition_Team
![](https://lh3.googleusercontent.com/otg9JxrGAgyemcr9UeviKS-L7NmdTHG5M82LVUXBXa9wRavFgJAxfSfncM8fcKSp1bvXUKvmHIp9gVp5sMoufQbs5Jn5WJxJvVcJPapQGkUc34kpbijM2uwwSpioj516hcAJYmfG4Lo9nODtdqQRFwyryvtNoL8CZfTh9_yGpKsMkLmtHLziLb__eCNMTiK4RXhdOxixzm9jrrILQnjmvZCnVMd4hbXH2h8HBDqAfyYIcheyUT7QI6PiB7BZi2U9GBAOZGJwQamP7GX3jWhYgOFmkAhNXsgx5cT9yo_XN_f3kS_dbRCNTcYrVem182Ee41RtJbcStftEFq_GKj8MoU9lbgW0QQqGeroXVdDNOIbpgZ2w9h_3QJKo1U1YU4TRgoxDYkEGBUSklarN5lP58F8j-Z610DGvMsqKG_Bo7N6g1JnjsDmTngvTLddWFwy-8Bo2D6bJSKY-ajAN0lVGzsK10nRQrnxkBLl4FQ2PHpwxfCvLEJa4G43YhRbpQcprkDZ5W41oXbbWRvBJWIzskTEo6sYMrnGL8fOBNELqvFvpVIQYegUQRLbILZWtEeB7TOJGtvuTdMyrVtM8Bte41eo5v_dUCU77BlGcQ5yWSYXiRIuMZ0OCc5mYk3JKvkvy_X3brgxPEQNLYUCl_MNkUNTWzx7Jyxdak2bQ4SigOpZHuTUrgmTqnajjfFzclQ=w1169-h657-no?authuser=1)


# Risks and Assumptions
# Risks
## Risk of Application based security break
Mobile security threats include everything from mobile forms of malware and spyware to the potential for unauthorized access to a device’s data, particularly in the case of accidental loss or theft of the device.

## Risk of location access
The process of poor coding and insecure handling of location data may cause the insecurity in accessing the location.

## Risk in the Operating System and data retrieval
Defects in the kernel code and vendor supplied system code may cause the Iphone or android jail breaks.

## Risk of poor authorization and authentication
Weak authentication and authorization allows an dispute to access the mobile device, or it is anonymous backend.


# Assumptions
## Users must create an account
As a developer, locking out users is much simpler until an entry in the user database has been solidified. But that's almost skillful from the consumer view point.

## Application design must be same as the responsive web design
Although responsive design is similar to mobile app design, there is a significant difference in developing apps for any device versus stand alone.
For mobile devices, consumers anticipate certain interaction patterns and elements of the graphical user interface.

## Symbols can be easily understand by the users
Symbols are attractive and can be visually attractive to convey information. The results will help to analyze clearly which symbol can be considered most effective in communicating the action that we wish the users to accomplish. 


