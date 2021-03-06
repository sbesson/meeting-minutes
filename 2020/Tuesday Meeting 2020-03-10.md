Dundee: - remote only

Remote: Will, Ola, Simon, Mark, Frances, June, Melissa, Kevin, Wilma,
Liza, Seb,

> Jean-Marie, Josh, Chris, Emil, David, Jason,

Start: 2:00 pm

1. Accepting minutes from [<u>last meeting</u>](https://docs.google.com/document/d/1rwSm8XINFrAqg5jrXzDGJvBwHtehjYISPbSi00ahu4Y/edit)
-------------------------------------------------------------------------------------------------------------------------------------

2. Project Status
-----------------

(2-3 minutes each)

-   IDR

    -   All extcloud05 VMs will be switched off tomorrow (includes VAE,
        > FTP)

        -   Maybe at 16:00 ?

        -   No ftp upload available.

        -   No idr-testing server available

        -   If you want access to raw data, copy to dundee

        -   Probably no access until late March (23rd) or early April

        -   DNS redirection? Temporary tenancy outside Embassy where
            > idr.openmicroscopy.org has been migrated

        -   Jason: plan for idr analysis and other URLs? Redirects?

        -   Simon: could do. Seb: we have a static maintenance page?

        -   Find / prep a page for tomorrow.

    -   Provision for testing resource? Problem not an option as they
        > gave us the only external IP

    -   IN P

    -   idr0077, idr0064, idr0070 are priority for copying to Dundee so
        > we have access.

-   Next release

    -   Release is set for March 25th giving us two weeks remaining.
        > Next steps? Perhaps build and deploy a release candidate that
        > we can use for final testing?

    -   Josh: no one knows ALL steps to releasing since de-coupling

        -   Updated release cards since de-coupling

            -   J-M: card added for artifacts doc deployment

        -   Rc1 build testing.

        -   Release template:
            > [<u>https://trello.com/b/gUTby8cp/omero-release-template</u>](https://trello.com/b/gUTby8cp/omero-release-template)

-   SA (learning/mail)

    -   Local networking issues

        -   Whois hanging on local box - network related?

        -   Wait for network issues to be fixed

    -   Jason - Thanks to Simon for GPFS licenses work

-   Glencoe

    -   Release prep

    -   Bio-Formats 6.3 & 6.4 release schedule setup

    -   Webinar next Tuesday

    -   Bio-Formats bug-fixes open

-   Community

    -   OME meeting. Invites going out etc.

        -   Current [<u>Draft
            > Agenda</u>](https://docs.google.com/spreadsheets/d/1qbkkBvpSzv2adT4uNMcJmv12KPlp5I3yv0Hxl73O3Gw/edit#gid=0)

        -   Chris: drive /showcase advanced implementations using our
            > stack

        -   eg. non-publishing workflows.

        -   First day focused on public data while second day would
            > focus on applications

        -   Workshops on the latter part of the second day or the third
            > day

        -   Need to decide soon if we can go ahead, re: Coronavirus

        -   Possible to organise a “remote” conference?

        -   Josh: more days for fewer hours if remote.

    -   Paris workshop (la Pitie Salpetriere)

        -   Workaround for group import. Data imported as sudo into
            > private group with all the people followed by a chown
            > operation

            -   Raises the question of exposing chown in the clients

        -   Light admin solution was not acceptable as the server covers
            > different core facilities of different modalities

        -   Chris: based on experience, this workflow will fail as soon
            > as too much data is transferred. Almost if not more
            > intensive than running an import.

        -   Need to look back into this problem and thinking how to
            > solve it.

        -   In GS experience, the usage of cron-based command line is
            > highly recommended for this type of workflow.

    -   [<u>https://github.com/zarr-developers/zarr-specs/issues/50\#</u>](https://github.com/zarr-developers/zarr-specs/issues/50#)

        -   Goal is to define the terms of the JSON to specify pyramid

        -   Seb: turn-around -&gt; spec?

        -   Josh: more like community agreement at this stage. Hopefully
            > usable by end of the month. Lots of community momentum
            > just now.

        -   Chris: don’t try to do too much at once

3. AOB
------

(5 min. max; tech. Discussion should be highlighted to relevant people
and rescheduled)

4. Main Topic - Navel gazing (14:46)
------------------------------------

(20-25 minutes plus 15 minutes questions max)

### Communication

-   High-level issue: OSAR feedback - communication / tracking issues.

-   Daily Morning chats e.g. for recent py3 have been useful to
    > coordinate team

    -   Monday’s idr meeting - lots to discuss. Maybe better to deal
        > with during the week.

-   Lots of effort put into external support. More than on internal
    > communication!? Rebalance somehow.

-   Josh: morning chats useful for big topics.

-   Mark: daily morning chats weren’t needed for sv work. 1-to-1 chats
    > in office often sufficient.

-   Josh: idr progress on datasets may be faster with more frequent
    > chats.

-   Frances: can chat during the week if urgent. On Slack ‘discuss on
    > Monday’ etc.

-   JM: can schedule morning chats as needed for after standup.

-   Frances: 1-on-1 discussions are easy to arrange. More is harder.

-   Simon/Mark - too many meetings at various times does hurt
    > productivity.

-   Mark: various questions e.g. “what’s at EBI?”, “what are the
    > spiders?”

-   Jason: Chats - want others to know what’s being discussed so they
    > can join if interested.

-   “Friday topics” - e.g. 2 hour training on various topics.

-   Simon: we did this a while back on Tuesday meetings.

    -   Josh: worked for a while, then we all got busy and they got
        > dropped

    -   JM: zoom presentations have worked in past. Recordings etc.

    -   Mark: training materials to come from these have been useful.
        > Eg. Ansible.

-   Jason: do we want to make a list?

    -   JM: e.g. Illastik integration.

-   Jason: where is the list going.

    -   JM: Presentations 2020 gdoc.

    -   Jason: Team meetings folder. OK.

### Calendaring

-   UoD now uses office365 for everything.

-   Jason: tricky to unite this with google calendaring.

-   Need to move calendaring to office365. Already have e-mail there.

-   Trying to port google OME calendar from google to office365.

-   Need to move individuals to office365.

-   Good zoom and slack integration in office365.

-   Annual leave etc added to you \*own\* calendar.

-   Good tool for scheduling meetings

-   Can use browser (Mac / Windows install only)

-   Josh: what about Glencoe?

-   Josh: created OME team and added members.

-   Can invite OME to meeting. Or invite individuals…

-   On Desktop - create meeting on OME group - get to see who is
    > available when.
