RadMachine Test Packs
=====================

This repository is an open collection of test packs that can be imported into
RadMachine. Given the flexibility in RadMachine to create custom tests, test lists,
Python scripts, and portable test packs, this repository is intended to be a place for
Radformation as well as the community (via pull requests) to share test packs for individual
clinics to use directly or to use as a starting point and inspiration for their own custom tests.

What is a Test Pack?
--------------------

A test pack is a JSON file that contains one or more test lists, along with any associated dependencies. 
Test packs can be imported into and exported from RadMachine. These test packs can be used as a simplistic backup
mechanism for test configurations (note the test pack does not contain historical data) or to share test configurations
with satellite clinics or the community.

How to load a test pack file
----------------------------

To load a test pack file into RadMachine, follow these steps:

1. Download the test pack file (.tpk) from this repository or clone the repository.
2. Open RadMachine and go to the `Data Administration` tab of the navbar.
3. Under the `Quality Assurance` section, click on `Import Test Lists`.
4. Click `Choose File` and select the test pack file you downloaded.
5. If you only want a subset of the test lists in the pack, select them from the list on the left. No action is needed if you want to import all of the test lists.
6. Select the behavior if a conflict is detected (e.g. a test list with the same name already exists in the database).
7. Click `Import` to import the test lists into RadMachine.

How to share a test pack file
-----------------------------

To share a test pack file, follow these steps:

1. Open RadMachine and go to the `Data Administration` tab of the navbar.
2. Under the `Quality Assurance` section, click on `Export Test Lists`.
3. Select the test list(s) you want to export.
4. Give an helpful description of the test pack.
5. Provide a name for the test pack. This will be the name of the file, so it cannot have spaces or special characters. Use underscores or hyphens instead.
6. Click `Export` to download the test pack file.
7. Create a new issue in this repository and attach the test pack file. Provide a description of the test pack and any other relevant information.
8. The RadMachine team will review the test pack and merge it into the repository if it meets the guidelines.

Descriptions
------------

* `dqa3_beam_checks.tpk` - Contains the test lists for most machine energies when uploading from a Daily QA3 database. This test pack is typically used in conjunction with the RadMachine local agent.
  If you indicate that you have a Daily QA3 database when setting up RadMachine, Radformation will usually set these test lists up for you. These are provided for transparency and as
  and additional resource for clinics to use or modify as needed.
* `mpc_beam_checks.tpk` - Contains the test lists for most machine energies when uploading from a Varian "I" drive with Machine Performance Check (MPC) .csv files. This test pack is typically used in conjunction with the RadMachine local agent.
  If you indicate that you use MPC when setting up RadMachine, Radformation will usually set these test lists up for you. These are provided for transparency and as
  and additional resource for clinics to use or modify as needed.
* `tg142_monthly.tpk` - Contains test lists for monthly AAPM TG-142 tests. The tests lean towards are literal interpretation of the texts rather than an ideal or efficient flow.
* `tg142_daily.tpk` - Contains test lists for daily AAPM TG-142 tests. The tests lean towards are literal interpretation of the texts rather than an ideal or efficient flow.
* `tg51_with_chamber_calibration.tpk` - Contains test lists for performing TG-51 and a separate test list for entering chamber calibration kQ factors.
* `tg66_ct_daily_monthly.tpk` - Contains test lists for daily and monthly AAPM TG-66 tests for CT scanners.
* `quad_wedge.tpk` - Contains test lists for using the IC Profiler with the "quad wedge".
* `monthly_dosimetry_with_factors.tpk` - Contains test lists for monthly dosimetry tests with the ability to enter chamber calibration kQ factors annually.
