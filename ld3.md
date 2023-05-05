# Grep
Command line options:
## -v
Invert the query; all lines that do *not* contain the given string will be printed.
`grep -v a government/Alcohol_Problems/Session4-PDF.txt`
Output:
```




Session 4.
Implementing Preventive Interventions in

own.
developed severe dependence, thereby pre-venting the development of
The provision of such interventions is currently not routine. A
of time.10
service provider.15
pressure to do so within the field of emergency medicine.
to be successfully implemented. No other existing model is likely
by
referred.
providers of this service.44 Furthermore, instilling this knowledge
Studies of cost-effectiveness should include not only direct
insurers.
to be
not the development of new intervention models or prototypes.
self-help or 12-step
References
1999;67:989-94.
injury recurrence. Ann Surg 1999;230:473-83.
U.S. Government Printing Office; 2000.
1999;134:564-8.
Suppl):163-6.
1989;261:3115-20.
medicine. J Addict Dis 1996;15:1-7.
1989;261:403-7.
JAMA 1991;266:2837-42.
1998;93:589-94.
JAMA 1984: 252;1905-7.
1971;127:1653-8.
Stud Alcohol 2000;61:912-5.
1993;88:791-804.
No. 95-3769.
1996;28:435-42.
1990.
2001;62(6):806-16.
Services; 2000.
1995.
1991;81:1571-5.
1999;67:688-97.
1997;30:181-9.
1998;93:589-94.
1998;4:129-39.
Intern Med 1997;127:1097-1102.
directions. JAMA 1995; 274(13):1043-8.
55. Form of written consent, 42 C.F.R. sect. 2.31 (2001).
94-3722.


the ED.
intervention.
"Where were you drinking before you were injured?" Linking the
driving.
Reference


Comments on Implementing Preventive Interventions in Emergency
problems.
would be of tremendous benefit to the field of emergency medicine.
those interventions.
policies?
Intervention course.
do.
References
Emerg Med 1998;5(12):1200-9.
of Surgeons; 1998.


interventions. In his multi-center study, interventionists felt
needed to meet different clients' needs.
observed
setting.
medicine.
intervention effect on the control group.
reviewers.
the model.


```
It is printing all lines that do not contain the string 'a'. This could be useful in a file that has an abundance of a specific character, and lines that omit it are significant in some way. Maybe a list of files, and you want to see which files are there that do not belong to a specific directory (the string you would grep with)

`grep -v ' ' government/Alcohol_Problems/Session4-PDF.txt`
Output:
```





own.
abuse.10,13-18
department.
categories:
treatment.40
by
referred.
approach.2,3,34,51
rate.
insurers.
Recommendations
privacy.
References
1999;67:989-94.
1999;134:564-8.
Suppl):163-6.
1989;261:3115-20.
1989;261:403-7.
1998;93:589-94.
1971;127:1653-8.
1993;88:791-804.
1996;28:435-42.
1990.
2001;62(6):806-16.
1995.
1991;81:1571-5.
1999;67:688-97.
1997;30:181-9.
1998;93:589-94.
1998;4:129-39.
94-3722.


intervention.
hospital-based
barriers.
driving.
Reference


problems.
policies?
area.
do.
References


observed
setting.
medicine.
reviewers.


```
Here, it is printing all lines without a space. This translates to empty lines and last words in paragraphs.
## -n
Print the number of each matching line, as well as the lines themselves.
`grep -n legal government/Media/A_Perk_Of_Age.txt`
Output:
```
10:states, Washington D.C., and Puerto Rico operate legal-assistance
12:caregivers as well. Volunteers offer advice on legal questions,
13:provide self-help materials, and make referrals to legal aid
22:legal-services network. Anyone who meets the age requirement can
23:call the hot line, but hands-on legal counsel goes first to people
31:numbers and hours, go to www.aoa.gov/legal/hotline.html, or call
33:state without a hot line, the locator can point you to local legal
39:legal counseling, either face-to-face or by phone, at no cost.
```
This prints the corresponding line number of each line that has a matching phrase. This could be useful in programming contexts, where specific parts of code are referenced with line numbers.

`grep -n Karima government/Media/Working_for_Free.txt`
Output:
```
10:Karima A. Haynes
```
Line 10 alone is printed because it is the only one with the author's name.
## -r
Recursively search through a directory, rather than a single file

