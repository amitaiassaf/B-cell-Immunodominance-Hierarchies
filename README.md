# B-cell-Immunodominance-Hierarchies

Related to the manuscript [**Defining and Manipulating B cell Immunodominance Hierarchies to Elicit Broadly Neutralizing Antibody Responses Against Influenza Virus**](https://www.cell.com/cell-systems/fulltext/S2405-4712(20)30335-5?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS2405471220303355%3Fshowall%3Dtrue) also find the pdf [**here**](https://github.com/amitaiassaf/B-cell-Immunodominance-Hierarchies/blob/master/Defining%20and%20Manipulating%20B%20cell%20Immunodominance%20Hierarchies%20to%20Elicit%20Broadly%20Neutralizing%20Antibody%20Responses%20Against%20Influenza%20Virus.pdf).


The yearly vaccine against the influenza virus targets a protein on its surface called hemagglutinin (HA), which helps the virus to bind and enter the host cells. Following vaccination, the immune system generates antibodies that target HA and can neutralize the virus. Most antibodies target the head of the HA protein, which mutates rapidly and often escapes those antibodies. The stem of HA contains conserved residues that are the target of broadly neutralizing antibodies. Eliciting strong antibody responses against the conserved part on the stem would offer universal protection. However, those conserved residues are immunologically recessive and are usually not targeted by the antibodies.

<img src="/Images/HA_3.jpg" width="600">

B cell immunodominance is a phenomenon where some part of an antigen is targeted more strongly that other. We sought to understand what are the rules determining the immunodominance of the head versus the conserved part on the stem. We study the effect of three factors:

1] Immunogen geometry.

2] B cell precursor frequency against different HA epitopes.

3] The initial affinity of those B cell precursors towards their target epitope.

To account for immunogen geometry, we created a coarse-grained representation of four immunogens used for vaccination

<img src="/Images/NP_1.jpg" width="600">

We used molecular dynamics simulations to compute the on-rate of the second and first one rate of an antibody model to different surface residues (epitopes) of HA as they are presented on the immunogen. We computed the on-rate of the first antibody arm and the second arm of the antibody, which gives us the geometry-dependent component contributing to epitope-specific affinity. 

<img src="/Images/virus_onrate_1.jpg" width="600">

The rates are input to a germinal center simulation that predicts the number of B cells created against different residue on the surface of HA

<img src="/Images/GC_scheme_1.jpg" width="600">

Based on this simulation, we can estimate the fraction of memory B cells against different surface residues - these are the B cell immunodominance maps (estimating from a simulation) of HA. The conserved part on the stem is outlined in yellow. Vaccination with the virus elicits very little response against this part

<img src="/Images/B_cell_immuno_virus.jpg" width="800">

You can download pdb files to illustrating the immunodominance maps of HA [Here](https://github.com/amitaiassaf/B-cell-Immunodominance-Hierarchies/tree/master/ImmunodominanceMapsHA)

Vaccinating with nanoparticle presenting the stem alone elicits response against the conserved residues

<img src="/Images/Bcell_immuno_SSnp.jpg" width="800">

The number of memory B cells against different epitopes depends on B cell precursor frequency and their initial (germline) affinity

<img src="/Images/Bcell_immuno_SSnp_precursor_affinity.jpg" width="800">
