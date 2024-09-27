_**For ease of reading, I'm going to break up sections with comments.**_

flowchart TD

    A[Copying An Optical Disc] -->|**Check Disc Type**| B(Choose Disc Drive)

    B --> C{DVD Drive}
    B --> F{Blu-Ray Drive}


    C --> D[**CD**]
    C --> E[**DVD**]
    F --> G{**Blu-Ray Disc**}

_**This is the section for copying a CD.**_

    D --> H[*Open Exact Audio Copy*]

    H --> I[Check for track gaps]

    I --> |*This is blank time between music tracks*| J[Adjust file tags]

    J --> |*These are how music software gives you album covers and track information*| K[Test & Copy Selected Tracks]

    K --> T

_**This is the section for copying a DVD.**_

    E --> L[Open *MakeMKV*]

    L --> M[Select the Disc Drive]

    M --> N[Begin choosing DVD titles]

    N --> O[Select *'Make MKV'*]

    O --> T

_**This is the section for copying a Blu-Ray disc.**_

    G --> P[Open *DVDFab*]

    P --> Q[Select the subprogram *Blu-Ray Ripper*]

    Q --> |Program begins selecting the main title automatically| R[Manually adjust output format]

    R --> S[Press Start]

    
    S --> T[Program outputs media files to destination folder]
    T --> Z{Done.} 

* First and foremost, an optical disc is a digital disc that has surface marks containing data that is read by an optical laser.
     * I was preferring to use // to indent comments, but GitHub did not like that and it would make the diagram difficult to import so I opted for Markdown instead.
* It's important what drive you choose, because each disc type has a unique laser required to read them. For the sake of this diagram, the DVD drive has both a 300-650 nm laser (DVD) and a 780 nm laser diode (CD).

1. A CD, or a Compact Disc, is an optical disc format that is primarily used for storing audio media, particularly music. It uses the most 'crude' laser type of the three main optical discs described here.
2. A DVD, or a Digital Video/Versatile Disc (both are considered acceptable), is an optical disc format and standard released primarily for video content.
3. A Blu-Ray disc is an optical disc format made to improve upon the DVD. It uses a blue laser, rather than a red one, to allow for more fine data structure on the discs, which allows for more data to be stored.