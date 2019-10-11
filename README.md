# # # #

  Title : README.md
  Contents : Clinical/Translational Notes For Real-World Evidence (REW) Data Collection @ The Mighty
  Start Date : 10/5/19
  End Date : Longitudinal ; will automate/push change views

# # # #

Clinical/Translational/Technical Objectives :

1/ Identify Clinical/Translational Problem :

    1.1/ Problem Domain :: Clinical Medicine :: Psychiatry / Mental Health

    1.2/ Problem Statement :: Can the Mighty help in reducing the risk of suicidal ideation among users with BPD I/II?

    1.1.2/ Data Parameterization ::

      1.1.3/ Engineering Parameters :: As per discussion with Phil, what we need here is a
      SATURATED representation of the relevant epitope space. We can tilt the probability of
      achieving this representation by trying to get the best representation of the relevant proteome
      that we can. For example, this includes exclusion of immunogenic nanobodies that are cross-reactive
      with self and hence unsuitable. To determine the "goodness of fit" for a given representation
      we consider the kinetic parameters (i.e. phsicochemical parameters) of the system. As discussed
      with Phil, this reduces to understanding the noise characteristics of the k_d, k_a, etc parameters.
      Even a first-order Michaelis-Mentin distribution/curve should point us to the physical condition (i.e.
      library) from which to start. What we are actually try to do is iteratively, deterministically
      enrich this "starter" library. As discussed with Phil, we should be mindful that we match choice
      of library or libraries to the known state of translational targets. For example, if we start off
      with a well-known clinical target like Ras or TP53 or BRCA1 etc, we should have no short supply of
      choices from both Phil's library as well as the Superhuman library. We can then use those complementary molecules as the "starter" library. In the event that the kinetic parameters of these complementary
      moluecles is known and, after discussion with Phil and some calculations, we observe that the predicted behavior matches our intended experimental goal, we can just proceed with generation from the existing library.
        In the converse coase that we need to widen our search, we can and should sample from additional libraries. What follows is a running list of libraries of note relevant to this search space ::

          1.1.3.1/ Libraries

            #1/ Jenthera library

            #2/ Superhuman library

            #3/ Discovery Services : to be discussed with Phil

            https://www.criver.com/sites/default/files/resource-files/DS-DS-services-and-facilities.pdf

      1.1.4/ Engineered Output : Complementary set of antibodies (i.e. nanobodies) for a
      given guide RNA substrate.

      1.1.5/ Cost Upper Bound : to be discussed with Phil

      1.1.6/ Staging/Operations : to be discussed with Phil

    1.2/ guide RNAs

        1.2.1/ Objective :: Engineer complementary set of guide RNAs for a
        given clinically-oriented genomic locus.

        1.2.2/ Solution :: Physicochemical construction as per discussion with Phil by way of the Jenthera platform.

        1.2.3/ Engineering Parameters :: As per discussion with Phil, Jenthera's platform is the
        ideal solution to construct clinically-oriented guide RNAs.

            1.2.3.1/ Libraries

              #1/ Jenthera library

        1.2.4/ Engineered Output : Complementary set of guide RNAs for a
        given clinically-oriented genomic locus.

        1.2.5/ Cost Upper Bound : to be discussed with Phil

        1.2.6/ Staging/Operations : to be discussed with Phil

3/ PDX (Patient-Derived Xenograft) Models ; Chick Models

    3.1/ Translation Rescue Experiments

        1.1.1/ Objective :: Demonstrate ability or inability of engineered CRISPR nanobody/guide RNA pairs
        to rescue tumor growth in targeted mouse genomic backgrounds.  

        3.1.2/ Solution :: As discussed with Phil, we can take advantage of several existing PDX pipeline services. Most importantly, this solution is in keeping with our internal objective of de-noising
        the general services pipeline. This will also be a general testbed for goodness of fit in working with Jackson Labs (JAX) PDX services longitudinally. Our hope here is that we can establish a
        working example of a pipeline, along with all of the required handoffs as an instance of
        the internal architecture that we will presumably propagate.

        3.1.3/ Engineering Parameters :: As per discussion with Phil, the parameters of the PDX pipeline should be robust insofar as they've been industrialized (read: translated from bench science to actual working science) at JAX. With this in mind, our expectation is that the JAX repository of
        clinically-oriented mouse lines from which to generate particular genomic backgrounds suitable for
        rescue is possibly the best out there, if not the best.

        As discussed with Phil regarding the clinical HLA/BRCA Nature Medicine paper, presumably we
        would :
          1/ Genetically generate the required genomic backgrounds (e.g. by crossing to get, for example,
          a relevant tumorigenic haplotype like HLA-A+/+, HLA-B+/-, BRCA1+/-).
          2/ Assess engineered tumor growth in the crossed backgrounds. As per standard service practice.
          3/ Assess CRISPR rescue in a PDX model using the engineered tumors.

        3.1.4/ Engineered Output : Experimental set of CRISPR nanobody/guide RNA pairs that demonstrate
        rescue from explanted tumor growth of engineered genomic backgrounds. This data would also presumably
        include kinetic parameter data for the chosen clinical locus.

        3.1.5/ Cost Upper Bound : to be discussed with Phil

        3.1.6/ Staging/Operations : to be discussed with Phil


4/ Shortlist of potentially useful sources/references :

    1/ https://www.uptodate.com/contents/suicidal-ideation-and-behavior-in-adults

    2/ https://psychiatryonline.org/pb/assets/raw/sitewide/practice_guidelines/guidelines/suicide.pdf

    3/ https://afsp.org/about-suicide/risk-factors-and-warning-signs/

    4/ https://www.ncbi.nlm.nih.gov/pmc/articles/PMC419387/pdf/i1523-5998-5-4-169.pdf

    5/ https://www.jabfm.org/content/jabfp/28/1/65.full.pdf
