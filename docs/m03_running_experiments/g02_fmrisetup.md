---
layout: default
title: fMRI Equipment setup
parent: Running experiments
permalink: /runningexp/fsetup
nav_order: 3
---

# fMRI Equipment setup
{: .no_toc }
{: .fs-11 }


<!-- ## Table of contents
{: .no_toc .text-delta } -->

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }

1. TOC
{:toc}
</details>

# DBIC daily setup



step 1
{: .label .label-blue}
## Scanner Projector Computer
{: .d-inline-block .fs-6}

* [ ] Log in: [ username: mruser, password: mruser ]
* [ ] On login, Chrome automatically brings up login + pass for projector control
* [ ] turn projector on (this takes 7 minutes) in the scanner project PC.
* [ ] When running experiment, always make sure `Shutter off`
* [ ] + Check projector settings by clicking on the `status` menu
{: .fs-3 .px-6}

step 2
{: .label .label-blue}
## Screening form
{: .d-inline-block .fs-6}
* Same PC as Scanner Projector PC
* [ ] Get safety screening signed
* [ ] Log participant into REDcap system
* [ ] (Chrome comes on automatically which allows adding a participant)
{: .fs-3 .px-6}

```
    1. Dartmouth id > SID
    2. Gender (default female. Double check if participant is male!)
    3. Race/ethnicity (information should be filled in safety form)
    4. Make sure to get the correct DBIC study number in - spacetop is 1076
```
{: .px-6}

* [ ] Add SID and accession number to scanner notebook
* [ ] Add SID and accession number to ST_participant spreadsheet
{: .fs-3 .px-6}



step 3
{: .label .label-blue}
## Stim PC and MRI devices
{: .d-inline-block .fs-6}
* [ ] Screen: Plug video VGA via USB-C adapter to Stim PC
{: .fs-3 .px-6}

For Audio
{: .text-delta .px-6}
* [ ] Turn on Volume box: Pyle. Stereo power amplifier 2x15w
* [ ] Plug audio splitter (aux cable) to Stim PC
{: .fs-3 .px-6}

For Response:
{: .text-delta .px-6}
* [ ] Configure button box
* For 2-button box: select HID key 2x2 12345
{: .fs-3 .px-7}
* For trackball: select track
{: .fs-3 .px-7}

* [ ] Plug button box USB to Stim PC
* [ ] If using multiple response devices, be ready for switching out devices
* [ ] Prep Trackball in advance and put “on deck”
{: .fs-3 .px-6}




step 4
{: .label .label-blue}
## Medoc TSA setup
{: .d-inline-block }
{: .fs-6}

* [ ] Turn TSA-II on before experiment, for safety test to pass
* [ ] check green light on TSA-II
* [ ] check connection between TSA-II & medoc-PC (USB!!)
* [ ] Turn Medoc PC on and open Acknowledge software (admin/admin)
* [ ] Click participant, test, and make sure "external control" is on.
{: .fs-3 .px-6}
    * External control “on”: External control > check box
{: .fs-3 .px-7}
* [ ] plug in participant information (use BIDS id)
{: .fs-3 .px-6}


step 5
{: .label .label-blue}
## Matlab
{: .d-inline-block }
{: .fs-6 .mb-2}
* [ ] Open all relevant tasks during T1
* [ ] Double-check participant - we cannot mess this one up
* [ ] Pay attention when runs start and end
* [ ] Start key will be `s` before the trigger.
* [ ] End key will be `e`
{: .fs-3 .px-6}



step 6
{: .label .label-blue}
## After scanning
{: .d-inline-block }
{: .fs-6}
* [ ] Pull out trigger / audio from pc
* [ ] Restock the scrubs
* [ ] If laundry basket full, take it up
* [ ] Turn the TV / lights off
{: .fs-3 .px-6}

---

# Dartmouth fMRI PC setup
{: .d-inline-block}
Maintained by Heejung
{: .label .label-green }
![tasks]({{ site.url }}/images/dbic_setup.png)

fMRI jack:
{: .fs-6}
XAF-09 in Moore B75 on "fmri-private network (VLAN 2554)""
{: .fs-3}

medoc computer
{: .fs-6}
* medoc.dartmouth.edu
* ip: 10.64.1.10
* netmask: 255.255.255.240
* default gateway: 10.64.1.1
{: .fs-3}

spacetop computer
{: .fs-6}
* spacetop.dartmouth.edu
* ip: 10.64.1.9
* netmask: 255.255.255.240
* default gateway: 10.64.1.1
{: .fs-3}

Note from research computing:
{: .fs-6}
If you need to communicate with other systems outside of the fMRI private network besides 129.170.17.4 and 10.232.11.5 then the ACLs on the network will have to be modified.
{: .fs-3}

If help needed,
{: .fs-6}
contact Andrew Knutsen, Technology Support Specialist
or Heejung Jung, who helped set up.
{: .fs-3}

---

# Singularity container
{: .d-inline-block }
move elsewhere
{: .label .label-green}
---