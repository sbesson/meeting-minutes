Attending: J-m, Josh (notes), Petr, Frances, Seb, Dom, Mark, David,
Liza  
Simon, Wilma, June, Melissa, Andreas, Jason, Chris, Emil

Start: 2:00 pm

1. Accepting minutes from [<u>last meeting</u>](https://drive.google.com/open?id=0B9Xg53EhqUycZEVHclBwRHNFRGM)
--------------------------------------------------------------------------------------------------------------

2. Project Status
-----------------

(2-3 minutes each)

-   IDR (Frances)

    -   Idr0064 ready for import once data migration is completed

    -   Seb: EBI is performing final data checks of the migration.
        > Hopeful that we will get a green flag this week. (Needs
        > reforwarding…)

-   IO (Josh)

    -   See ongoing notes: [<u>Chunked 2020
        > Scoping</u>](https://docs.google.com/document/d/1B8EiwJLslNhGeVw1ZahDEcYiI5NJs-8g8rw3t5ZaxEs/edit#)

    -   General outline of a minimal project along with some extensions

    -   Focus is on raw data access, not (yet) rendering, etc.

    -   Last calls for changes to the plan and/or vetoes.

-   SA (learning/mail)

    -   Simon: Provisional quote for VMWare and GPFS license renewals

        -   JRS: follow-up this call with a chat

    -   Waiting for someone to look at seabass server in datacentre

    -   Jason: maxquant server is also down (ticket filed)

    -   Mark: soon (days) will look into step1 of mail migration from
        > necromancer, namely finding the configuration and backing it
        > up.

        -   Plan is generally to move to a new VM, copying existing
            > configuration with newer versions of the packages.

        -   I.e. not moving to google apps

        -   Focusing on postfix, mailman, and apache

        -   Need various SPAM handling configurations needed

        -   JRS: “just” a couple of mailing lists? Fairly chance of just
            > getting it to work (without understanding all the details)

        -   Simon: backups? Chris: last time we looked it *was* backed
            > up nightly via TSM

        -   **Or dropping legacy?**

        -   Simon: why not using google apps? Familiarity.

-   Glencoe - 14:16

    -   Still migrating OMERO Plus instances.

    -   Variety of issues with Python versions (3.5 -- 3.7)

    -   Upgrades have gone smoothly, though some bfmemo generation
        > issues that need nailing down, e.g. memory requirements.

    -   Users moving to Java 11 if not 13. Worries over reflection
        > warnings, etc.

    -   Mark: upcoming questions on pixelbuffer microservices

        -   Chris: easiest to adapt. Brand new since it isn’t part of
            > standard OMERO.

        -   Primarily consumed by internal analysis tools.

        -   Emil: some customers use that on their client side.

-   Community

    -   FYI First “external”
        > [<u>omero-guide-mde</u>](https://omero-guide-mde.readthedocs.io/en/latest/),
        > contributed by Susanne.

    -   OME Community Meeting (see
        > [<u>Notes</u>](https://docs.google.com/document/d/1rSNiTrttVHeeF37DwjvTRSGebwKn_Jco036PS8vaEF0/edit#))

        -   Call with [<u>KI</u>](https://knowinnovation.com/): assuming
            > everyone on the team wants to participate

            -   Due to complexity of handling up to 200 attendees

        -   Zoom Check: most things doable via the standard setup (i.e.
            > non-webinar)

            -   Will need to boost the numbers

        -   Practice with BioImagingUK:

            -   Somewhat smaller meeting

            -   Exercise technology

        -   Updates to web site:

            -   See recent updates from Liza

            -   [<u>https://snoopycrimecop.github.io/www.openmicroscopy.org/</u>](https://snoopycrimecop.github.io/www.openmicroscopy.org/)

            -   Seb: program will need back-linking

                -   JRS: in the past, we’ve updated the program after
                    > the fact

                -   At the moment, can’t even tell there *is* a meeting

                -   Seb: save-the-date would be pretty easy, and
                    > personal arrangements need making.

                -   Liza: will link to the most recent announcement

            -   JRS: question of timing with timezones

            -   Also: zoom video processing isn’t working too well at
                > the moment

                -   Turn-around of many days

                -   Pre-recording may not work in our type of forum

                -   Or some other processing tool?

        -   How to handle registrations? Soon to start.

        -   Petr: someone to test who isn’t a zoom ace?

3. AOB
------

(5 min. max; tech. Discussion should be highlighted to relevant people
and rescheduled)

-   Annual Leave, Extra Annual Leave, Family Leave…..

    -   JRS: difficult time. Kudos to keeping things running. Various
        > things swirling around about partial cuts, furloughing, …
        > Status of research funded salaries? No one knows, but
        > currently being paid.

    -   Looking into Family Leave. Unclear how the university plans to
        > handle it. Continue handling it as previously.

    -   Agencies are discussing extending grants. Again, no one knows
        > the answers.

    -   Lots of opportunities for development. Trying to track things,
        > but definitely things are being missed. Post prominently if
        > you see anything. Chance for OME/GS to make large
        > contributions.

4. Main Topic
-------------

(20-25 minutes plus 15 minutes questions max)

[<u>SV
Retrospective</u>](https://docs.google.com/document/d/12fMqIHoaESYgKu_fsmZ0PIn2SkK7NrIB8fIQ1gPDQbw/edit#heading=h.w8ton6cm0iay)

-   Josh: feedback that artifacts are built sooner. (**timeline**)

    -   Chris: even kernel has source code visible before shipped to
        > vendors

-   J-m: devspace had fallen out of date. Better to keep it up-to-date
    > (**testing**)

-   Simon: push security tests to public after n weeks.

    -   J-m: problem of exposing attacks

    -   Mark: would be good if all the tests were regularly run

-   Simon: optimizing upgrade

    -   Chris: ease of upgrade isn’t the problem, but having
        > stakeholders agree to it. E.g. dev must be updated first.

-   Seb: where should we spend time *before* the next one

    -   Josh: make the decisions when we’re *not* under pressure

    -   Need to dust off the process periodically (once a year?)

-   Petr: the two testing servers were beneficial

-   Simon: use omero-py as the next test?

    -   Chris: hard since nexus config is needed. Need a virtual repo
        > exported to aggregate the deploy repo and the pypi one.

-   Josh: is the modularization of the server a big / the biggest
    > complexity?

    -   Chris: suggest releasing every build as a separate artifact to
        > simplify testing. (Have done that on the GS side.) Make the
        > dependencies looser in the individual jars (5.6+)

-   Mark: Missing steps?

    -   Manual download of omero-web

    -   Staging website update (not in devspace ecosystem) - Seb: can
        > look at that.
