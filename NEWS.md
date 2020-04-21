# recountWorkflow 1.11.2

SIGNIFICANT USER-VISIBLE CHANGES

* Documentation website is now available at
http://LieberInstitute.github.io/recountWorkflow/. It gets updated with every
commit on the master branch (bioc-devel) using GitHub Actions and pkgdown.
* Added a `NEWS.md` file to track changes to the package.

# recountWorkflow 1.11.2


BUG FIXES

* Fix the spelling of RIN to rin now that all SRA columns are in lower case.
* Fix the DESCRIPTION file (had a missing comma).


# recountWorkflow 1.11.1


NEW FEATURES

* Piggyback on GenomicState now that this package produces all the pieces
        needed for making the ER plots.
* Potentially everything works on Windows now that rtracklayer::import.bw()
        seems to work there. But I haven't tested it.

BUG FIXES

* Update SRARunTable.txt reading code since they changed the format on
        delivered by SRA. Adjust variables accordingly.

# recountWorkflow 1.7.2
------------------------

BUG FIXES

* Fix the call to bumphunter::annotateTranscripts().
* See https://gist.github.com/lcolladotor/196dabeb1ac628c35656bfa94b5d9577 for more details.


# recountWorkflow 1.7.1
------------------------

BUG FIXES

* Fix the ftp url for the Gencode v25 gtf file.


# recountWorkflow 1.3.1
------------------------

SIGNIFICANT USER-VISIBLE CHANGES

* Use BiocManager
    
# recountWorkflow 0.99.0


NEW FEATURES

* Created the workflow.
