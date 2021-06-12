# Stock Data Group Sorting Problem

Stock data is present in a SQL database.

User can search the stocks either by symbol or name.

1. Upon receiving the search text
2. Check stock symbol or name match
3. The matched result set should be grouped sorted based as below
4. If multiple hits are found in a group, they should be ordered by `Name` then `Symbol`
   
###### Group Sort criteria

    1. Symbol exact matched records
    2. Name exact matched records
    3. Symbol starting with search key
    4. Name starting with search key
    5. Symbol contains search key
    6. Name contains search key
    7. Symbol ending with search key - mostly covered in 5, 6
    8. Name ending with search key - mostly covered in 5, 6

### Assume the below table. (Not realtime values)
When user searches with 'nio'. 
Result set should be like below.

1. NIO - NIO Inc
2. NIOBF - NioCorp Developments
3. UAN - Nio Stock name starting with nio
4. UNIOU - Stock symbol with nio in between
5. UNIO - Stock symbol with nio in the end
6. OG - Onion Global 
7. UGHL - Union Bridge Holdings

### Stock Data

Stock Symbol    |   Stock Name
---             |   ---
AAPL            |   Apple
AAC             |   Ares Acquisition
AACE            |   Alexandria Agtech/Climate Innovation
AACG            |   ATA Creativity Global
AACO            |   Advancit Acquisition I
AACP            |   Aeon Acquisition
AACQ            |   Artius Acquisition
INTC            |   Intel Corporation Common Stock
GOOG            |   Alphabet Inc.
APPL            |   Apple Inc New Stock
NIO             |   NIO Inc
NIOBF           |   NioCorp Developments
OG              |   Onion Global
UGHL            |   Union Bridge Holdings
UNIOU           |   Stock symbol with nio in between
UNIO            |   Stock symbol with nio in the end
UIN             |   Stock name ending with nio
UAN             |   Nio Stock name starting with nio
