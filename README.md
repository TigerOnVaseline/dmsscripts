# SOS scripts for the Nortel DMS-100 

Stolen from Steve Barratt <steve.barratt@po7.etl.ericsson.se>

## IMAGIC

Checks whether the last image was successsful and if so, creates a script that contains the instructions to back up the MS and CM images to tape.
The tape volume is given a name based upon the current date.

## LINETOOLS

Despatchers with limited knowledge of DMS commands may require access to switches in order to determine the state of the local loop. This area of MAPCI contains much extraneous info that confuses untrained users. Misuse of MAPCI commands can be service-affecting.

Basically the utility allows the despatcher to examine the state of a line, busy/forcebusy it or return it to service without having any visibility of real MAPCI commands. It also provides a limited level of help and advice.

The following utility should be defined as the despatchers profile. All the commands used by it should be defined in table commands with an additional security level.

The despatcher should then be given only the additional level plus the profile command. Once the depatchers profile has been set the "profile" command should be withdrawn from the users permission.

## PATCHMAGIC

This program demonstrates how to identify files of a particular type and perform housekeeping activities on them.

## PERMISSIONS

Maintaining identical user permissions across a number of different switches can be quite a chore. Once a security strategy has been devised and command permissions have been defined, the following utility can be read by admin. Once modified according to your requirements the new commands will allow the administrator to rationalise user permissions. If the user does not exist the user will be created with "all." If the user does exist the user will be given the alloted permissions.

## PLOCURE

Posts and force-releases all lines in the PLO state

## SBSYCURE

Posts all system busy lines on the switch one at a time and force releases them. 

## TIDYDISK

Removes older duplicates from DDU drives.