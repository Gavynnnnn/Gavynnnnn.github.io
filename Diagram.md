\\ For ease of reading, I'm going to break up sections with comments. Remove the comments and this entire flowchart is compatible with Mermaid's Live Editor.

\\ First and foremost, an optical disc is a digital disc that has surface marks containing data that is read by an optical laser.
flowchart TD

    A[Copying An Optical Disc] -->|**Check Disc Type**| B(Choose Disc Drive)

\\ It's important what drive you choose, because each disc type has a unique laser required to read them. For the sake of this diagram, the DVD drive has both a red laser (DVD) and a 780 nm laser diode (CD)
    B --> C{DVD Drive}

    B --> F{Blu-Ray Drive}


    C --> D[**CD**]

    C --> E[**DVD**]

    F --> G{**Blu-Ray Disc**}

\\ This is the section for copying a CD, or a Compact Disc. This format is primarily used for storing audio media, particularly music.
    D --> H[*Open Exact Audio Copy*]

    H --> I[Check for track gaps]

    I --> |*This is blank time between music tracks*| J[Adjust file tags]

    J --> |*These are how music software gives you album covers and track information*| K[Test & Copy Selected Tracks]

    K --> T

\\ This is the section for copying a DVD, or a Digital Video/Versatile Disc, both are considered acceptable, which is an optical disc format and standard released primarily for video content.
    E --> L[Open *MakeMKV*]

    L --> M[Select the Disc Drive]

    M --> N[Begin choosing DVD titles]

    N --> O[Select *'Make MKV'*]

    O --> T

\\ This is the section for copying a Blu-Ray disc, an optical disc format that uses a blue laser for reading more fine pits of data than a traditional red laser can read.
    G --> P[Open *DVDFab*]

    P --> Q[Select the subprogram *Blu-Ray Ripper*]

    Q --> |Program begins selecting the main title automatically| R[Manually adjust output format]

    R --> S[Press Start]

    
    S --> T[Program outputs media files to destination folder]
    T --> Z{Done.} 
    