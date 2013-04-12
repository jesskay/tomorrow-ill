=====================================
Tomorrow, I'll...
=====================================

-------------------------------------
A todo-list app for short-term plans.
-------------------------------------

(If you're reading this on the live site, you should probably go check out the
`project page`_ on GitHub. The README looks a lot nicer with its formatting
applied there.)


What is it?
===========

*Tomorrow, I'll...* is a todo-list app geared to my preferred form of planning -
make concrete plans a day ahead. Anything I have to do now, I'll do now,
otherwise it goes into my plans for tomorrow if it's a short-term thing; or into
my long-term plans if it's vaguer, less important, or more of a goal.

To that end, it offers only three views of your lists:

- **Today:** See the tasks set yesterday, and record things you get done
  (anything of note, not just the tasks you set the day before).
- **Tomorrow:** Enter tasks for tomorrow. They should be clear and concise.
  Don't enter something like "finish project", instead enter separate tasks
  for each part of the project that still needs doing.
- **Earlier:** What you got done on previous days. It's good to look back
  and see what you got done, so there's the option to view what you
  completed.
  You may *not* view the previous days' tasks, because I have no wish to
  dwell on tasks I never got done, and the ones I *did* get done will be in
  what's shown anyway.


.. _project page: //github.com/bit-shift/tomorrow-ill/


How do I use it?
================

The app is very small, so I'd recommend just playing about with it and learning
how it works that way, but if you'd prefer to have it explained, here goes:

Overview
--------

Along the top of the app, you'll see 5 tabs. The first 3 are your lists, and
are for the purposes described in `What is it?`_. The remaining 2 are:

- **Import/Export:** For moving your data between different computers, or
  between different browsers on the same computer.
  The data exported is plain ASCII with no meaningful whitespace, which
  means in layman's terms that it can be safely sent via just about any
  plain text method you care to use (email, as a text file, even via an IM
  service if you split it into chunks that fit within the message limit of
  that service.)
- **Options:** This is where you will be able to lightly tweak the behaviour
  of the app if it ever gains features that require options, or clear your
  data if you need to start fresh (though I'd still recommend exporting it
  first, and keeping that copy safe, if you have even the slightest chance
  of needing it back).

Earlier
-------

This is simply a list of what you did on previous days, and cannot be edited.
It's ordered by date, most recent first. You probably won't spend too much time
here.

Today
-----

The meat of the app, this is where you enter your daily progress, and view the
tasks you set yourself yesterday.

The tasks are displayed first, and these may not be edited.

Below the tasks, there is the progress list, where you may enter things you get
done during the day.

Progress updates may be added one of two ways:

- **Adding them to the general progress list:** To create an entry this way,
  click the **+** button at the end of the list, and type in a quick summary
  of that piece of progress. It will be saved and added to the list as soon
  as you press enter, or click outside of the text entry area.  Entries may
  be edited right up until the end of the day, by clicking the **Edit**
  button to the right of the entry.
- **Associating them to a task:** To create an entry this way, click the
  **+** button to the right of a task, and enter the summary as above. This
  will display progress inline with that task, and is provided as a means of
  visually associating tasks to their progress. It is *not* mandatory,
  simply provided for convenience if you prefer to work that way.  The tasks
  themselves are *not* kept beyond the end of the day, so if you wish to
  re-read your progress in the **Earlier** tab, you may want to describe
  your progress in ways that do not require the context of the associated
  task to be understood.

Tomorrow
--------

Tasks may be entered here in much the same way as progress on the **`Today`_**
tab, by clicking the + button at the end of the list, and entering a short
description of the task. This should be:

- **Clear:** Don't be vague about it, you will only wish you'd been more
  specific when you come to look back at the task tomorrow.
- **Concise:** Conversely, don't go into the minutiae of it - you'll find it
  harder to follow if you have to read through too much text to actually get
  an idea of what you wanted yourself to do.
  If you find a task becoming too long, consider only including the details
  you *need*, but are unlikely to remember; or splitting it into smaller
  tasks if there's more than one part to it.

You may edit a task at any time before tomorrow, by clicking the **Edit** button
to the right of it and changing the text.

You may delete a task at any time before tomorrow, by clicking the **Delete**
button to the right of it. Please note that this cannot be undone, and will also
prevent a recurring task (see below) appearing on any future days.

You may also make a task recur by clicking the **Recur** button to the right of
it. This will pre-fill it as a task on future days until you stop it, either by
clicking the **Recur** button again, which will keep it but stop it recurring
any further, or by deleting it, which will remove it *and* prevent it appearing
on future days.

Import/Export
-------------

At any time, you may export your data, or import existing data, on this tab.

To export your data, copy all the text under the **Export** heading. This is
kept up to date as you use the app, so don't worry about it missing anything
you've done - it won't.

To import data, put data exported previously into the text field under the
**Import** heading, click the **Import** button, and confirm that you do wish to
import data when the confirmation dialog pops up. This will *replace* your
current data with the imported data, so please be careful when replacing data
you haven't already exported. It ignores any whitespace in the data, so pasting
directly from an email ought to just work, even if your client splits the lines
of the email.

Options
-------

Here, you may clear your data, or set one of a small number of options once they
exist (at the present point, there are no features which require options, and I
would prefer to keep it that simple).

To clear your data, click the **Clear data** button, and confirm that do wish to
clear your data when the confirmation dialog pops up.


Where can I use it?
===================

The most recent tagged version will always be present on the `live demo`_, but
you can also run the app locally by downloading the `snapshot`_ or cloning the
repo if you prefer to track changes to it. You will need to be running some
kind of server on your machine, as the app is not currently able to work
correctly when run from file:// URLs (this may change in future, but at present
it is not possible).


.. _live demo: //bit-shift.github.io/tomorrow-ill/
.. _snapshot: //github.com/bit-shift/tomorrow-ill/archive/master.zip
