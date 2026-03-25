# Fernandez-Cervantes Family Tree

```mermaid
graph TD
    %% === FERNANDEZ SIDE (Father's) ===
    
    %% Great-Great-Great Grandparents
    JT["Juan Tamondong<br/>~1850 - deceased"] --- JT_JP
    JPag["Juana Paglingayen<br/>deceased"] --- JT_JP
    JT_JP((" ")) --> CT

    %% Great-Great Grandparents - Fernandez Line
    PF["Pablo Fernandez<br/>~1875 - deceased"] --- PF_MV
    MV["Marta Villanueva<br/>~1901 - deceased"] --- PF_MV
    PF_MV((" ")) --> MaF

    %% Great-Great Grandparents - Daquigan Line
    DD["Domingo Daquigan<br/>~1880 - deceased"] --- DD_BB
    BB["Benita Bacarro<br/>~1880 - deceased"] --- DD_BB
    DD_BB((" ")) --> VD

    %% Great-Great Grandparents - Abalos Line
    JA["Jose Abalos<br/>deceased"] --- JA_CT
    CT["Carlina Tamondong<br/>deceased"] --- JA_CT
    JA_CT((" ")) --> HA

    %% Great-Great Grandparents - Rosario Line
    FR["Francisco Rosario<br/>deceased"] --- FR_JG
    JGut["Juana Gutierrez<br/>deceased"] --- FR_JG
    FR_JG((" ")) --> FilR

    %% Great Grandparents - Fernandez
    MaF["Mariano Fernandez<br/>~1905 - deceased"] --- MaF_VD
    VD["Victoriana Daquigan<br/>1917 - deceased"] --- MaF_VD
    MaF_VD((" ")) --> BF

    %% Great Grandparents - Abalos
    HA["Hilario Abalos<br/>deceased"] --- HA_FR
    FilR["Filomena Rosario<br/>deceased"] --- HA_FR
    HA_FR((" ")) --> ARA

    %% Grandparents - Fernandez
    BF["Bienvenido Fernandez<br/>1933/1937 - 1994<br/>📍 San Carlos City → Chicago"] --- BF_ARA
    ARA["Aurea Rosario Abalos<br/>~1936 - living"] --- BF_ARA
    BF_ARA((" ")) --> RF

    %% === CERVANTES SIDE (Mother's) ===
    
    %% Grandparents - Cervantes
    DC["Diosdados Cervantes<br/>deceased"] --- DC_NC
    NC["Natividad Cabrera Cervantes<br/>deceased"] --- DC_NC
    DC_NC((" ")) --> JC

    %% Parents
    RF["Raul Fernandez"] --- RF_JC
    JC["Janice Cervantes"] --- RF_JC
    RF_JC((" ")) --> AF
    RF_JC((" ")) --> KF
    RF_JC((" ")) --> KiF

    %% Children
    AF["Adrian Fernandez<br/>b. Mar 2, 1987<br/>📍 Allen, TX"]
    KF["Kristine Fernandez"]
    KiF["Kiana Fernandez"]

    %% Styling
    classDef living fill:#90EE90,stroke:#333,stroke-width:2px
    classDef deceased fill:#D3D3D3,stroke:#333,stroke-width:1px
    classDef current fill:#87CEEB,stroke:#333,stroke-width:2px
    classDef connector fill:none,stroke:none

    class ARA,AF,KF,KiF living
    class JT,JPag,PF,MV,DD,BB,JA,CT,FR,JGut,MaF,VD,HA,FilR,BF,DC,NC deceased
    class RF,JC current
    class JT_JP,PF_MV,DD_BB,JA_CT,FR_JG,MaF_VD,HA_FR,BF_ARA,DC_NC,RF_JC connector
```

## Legend
- 🟢 Green = Living
- ⬜ Gray = Deceased  
- 🔵 Blue = Parents (status unknown)
- 📍 = Known locations

## Key Dates
| Person | Event | Date | Location |
|--------|-------|------|----------|
| Bienvenido & Aurea | Marriage | Dec 16, 1963 | San Carlos City, Pangasinan |
| Bienvenido | Death | 1994 | Chicago, IL |
| Adrian | Birth | Mar 2, 1987 | — |

## Confirmed by Records
- ✅ Bienvenido's parents: Mariano Fernandez & Victoriana Daquigan (FamilySearch marriage record)
- ✅ Aurea's parents: Hilario Abalos & Filomena Rosario (FamilySearch marriage record)
- ✅ Marriage location: San Carlos City, Pangasinan (FamilySearch)
- ⬜ Cervantes side: needs research