`grep -r 'ion channels' biomed`
Output:
```
biomed/1471-2091-2-16.txt:          related anion channels such as the extrajunctional
biomed/1471-2091-2-16.txt:        probe of tobacco budworm ion channels. Chemical libraries
biomed/1471-2091-3-15.txt:        this superfamily of ligand gated ion channels [ 1 2 3 ] .
biomed/1471-2091-3-15.txt:        structural similarity to other ligand gated ion channels
biomed/1471-2091-3-16.txt:        The cysteine-loop family of ligand gated ion channels
biomed/1471-2091-3-31.txt:          cell through open transduction channels), should permit
biomed/1471-2164-3-32.txt:        promotes activation of effector enzymes and ion channels by
biomed/1471-2164-3-32.txt:        such as GPCRs, ion channels, tyrosine phosphatases, nuclear
biomed/1471-2164-3-6.txt:          of ion channels and membrane bound receptors [ 6 ] . This
biomed/1471-2164-4-24.txt:        may as well be modifiers of ion channels or
biomed/1471-2202-2-18.txt:        5 6 7 ] . Some of these genes code for ion channels that
biomed/1471-2202-2-6.txt:        taste cells by direct interaction with apical ion channels.
biomed/1471-2202-2-7.txt:        non-NMDA receptors opens ion channels more permeable to
biomed/1471-2202-2-7.txt:        NMDA receptors are heteromeric ion channels composed of
biomed/1471-2202-3-11.txt:          including neuropeptides, ion channels, receptor and
biomed/1471-2202-3-11.txt:          dorsal spinal cord. A number of ion channels were found
biomed/1471-2202-3-11.txt:        receptors, ion channels, and signaling molecules to be
biomed/1471-2202-3-16.txt:          excitability (ion channels) or neurotransmission
biomed/1471-2202-3-17.txt:        on a class of ligand-gated ion channels called P2X [ 4 5 6
biomed/1471-2202-3-17.txt:          In some ligand-gated ion channels, such as ACh
biomed/1471-2202-3-4.txt:        ion channels [ 6 12 13 14 15 16 ] . Recent expression
biomed/1471-2202-3-4.txt:        trp family of ion channels. For those
biomed/1471-2202-3-4.txt:        ion channels within this superfamily for which
biomed/1471-2202-3-4.txt:          superfamily of ion channels, VR1 most likely assembles
biomed/1471-2202-3-4.txt:          for dimerization of limited domains of ion channels
biomed/1471-2202-4-10.txt:        short-term effects on ion channels and other effectors such
biomed/1471-2210-1-7.txt:        ...function not only as ion channels but
biomed/1471-2210-3-3.txt:        affect the permeability of gap junction channels. Secondly,
biomed/1472-6793-1-11.txt:        and represent a new family of Ca-selective ion channels
biomed/1472-6793-1-11.txt:        within the cell, or activation of Ca ++ion channels in the
biomed/1472-6793-2-2.txt:        MTX-activated cation channels and for understanding their
biomed/1472-6793-2-4.txt:        sensitivities) have been observed for ion channels
biomed/1472-6793-2-4.txt:        regulated non-selective cation channels [ 10 ] when gated
biomed/1472-6793-2-4.txt:        design, ion channels function to change membrane potential
biomed/1472-6793-2-4.txt:          voltage-gated ion channels [ 23 ] , which rely on a
biomed/1472-6793-2-4.txt:          as ion channels gated by cGMP, within a background of
biomed/1472-6807-2-1.txt:        ligand-gated ion channels, nAChRs are homo- or
biomed/1477-7827-1-31.txt:          ion channels that can contribute to the regulation of not
biomed/1477-7827-1-31.txt:          by 4-AP in pig GC are conducted by ion channels formed by
biomed/1477-7827-1-31.txt:          cell ion channels. We demonstrate for the first time not
biomed/gb-2001-2-7-research0025.txt:          associations among membrane proteins, ion channels,
biomed/gb-2002-3-10-research0055.txt:          are ion channels (Figure 7d, whereas others are
biomed/gb-2003-4-9-r58.txt:        +channels, insights into the ion channels in the genomes of
biomed/gb-2003-4-9-r58.txt:        although ion channels are clearly targets of insecticides.
```
Every line in every file in the biomed directory is searched for 'ion channels', and the corresponding file that each listing was found in is printed as well. This is very useful if you want to search through multiple text files easily.

`grep -r lovely .`
Output:
```./plos/journal.pbio.0020064.txt:        School of Medicine, New Haven, Connecticut, United States) says that ‘it is lovely to see
```
Here, the entire techincal folder (current working directory) is searched for 'lovely'
## -c
Print only the count of lines with occurences, rather than the lines themselves.
`grep -c 'circuit' biomed/gb-2001-2-4-research0012.txt`
Output:
```
8
```
The number of lines that have the word 'circuit' in them are printed. This is useful if you just want to know how many lines of a file contain a string, and don't need to know the specific lines themselves.

`grep -c 'we' government/Post_Rate_Comm/Gleiman_EMASpeech.txt`
Output:
```
44
```
44, the number of lines in the file that contain the phrase 'we', is printed.


