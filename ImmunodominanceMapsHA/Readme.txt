We simulated a germinal center response following 3 vaccinations (prime, boost 1, boost 2 scheme). In all of the simulations, the precursor frequency against all targeted residues is the same. Hence, it shows the role of immunogen geometry in manipulating B cell immunodominance.

To visualize the B cell immunodominance hierarchies to HA residue, we encode the fraction of memory B cells targeting a given residue following each vaccination onto 
the B-factor field of the pdb file.

There are corresponding pdb files for a vaccination with the full virus, nanoparticle presenting 8 HA molecules (HA-np), a nanoparticle presenting 8 HA stems (SS-np), and vaccination with the HA trimer.

These can be visualized by opening the pdb file with PyMol and writing in the command line:

show spheres

spectrum b, blue_white_red, minimum=0.01, maximum=0.14

-------------------------

For the "Virus_Vaccine_PostPrime.pdb"

show spheres

spectrum b, blue_white_red, minimum=0.01, maximum=0.14

-------------------------

For the "Virus_Vaccine_PostBoost1.pdb"

show spheres

spectrum b, blue_white_red, minimum=0.01, maximum=0.17

-------------------------

For the "Virus_Vaccine_PostBoost2.pdb"

show spheres

spectrum b, blue_white_red, minimum=0.01, maximum=0.19

-------------------------
