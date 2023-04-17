# utl-setup-notepad--editor-for-use-with-wps-altair-sas
utl-setup-notepad++-editor-for-use-with-wps-altair-sas
    %let pgm=utl-setup-notepad++-editor-for-use-with-wps-altair-sas;

    Setup notepad++ editor for use with wps altair sas

    github
    https://tinyurl.com/3w2vwp48
    https://github.com/rogerjdeangelis/utl-setup-notepad--editor-for-use-with-wps-altair-sas

    Go to this site for instruction to install notepad +++
    https://tinyurl.com/wznt7d2y
    https://blogs.sas.com/content/sasdummy/2017/08/25/npp-with-sas/#:~:text=In%20Windows%20Explorer%2C%20right%2Dclick,Always%20use%20this%20app%22%20check

    Just replace the SAS executable with the WPS executable

    "C:\Program Files\SASHome\SASFoundation\9.4\sas.exe" -sysin "$(FULL_CURRENT_PATH)"
    -log "$(CURRENT_DIRECTORY)\$(NAME_PART).log" -print "$(CURRENT_DIRECTORY)\$(NAME_PART).lst"

    With

    "C:\progra~1\worldp~1\wpsana~1\4\bin\wps.exe"
    -sysin "$(FULL_CURRENT_PATH)" -log "$(CURRENT_DIRECTORY)\$(NAME_PART).log"
    -print "$(CURRENT_DIRECTORY)\$(NAME_PART).lst"

    If you edit the following program located at c:/ut/opts.sas

    proc options;
    run;quit;

    The log will appear in c:/utl/opts.log


    1  The WPS System        10:23 Monday, April 17, 2023

    NOTE: Copyright (c) 2002-2019 World Programming Limited. All rights reserved.
    NOTE: World Programming System 4.02 (04.02.00.02.007562)
    NOTE: This session is executing on the X64_WIN10PRO platform and is running in 64 bit mode

    1         proc options;
    2         run;quit;

    Portable Options:

     ALTLOG=            Name of the altlog
     NOAUTOSIGNON       Remote submit will not attempt to automatically signon
     BASEENGINE=WPD     The library engine to use when BASE is specified
     BOMFILE            Write a Byte Order Mark prefix on external Unicode files
     BUFNO=1            Specifies the number of buffers used by a library engine for a data set (not
    honoured by all engines)
     BUFSIZE=0          Specifies the size of a page for a WPS data set
     BUFSIZECMULT=6     Specifies a multiplier that is applied to the computed minimum size of a
    page for a compressed WPS data set



    There does not appear to be a good windows command line editor. I did try SPFlite.
    Ultraedit is time limited and I could not figure how much it costs for personal use.
    I think when any software is purchased with taxpayers money the cost is public, FOIA request?

    Roger


    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */
