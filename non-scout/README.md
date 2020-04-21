## preProc-XML ##

Some additional context to this working directory: these files are the de-duplicated remnants of the following directories on central:/d1/area3/prod3/prod_picked_up/05

* 20110310-errors/
* 20110406/
* 20121127/
* 20100205_InsuranceCompany/
* 20100209_Lyndy-Ian_misc/
* oldJPEGs/

After de-duplicating the directories and basic well-formedness/validation checks, the XML and associated JPEGs are bundled together. 

these are files that have been languishing on our work server for a long time (the blame, i'll take it). they are (poorly) grouped into several directories:

* HOLD (125 transcriptions)
* problems 
* READY (283 transcriptions)
* RETURN (15 transcriptions)
* RETURN-BACK (332 transcriptions)
* unnecessary-copies 
* unused-images

i'm working on trying to figure out what these different directories are meant to hold (it's been too long since i worked on this). There is a **lot** of duplication in these directories, so these file counts are misleading.

### HOLD ###
In addition to these files missing LCSH keywords, these need to have their note\[@type='collection'] and note\[@type='manuscript'] values double-checked. In other respects, these files are in good shape.

#### to do ####
* fix duplicate bibl/* elements; e.g. some of the 0012_000060* TEI

### READY ###
What it says on the tin, with a caveat.

#### to do ####
* check for duplicate bibl/* elements

### RETURN and RETURN-BACK ###
<a id="return"/>
#### RETURN ####
The files the were kept here have been moved to the problems directory or deleted because they were duplicates.

#### RETURN-BACK ####
Lots of duplicates in here. D: Fortunately, all relatively easy to deal with. The files in RETURN-BACK were duplicated processing files for TEI in HOLD and READY.

### unnecessary-copies ###
Again, many duplicated processing files under this directory. Any unique files were (eventually) moved to the problems directory.

### problems ###
The same: lots of duplicated files in here. Diffing vs the copies in HOLD or READY suggested that it was safe to delete the copies under problems. The files that are left over should probably go to RETURN, or maybe those files need to come here. Okay, I decided to put them all in ~~RETURN~~  problems (or keep them here, as the case may be)!

* 0012_000060_000413* - these JPEGs do **not** have a corresponding XML file that I can find (on any of our servers)
* 0012_000117*, David Burford Papers, MS.1185
    * 0012_000117_000206_0000/ is an incomplete transcription
        * missing last page
    * 0012_000117_000201_000{1..3}.jpg(s) are missing their transcription
        * isn't on central:/d1/area3/prod3/
* 0012_000194_000200_0000/ 
    * missing figures/* 
* 0012_002408_000200_0000/ is a still image; there isn't any text to transcribe
    * should probably be treated like a basic/large image
    * associated hand-written memoir @ [processed-files/READY/0012_002408_000200_0000](./processed-files/READY/0012_002408_000200_0000)
* 0012_001519_000224_0001.jpg is a still image
    * should probably be treated like a basic/large image
    * associated with the Horace Maynard Papers, MS.0415
* 0012_000840_* - these JPEGs do **not** have a corresponding XML file that I can find on central.

### unused-images >> 001526-images-onHold ###
The image files here are associated with The University of Tennessee's President's Papers, AR.0001. This collection was digitized, transcribed (to a certain extent), and then delivered in Trace. The TEI files are on central:/d1/area3/prod3/prod_picked_up/001526_onHold