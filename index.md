# Lab Report 3 - Researching Commands (Week 6)
The lab report showcases the implementation of the `grep` command with four different command-line options. The `grep` command is used on the directory located at https://github.com/ucsd-cse15l-s23/stringsearch-data.

1. `-i` would match the lines containing a specific word in a file. <br>
    Examples: <br>
    1.  The following example searches for and returns all lines which contain the word *hello* in the given file:<br>
        input: `grep -i "hello" stringsearch-data/technical/911report/chapter-1.txt`<br>
        output: `At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?`
   2. The following example searches for and returns all lines which contain the word *using* in the given file:<br>
        input: `grep -i "using" stringsearch-data/technical/biomed/1468-6708-3-1.txt`<br>
        output: `for all subjects using a baseline home interview, an
          report results using only the simpler definition.
          years, using validated methods presented elsewhere [ 20 ]
          for difference among BMI groups using confidence
        using either YHL or YOL as the outcome variable. Trials to
        evaluated using YHL, but not YOL. Trials to improve the
        the persons with partially estimated data, and using two
          be performed efficiently using either YOL or YHL as the
        measures of YHL. Using either YOL or YHL, however, we found
        'overweight' by the NHLBI guidelines. This suggests using`

2. `-r` will match and return the lines containing a specific word in **all** files under the given directory and its subdirectories. <br>
    Examples: <br>
    1.  The following example searches for and returns all lines which contain the word *cannot* in all files under and the given directory and its subdirectories:<br>
        input: `grep -r "cannot" stringsearch-data/technical/biomed` <br>
        output: `stringsearch-data/technical/biomed/gb-2002-4-1-r2.txt:        which cannot initiate actin polymerization in host cell
stringsearch-data/technical/biomed/gb-2002-4-1-r2.txt:        mutant (DP-L1942) [ 30], which cannot initiate the
stringsearch-data/technical/biomed/gb-2002-4-1-r2.txt:        of the internalins, but cannot escape from the phagocytic
stringsearch-data/technical/biomed/gb-2002-4-1-r2.txt:          cytoskeleton. We cannot rule out the possibility that
stringsearch-data/technical/biomed/gb-2002-4-1-r2.txt:          host-pathogen interactions, they cannot fruitfully assist
stringsearch-data/technical/biomed/1471-2202-2-9.txt:          cannot be ruled out. However, when these data are taken
stringsearch-data/technical/biomed/1471-2202-2-9.txt:          this three-dimensional parallel geometry. It also cannot
stringsearch-data/technical/biomed/cc991.txt:        clearance alters outcomes cannot be determined from our
stringsearch-data/technical/biomed/cc991.txt:        effects. Our design cannot answer this question. All
stringsearch-data/technical/biomed/1476-069X-2-4.txt:          evidence that one cannot simply calculate public health
stringsearch-data/technical/biomed/1471-2164-2-9.txt:          of yCCR4 cannot mediate transcription activation, but is
stringsearch-data/technical/biomed/gb-2001-2-4-research0010.txt:          be small). The effect cannot be fully explained by
stringsearch-data/technical/biomed/gb-2001-2-4-research0010.txt:          and cannot change. Thus, the frequency of each codon can
stringsearch-data/technical/biomed/gb-2001-2-4-research0010.txt:          cannot be distinguished from a G→C mutation on the other.
stringsearch-data/technical/biomed/1471-213X-2-1.txt:          effects of PN-1 on GnRH neuronal distribution cannot be
stringsearch-data/technical/biomed/1471-2180-2-22.txt:        bacteria in nature cannot be cultured. Our work indicates
stringsearch-data/technical/biomed/1471-2180-2-22.txt:        Unfortunately, we cannot sample all possible terrestrial
stringsearch-data/technical/biomed/1471-2180-2-22.txt:        Valley, Antarctica) appears to be sterile. We also cannot
stringsearch-data/technical/biomed/1471-2091-2-11.txt:          glycine-conjugated bile acids cannot be attributed simply
stringsearch-data/technical/biomed/gb-2001-2-4-research0011.txt:          of protein sequence similarity of HNBC7 to SLC4A9 cannot
stringsearch-data/technical/biomed/gb-2001-2-4-research0011.txt:          and function, if any, of such a protein cannot be known
stringsearch-data/technical/biomed/1468-6708-3-10.txt:          left or right ventricular dysfunction that cannot be
stringsearch-data/technical/biomed/1468-6708-3-10.txt:        beta-blockers cannot be ascertained from the data.
stringsearch-data/technical/biomed/gb-2003-4-5-r34.txt:          shown because the input parameter cannot be tuned to
stringsearch-data/technical/biomed/gb-2003-4-5-r34.txt:          raw data matrix as input, so we cannot apply these two
stringsearch-data/technical/biomed/1471-2202-2-8.txt:        geometry) cannot be evaluated separately. This limitation
stringsearch-data/technical/biomed/1471-2202-2-8.txt:          present prior to injury (disrupted geometry) cannot be
stringsearch-data/technical/biomed/1471-2202-2-8.txt:          growth cones on the sections cannot be assumed to be the
stringsearch-data/technical/biomed/1471-2202-2-8.txt:          uncrushed nerve. The reduced neurite density cannot be
stringsearch-data/technical/biomed/1471-2156-3-10.txt:        cannot be generalized to the original population from which
stringsearch-data/technical/biomed/1471-2458-3-20.txt:        reliable, as the level and effect of panic likely cannot be
stringsearch-data/technical/biomed/1471-2350-4-2.txt:        or both of these, and cannot distinguish them. To measure
stringsearch-data/technical/biomed/1472-6807-2-3.txt:          functional relationships that cannot be detected by
stringsearch-data/technical/biomed/1472-6807-2-1.txt:        135 of beta2, but cannot accommodate Leu 135 of beta4.
stringsearch-data/technical/biomed/1476-4598-1-8.txt:        only methylation of full-length CpG islands and cannot
stringsearch-data/technical/biomed/1476-4598-1-8.txt:        MGMT cannot be ruled out. Other
stringsearch-data/technical/biomed/1476-0711-2-7.txt:        cannot be followed strictly within the specified time
stringsearch-data/technical/biomed/gb-2002-4-1-r1.txt:            very short conserved regions still cannot be covered by
stringsearch-data/technical/biomed/gb-2001-2-7-research0025.txt:          that span the centromere. Thus, the jump cannot be
stringsearch-data/technical/biomed/ar130.txt:        cannot explain our failure to eliminate BMPCs in fresh
stringsearch-data/technical/biomed/ar130.txt:        7). This cannot be explained by proliferation, because BMP2
stringsearch-data/technical/biomed/1471-2253-2-5.txt:          PBPK parameters [ 45 47 ] . PKQuest cannot complete with
stringsearch-data/technical/biomed/1471-2202-3-19.txt:        morphine cannot stimulate δ receptor as effectively as
stringsearch-data/technical/biomed/1472-6963-2-10.txt:        , such as complications, one cannot deduce from this study
stringsearch-data/technical/biomed/1471-2458-3-5.txt:        cannot be amplified. This explanation would account for the
stringsearch-data/technical/biomed/1471-2458-3-5.txt:        cannot determine if the microorganism is infectious at the
stringsearch-data/technical/biomed/1471-2458-3-5.txt:        cannot be used for longer than 15-20 minutes. As was
stringsearch-data/technical/biomed/1472-6769-1-4.txt:        antitumor activity, CC-1065 cannot be used in humans
stringsearch-data/technical/biomed/gb-2003-4-4-r26.txt:          M. incognita , we cannot rule out
stringsearch-data/technical/biomed/1471-2180-2-35.txt:          mouse's defenses cannot prevent further growth of the
stringsearch-data/technical/biomed/1471-2121-3-12.txt:        in addition to causing rapid degradation, one cannot rule
stringsearch-data/technical/biomed/1471-2121-3-12.txt:        intracellularly [ 3 4 ] , although one cannot rule out that
stringsearch-data/technical/biomed/gb-2001-2-3-research0008.txt:          both tissues, so transcripts detected in both cannot be
stringsearch-data/technical/biomed/1471-2156-2-1.txt:          AKXD28 chromosome cannot be ruled out. The presence in
stringsearch-data/technical/biomed/1471-2466-3-1.txt:        patients were without overt inflammatory disease, we cannot
stringsearch-data/technical/biomed/1471-2466-3-1.txt:        infection, cannot exclude either of these hypotheses.
stringsearch-data/technical/biomed/bcr568.txt:        these prognostic markers, high-risk NNBC patients cannot be
stringsearch-data/technical/biomed/1475-2875-2-14.txt:        effect of malaria during treatment cannot be dismissed. It
stringsearch-data/technical/biomed/1475-2875-2-14.txt:          elevation of intracellular calcium cannot be attributed
stringsearch-data/technical/biomed/1475-2875-2-14.txt:          occur within 20 min of exposure, but cannot be accounted
stringsearch-data/technical/biomed/1471-2288-2-4.txt:        additional diagnostic follow-up. Therefore they cannot be
stringsearch-data/technical/biomed/1475-2875-2-10.txt:        very limited budgets and cannot afford to discard drugs
stringsearch-data/technical/biomed/1475-2875-2-10.txt:        because outlets were not randomly selected, one cannot
stringsearch-data/technical/biomed/1475-2875-2-10.txt:        but it also had some drawbacks. Mystery shoppers cannot
stringsearch-data/technical/biomed/1471-2156-2-5.txt:          2-DG causes glucose repression but cannot be used as a
stringsearch-data/technical/biomed/ar68.txt:          these results cannot be interpreted in a C 
stringsearch-data/technical/biomed/ar68.txt:          RNA, these fingerprinting assays cannot readily
stringsearch-data/technical/biomed/1471-2172-3-2.txt:        In our system, we cannot distinguish if the amino acid
stringsearch-data/technical/biomed/1472-6750-1-12.txt:        lethality cannot be studied using regular transgenic
stringsearch-data/technical/biomed/1472-6750-1-12.txt:        procedures because lines of founder mice cannot be
stringsearch-data/technical/biomed/1472-6882-1-7.txt:        of FMS, the results cannot be compared directly with other
stringsearch-data/technical/biomed/1472-6882-1-7.txt:        studies. It's possible, but cannot be proven here, that
stringsearch-data/technical/biomed/1471-2148-2-15.txt:          equation based on Bayes' Theorem cannot therefore be
stringsearch-data/technical/biomed/1472-6874-2-1.txt:        sexual frequency of zero cannot become worse, this may have
stringsearch-data/technical/biomed/1471-2091-3-8.txt:        cannot be synthesized by mammals, and thus thiamine can be
stringsearch-data/technical/biomed/1471-2091-3-8.txt:        cytosolic and mitochondria cannot convert thiamine to ThDP
stringsearch-data/technical/biomed/1471-2091-3-8.txt:          and mitochondria cannot convert thiamine to ThDP [ 14 16
stringsearch-data/technical/biomed/1471-2091-3-8.txt:          lymphoblasts cannot take up thiamine with high affinity,
stringsearch-data/technical/biomed/1471-2091-3-8.txt:        since mitochondria cannot form ThDP from thiamine [ 14 15
stringsearch-data/technical/biomed/1472-6793-2-8.txt:        differences in innate fiber phenotype. However, we cannot
stringsearch-data/technical/biomed/1472-6793-2-8.txt:        induced angiogenesis cannot be determined from our study.
stringsearch-data/technical/biomed/1472-6793-2-8.txt:        We cannot explain why electrical stimulation tends to
stringsearch-data/technical/biomed/1471-213X-2-7.txt:          of the socket cells. We cannot be certain from these
stringsearch-data/technical/biomed/1471-2202-3-20.txt:        it cannot be ruled out, based on the present study, that
stringsearch-data/technical/biomed/1471-2350-2-2.txt:        cannot exclude the possibility of inadequate power to
stringsearch-data/technical/biomed/gb-2001-2-11-research0046.txt:          remain to be defined and these SDPs unfortunately cannot
stringsearch-data/technical/biomed/gb-2001-2-8-research0032.txt:          their negative indexes. Here, we cannot obtain correct
stringsearch-data/technical/biomed/gb-2001-2-8-research0032.txt:          one gene, the fold change cannot be estimated with much
stringsearch-data/technical/biomed/1471-2415-3-1.txt:        onset age of cataract. Though we cannot deduce the age of
stringsearch-data/technical/biomed/gb-2003-4-5-r32.txt:          basic tissue elements and therefore cannot be validated
stringsearch-data/technical/biomed/1472-6750-1-13.txt:        the selected substitutions cannot always be conveniently
stringsearch-data/technical/biomed/1471-2156-3-16.txt:          possibilities are that these chromosomes cannot express
stringsearch-data/technical/biomed/1471-2156-3-16.txt:        ] ? If so, obviously the cutter and telomerase cannot
stringsearch-data/technical/biomed/1471-2156-3-16.txt:        with template As, several cannot, specifically the 25 dAs
stringsearch-data/technical/biomed/gb-2003-4-7-r43.txt:        TCRs cannot be discounted.
stringsearch-data/technical/biomed/1472-6807-2-5.txt:        fibers that are grossly similar, we cannot be certain that
stringsearch-data/technical/biomed/ar297.txt:          precaution: no contamination was detected. We cannot
stringsearch-data/technical/biomed/1471-2172-3-1.txt:        cannot be a concern. After 3.0 h incubation RNA was
stringsearch-data/technical/biomed/gb-2003-4-5-r30.txt:          between the downstream sequences of two such L1s cannot
stringsearch-data/technical/biomed/gb-2002-3-9-research0051.txt:          C. psittaci apparently cannot
stringsearch-data/technical/biomed/gb-2002-3-9-research0051.txt:        between closely related stains, one cannot be certain at
stringsearch-data/technical/biomed/gb-2002-3-9-research0051.txt:        C. psittaci. It cannot be ruled out
stringsearch-data/technical/biomed/gb-2002-3-9-research0045.txt:          expression in seedling leaves and adult leaves cannot be
stringsearch-data/technical/biomed/gb-2002-3-9-research0045.txt:          hybridization conditions cannot resolve the precise
stringsearch-data/technical/biomed/gb-2002-3-9-research0045.txt:          fraction of constitutively expressed genes cannot be
stringsearch-data/technical/biomed/gb-2001-2-8-research0030.txt:          is much less expensive. However, *PheC cannot be
stringsearch-data/technical/biomed/gb-2001-2-8-research0030.txt:          Methanococcus jannaschii cannot be
stringsearch-data/technical/biomed/bcr631.txt:        the development of drug resistance. Nevertheless, we cannot
stringsearch-data/technical/biomed/bcr631.txt:          with caution because functional protein levels cannot be
stringsearch-data/technical/biomed/bcr631.txt:          cannot be classified as truly 'normal' breast tissue.
stringsearch-data/technical/biomed/bcr631.txt:          isotypes alone cannot confer resistance to antimitotics.
stringsearch-data/technical/biomed/cc3.txt:        output cannot be sustained by cardiac physiology [ 30].
stringsearch-data/technical/biomed/cc3.txt:        also consider what we cannot afford not to monitor. Massive
stringsearch-data/technical/biomed/1471-2431-2-4.txt:        sucrose and some starches. Because absorption cannot take
stringsearch-data/technical/biomed/1471-2458-3-2.txt:        infection [ 36 ] . Although our results cannot be
stringsearch-data/technical/biomed/1477-7819-1-10.txt:        which cannot be assessed preoperatively by clinical
stringsearch-data/technical/biomed/1477-7819-1-10.txt:        tongue cancer [ 16 17 ] . Its diagnostic role cannot be
stringsearch-data/technical/biomed/bcr618.txt:        practice pattern of individual physicians, and cannot be
stringsearch-data/technical/biomed/1471-2229-2-4.txt:        However, alternative explanations cannot be ruled out at
stringsearch-data/technical/biomed/1471-2229-2-4.txt:        of only 1.4 mM indicates that the effects of mannose cannot
stringsearch-data/technical/biomed/1471-2229-2-4.txt:        explanations cannot be ruled out at this time. The
stringsearch-data/technical/biomed/1471-2350-3-12.txt:          Although the assumptions of the t-test cannot be
stringsearch-data/technical/biomed/gb-2002-3-9-research0044.txt:        cannot be co-clustered with one another), such a strategy
stringsearch-data/technical/biomed/gb-2002-3-9-research0044.txt:        represent fragments of the full transcripts, we cannot be
stringsearch-data/technical/biomed/1471-2474-4-4.txt:        certain heuristics that cannot be directly translated into
stringsearch-data/technical/biomed/1472-6904-2-5.txt:          as single compartments. This means that PKQuest cannot
stringsearch-data/technical/biomed/1472-6904-2-5.txt:          cannot be directly determined by the deconvolution
stringsearch-data/technical/biomed/1472-6823-3-1.txt:        cannot be assigned without the ability to control for other
stringsearch-data/technical/biomed/1471-2474-2-2.txt:        rats cannot respond that quickly and fail to complete the
stringsearch-data/technical/biomed/1471-2474-2-2.txt:        fracture healing in these older rats, and we cannot find
stringsearch-data/technical/biomed/gb-2002-3-2-research0008.txt:        a duplication because of its long-term advantage cannot
stringsearch-data/technical/biomed/gb-2002-3-2-research0008.txt:        s ratio in paralogous genes cannot be
stringsearch-data/technical/biomed/gb-2002-3-11-research0059.txt:            the experiments that cannot be realized when the
stringsearch-data/technical/biomed/gb-2002-3-11-research0065.txt:        the reference strain cannot be compared to the reference
stringsearch-data/technical/biomed/1471-2164-3-15.txt:        reveals that this virus-like element cannot be assigned to
stringsearch-data/technical/biomed/1471-2164-3-15.txt:        viral phyla. This element cannot be assigned to any known
stringsearch-data/technical/biomed/1471-2288-3-4.txt:          a . We cannot observe type 
stringsearch-data/technical/biomed/1471-2288-3-4.txt:          cannot be ruled out. The PSE estimates were higher than
stringsearch-data/technical/biomed/gb-2002-3-8-research0040.txt:          related, but whose similarities cannot necessarily be
stringsearch-data/technical/biomed/1475-2867-3-12.txt:        transcription or RNA processing, we cannot rule out the
stringsearch-data/technical/biomed/1471-2164-3-16.txt:        Thus, from the amplified results, one cannot infer the
stringsearch-data/technical/biomed/1471-2164-3-16.txt:          cannot be reliably distinguished from background noise.
stringsearch-data/technical/biomed/gb-2002-3-12-research0087.txt:          cannot be sure to have reached the true start site, even
stringsearch-data/technical/biomed/1471-2091-3-30.txt:          AA release by U0126 cannot be ascribed to a failure in
stringsearch-data/technical/biomed/gb-2002-3-12-research0078.txt:        genes were also identified that cannot formally be ruled
stringsearch-data/technical/biomed/1471-2172-2-4.txt:          we cannot rule out the possibility that Btk:ER activates
stringsearch-data/technical/biomed/1471-2180-1-12.txt:        DNA synthesis [ 7, 9, 10], (ii) it cannot be isolated in an
stringsearch-data/technical/biomed/1471-2180-1-12.txt:        polarity DNA cannot be synthesized and no infectious
stringsearch-data/technical/biomed/1471-2180-1-12.txt:          oligonucleotide of positive polarity that cannot anneal
stringsearch-data/technical/biomed/1471-2180-1-12.txt:          assay. Micrococcal nuclease cannot gain access to the
stringsearch-data/technical/biomed/1471-2180-1-12.txt:        that we cannot formally exclude. The first possible cause
stringsearch-data/technical/biomed/1471-2180-1-12.txt:        contribute to the commitment. However, this cannot entirely
stringsearch-data/technical/biomed/1471-2180-1-12.txt:        cannot degrade exogenous substrates under a very wide
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          delay artifacts, one probably cannot expect to be able
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          It is clear from these results that one cannot judge
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          that cannot be described by a single gamma distribution,
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          solution so that the input rate cannot be negative. In
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          If the input cannot be described by a single gamma
stringsearch-data/technical/biomed/1472-6904-3-1.txt:          analytical approach cannot be constrained from reaching
stringsearch-data/technical/biomed/1476-072X-2-4.txt:          epidemiological studies, pattern analysis cannot
stringsearch-data/technical/biomed/1476-072X-2-4.txt:        dataset covers the period from 1993-7. We cannot argue that
stringsearch-data/technical/biomed/1476-072X-2-4.txt:        causal relationship cannot be precluded. This is an
stringsearch-data/technical/biomed/1471-2105-4-24.txt:        differences cannot be determined from this data. However,
stringsearch-data/technical/biomed/1471-2105-4-24.txt:        hand, if bias cannot be excluded, the possibility must be
stringsearch-data/technical/biomed/1471-2156-3-3.txt:        position of each eye is downward and cannot be elevated
stringsearch-data/technical/biomed/1471-2156-3-3.txt:          therefore, this locus cannot be formally ruled out.
stringsearch-data/technical/biomed/1471-2466-2-3.txt:        However, we cannot definitely exclude residual confounding
stringsearch-data/technical/biomed/1471-2466-2-3.txt:        we cannot exclude the potential of residual confounding.
stringsearch-data/technical/biomed/gb-2003-4-2-r14.txt:          Xylella , one cannot be certain
stringsearch-data/technical/biomed/ar422.txt:          protease-resistant fragments, it cannot be ruled out that
stringsearch-data/technical/biomed/1472-6831-3-1.txt:        cannot be etched because of the acid resistance of ZrO 
stringsearch-data/technical/biomed/1472-6831-3-1.txt:          cannot exclude that these differences are coincidental.
stringsearch-data/technical/biomed/1472-6831-3-1.txt:          In the case of Procera, one cannot exclude the
stringsearch-data/technical/biomed/1472-6831-3-1.txt:          beneficial clinical advantages that cannot be
stringsearch-data/technical/biomed/ar387.txt:        sedentary lifestyle. Moreover, we cannot determine whether
stringsearch-data/technical/biomed/ar387.txt:        hip arthritis patients cannot be deemed causative of the
stringsearch-data/technical/biomed/ar387.txt:        cannot be ignored. Our data suggest that we should not
stringsearch-data/technical/biomed/1471-2105-2-8.txt:          But here, we cannot assume equiprobability for the
stringsearch-data/technical/biomed/1471-2105-2-8.txt:          regions, we cannot exclude the possibility that they
stringsearch-data/technical/biomed/1471-2105-2-8.txt:          correspond to novel RNAs, and we cannot assign a known
stringsearch-data/technical/biomed/1471-2105-2-8.txt:        BLASTN cannot detect RNA sequences that are this diverged.
stringsearch-data/technical/biomed/1478-7954-1-3.txt:        and the onset of chronic diseases cannot be addressed using
stringsearch-data/technical/biomed/1478-7954-1-3.txt:        alcohol intake data in the FOS cannot make such
stringsearch-data/technical/biomed/1471-2091-3-31.txt:        that chemomechanical coupling cannot ensue.
stringsearch-data/technical/biomed/gb-2002-3-12-research0086.txt:          cannot otherwise be detected in pairwise comparisons.
stringsearch-data/technical/biomed/1476-069X-1-3.txt:        ventilated corporate offices, it cannot be extrapolated to
stringsearch-data/technical/biomed/1471-2431-3-4.txt:          socioeconomic group. Nevertheless, bias cannot be
stringsearch-data/technical/biomed/1471-2431-3-4.txt:          the present study, bias in the sample cannot be excluded.
stringsearch-data/technical/biomed/1471-2431-3-4.txt:          answers cannot be excluded.
stringsearch-data/technical/biomed/gb-2002-3-12-research0082.txt:        become available, we cannot hope to provide a high level of
stringsearch-data/technical/biomed/gb-2002-3-12-research0082.txt:        biological features still cannot be recognized by
stringsearch-data/technical/biomed/ar750.txt:        other sex-specific factors cannot be ruled out. In our
stringsearch-data/technical/biomed/1471-2474-3-3.txt:        so that reported deformation rates cannot be converted into
stringsearch-data/technical/biomed/1472-6785-2-6.txt:        sampled repeatedly and each individual sample cannot be
stringsearch-data/technical/biomed/1472-6785-2-6.txt:        stages. It cannot be ignored, however, that such a pattern
stringsearch-data/technical/biomed/1477-7827-1-9.txt:        secondary interstitial cells, one cannot exclude the
stringsearch-data/technical/biomed/gb-2001-2-6-research0021.txt:            determined, we cannot infer detailed structure-function
stringsearch-data/technical/biomed/ar624.txt:        present study. However, we cannot completely exclude the
stringsearch-data/technical/biomed/1471-2105-3-14.txt:        based methods alone cannot recognize that a new sequence
stringsearch-data/technical/biomed/1471-2105-3-14.txt:        sequence cannot be inferred (in the two proteomes analyzed
stringsearch-data/technical/biomed/1471-2105-3-28.txt:          53 bits of precision [ 5 ] ) cannot be determined. The
stringsearch-data/technical/biomed/1471-2105-3-28.txt:           , the true forward and backward distances, cannot be
stringsearch-data/technical/biomed/1471-2458-2-11.txt:          when emission rates cannot be accurately determined.
stringsearch-data/technical/biomed/gb-2001-2-6-research0020.txt:        and common regulation cannot easily account for the
stringsearch-data/technical/biomed/gb-2001-2-6-research0020.txt:        genes in which order is conserved. A run cannot comprise
stringsearch-data/technical/biomed/cc103.txt:          diuretics cannot be recommended to prevent ATN.
stringsearch-data/technical/biomed/cc103.txt:          function cannot be recommended. This is not to say that
stringsearch-data/technical/biomed/gb-2002-3-12-research0083.txt:            and cannot be annotated until the duplications are
stringsearch-data/technical/biomed/gb-2002-3-12-research0083.txt:            cannot be expected to cover every eventuality. As a
stringsearch-data/technical/biomed/1471-2180-3-13.txt:          cannot rule out a functional role for stem loops b and c
stringsearch-data/technical/biomed/1471-2210-2-8.txt:          conditions of the experiment [ 8 ] . Therefore it cannot
stringsearch-data/technical/biomed/1472-6793-1-8.txt:          cannot be explained by charge movements in the γ 
stringsearch-data/technical/biomed/1472-6793-1-8.txt:          1 subunit. However, we cannot rule out
stringsearch-data/technical/biomed/1472-6793-1-8.txt:        inactivation cannot be completely ruled out. The γ 
stringsearch-data/technical/biomed/1471-2350-3-1.txt:        genes when carrier status cannot be defined on the basis of
stringsearch-data/technical/biomed/1471-2350-3-1.txt:            ischemic stroke. If the SVC neurologist cannot confirm
stringsearch-data/technical/biomed/1471-2350-3-1.txt:            If the diagnosis of ischemic stroke cannot be verified
stringsearch-data/technical/biomed/1471-2350-3-1.txt:        recorded in a research database. This right cannot be
stringsearch-data/technical/biomed/gb-2002-3-11-research0062.txt:          Because one cannot determine 
stringsearch-data/technical/biomed/gb-2002-3-11-research0060.txt:          chromosome usually cannot be resolved by the chromosomal
stringsearch-data/technical/biomed/cc303.txt:        for RRHs cannot be explained by patient record selection
stringsearch-data/technical/biomed/1471-2377-3-4.txt:        if the specific studies cannot be known. A future-use
stringsearch-data/technical/biomed/1471-2180-3-11.txt:          the first passage, which implies that the mutant cannot
stringsearch-data/technical/biomed/1471-2180-3-11.txt:          mutant, the mutant virions cannot benefit from phenotypic
stringsearch-data/technical/biomed/1471-2180-3-11.txt:        , we cannot compare the mutant frequencies reported in
stringsearch-data/technical/biomed/1471-2180-3-11.txt:        mutant, so that the mutant virions cannot benefit from
stringsearch-data/technical/biomed/1471-2091-3-22.txt:          identified here (Fig. 7A). At present, we cannot exclude
stringsearch-data/technical/biomed/1471-2172-3-16.txt:          indirect. Although we cannot rule out the possibility
stringsearch-data/technical/biomed/1471-2121-2-22.txt:        analysis cannot disprove the hypothesis that by mutating
stringsearch-data/technical/biomed/1471-2121-3-8.txt:        studies activated NF-κB cannot protect cells from apoptosis
stringsearch-data/technical/biomed/1472-6963-1-8.txt:          charges, and cannot be separated out. Charges by the
stringsearch-data/technical/biomed/1471-2407-2-15.txt:        cells cannot respond to the IGF-I so do not transform.
stringsearch-data/technical/biomed/1471-2105-3-17.txt:        where the inherent error of measures cannot be accurately
stringsearch-data/technical/biomed/1471-2105-3-17.txt:          control state, and which cannot be ascribed to chance or
stringsearch-data/technical/biomed/1471-2105-3-16.txt:        method cannot identify genes that are functionally related,
stringsearch-data/technical/biomed/1476-072X-2-3.txt:        this study region? We cannot exclude any particular
stringsearch-data/technical/biomed/ar140.txt:        (CD45RO +, CD27 +) CD4 +T cells cannot secrete IL-4 after a
stringsearch-data/technical/biomed/ar140.txt:        possibility cannot be the full explanation of the current
stringsearch-data/technical/biomed/ar140.txt:        obtain a polarized cytokine secretion profile that cannot
stringsearch-data/technical/biomed/ar140.txt:        these cells cannot produce IL-4 and few produce IFN-γ in
stringsearch-data/technical/biomed/gb-2003-4-3-r17.txt:          r -values. While we cannot be sure
stringsearch-data/technical/biomed/gb-2003-4-3-r17.txt:          Heterogeneous dissection cannot account for most of
stringsearch-data/technical/biomed/gb-2003-4-3-r17.txt:          most of the differences observed. However, we cannot rule
stringsearch-data/technical/biomed/gb-2003-4-3-r17.txt:          expression of X-inactivated polymorphic alleles cannot
stringsearch-data/technical/biomed/1471-2172-2-3.txt:          cells, although we cannot exclude the possibility that
stringsearch-data/technical/biomed/1471-2172-2-3.txt:          of the larger isoform cannot be attributed solely to a
stringsearch-data/technical/biomed/1471-213X-1-4.txt:        lacZ expression, which cannot be
stringsearch-data/technical/biomed/gb-2002-3-12-research0080.txt:          this category. We cannot at present distinguish whether
stringsearch-data/technical/biomed/cc1476.txt:          can also increase due to bronchodilation. We cannot
stringsearch-data/technical/biomed/cc1476.txt:          airway obstruction, we cannot be certain whether we have
stringsearch-data/technical/biomed/1471-2202-1-1.txt:        We cannot exclude the possibility that labelled vesicles
stringsearch-data/technical/biomed/1472-6750-2-13.txt:          primer-binding sites. Therefore a "chain reaction" cannot
stringsearch-data/technical/biomed/cc2172.txt:        i response among individuals cannot
stringsearch-data/technical/biomed/cc2172.txt:        levels and for longer durations cannot be completely
stringsearch-data/technical/biomed/1471-213X-1-9.txt:        the IAP insert itself cannot be regarded as a specific
stringsearch-data/technical/biomed/gb-2002-3-12-research0072.txt:          mean (-77.75). RSS flanking pseudogenes cannot be
stringsearch-data/technical/biomed/gb-2002-3-12-research0072.txt:        has not yet been, or perhaps cannot be, experimentally
stringsearch-data/technical/biomed/1472-6963-3-11.txt:        surgery cannot be reduced, because each piece of
stringsearch-data/technical/biomed/1475-4924-1-10.txt:          Such a model cannot accommodate our observations with the
stringsearch-data/technical/biomed/1472-6874-2-13.txt:        given analyte cannot be increased through improving study
stringsearch-data/technical/biomed/1471-2121-2-12.txt:        that GSK3α cannot substitute for GSK3β in this model
stringsearch-data/technical/biomed/1475-925X-2-6.txt:        distribution of the magnetic fields cannot be effectively
stringsearch-data/technical/biomed/1471-2148-1-14.txt:        (the asparagine) cannot occur with most other alignments of
stringsearch-data/technical/biomed/1471-2407-2-19.txt:        progression has not been fully elucidated and cannot simply
stringsearch-data/technical/biomed/1471-2407-2-31.txt:        have taken and cannot rule out the possibility that cases
stringsearch-data/technical/biomed/gb-2003-4-1-r5.txt:        UV cross-linking cannot be overemphasized.
stringsearch-data/technical/biomed/gb-2003-4-1-r5.txt:        cannot discount the possibility that alternative attachment
stringsearch-data/technical/biomed/1471-2156-2-12.txt:            these very old mice cannot be ruled out [ 49 ] . The
stringsearch-data/technical/biomed/1471-2156-2-12.txt:          was used at very low intensity and was dim but we cannot
stringsearch-data/technical/biomed/1472-6963-3-7.txt:        resource use and their time course and thus cannot help
stringsearch-data/technical/biomed/1472-6963-3-7.txt:        data in an economic analysis cannot be ignored. As noted
stringsearch-data/technical/biomed/1472-6963-3-7.txt:        uncertainty in these estimates cannot be quantified because
stringsearch-data/technical/biomed/1472-6963-3-7.txt:        health care decision makers in Canada, who cannot wait for
stringsearch-data/technical/biomed/1472-6963-3-7.txt:        level, economic factors cannot be ignored. In order to
stringsearch-data/technical/biomed/1471-2091-2-5.txt:        tryptophan itself cannot induce IDO synthesis [ 5]. IDO is
stringsearch-data/technical/biomed/1471-2091-2-5.txt:        modulating various cellular processes in a way that cannot
stringsearch-data/technical/biomed/1475-4924-1-5.txt:        biological samples, we cannot infer the profiles of unique
stringsearch-data/technical/biomed/1471-2202-2-19.txt:        Moreover this difference in density and orderliness cannot
stringsearch-data/technical/biomed/1471-2202-2-19.txt:        Therefore we conclude that differences in structure cannot
stringsearch-data/technical/biomed/1471-2091-3-13.txt:        carry out DNA cleavage-religation, Top67 by itself cannot
stringsearch-data/technical/biomed/1471-2164-4-14.txt:        T transcripts cannot be produced from
stringsearch-data/technical/biomed/1471-2164-3-35.txt:        same, one cannot be certain that the similarity of the
stringsearch-data/technical/biomed/1471-2164-3-35.txt:        are nearly the same, one cannot be certain that the
stringsearch-data/technical/biomed/1471-2164-3-35.txt:          model cannot be used to fit the data, due to near
stringsearch-data/technical/biomed/bcr273.txt:          or premalignant tissues. Although we cannot eliminate the
stringsearch-data/technical/biomed/bcr273.txt:          we cannot rule out more subtle effects on TGF-β activity,
stringsearch-data/technical/biomed/bcr273.txt:          certainly cannot rule out the possibility that tamoxifen
stringsearch-data/technical/biomed/bcr273.txt:        expression of TGF-βs. Although we cannot rule out more
stringsearch-data/technical/biomed/1471-2164-3-23.txt:          produces cannot be easily attributed to chance. A broader
stringsearch-data/technical/biomed/1471-2164-3-23.txt:          levels cannot be re-scaled by the reciprocal square root
stringsearch-data/technical/biomed/gb-2002-3-12-research0071.txt:          because the difference between estimates cannot exceed
stringsearch-data/technical/biomed/gb-2002-3-12-research0071.txt:           above. This model cannot be directly implemented
stringsearch-data/technical/biomed/1471-2180-1-33.txt:          not shown). Thus the restoration of β-hemolysis cannot be
stringsearch-data/technical/biomed/1471-2180-1-33.txt:        recovered following mouse passage cannot be explained by
stringsearch-data/technical/biomed/gb-2001-3-1-research0005.txt:        expression from noise cannot be overemphasized, no
stringsearch-data/technical/biomed/bcr45.txt:          the basis of mutational analysis. Such alterations cannot
stringsearch-data/technical/biomed/bcr45.txt:        basis of mutational analysis. Such alterations cannot be
stringsearch-data/technical/biomed/1471-2105-3-18.txt:        . However, both approaches are approximate and cannot
stringsearch-data/technical/biomed/1471-2105-3-18.txt:          cannot do worse than 
stringsearch-data/technical/biomed/1471-2261-3-5.txt:        events are few. While we cannot claim such a relationship
stringsearch-data/technical/biomed/1471-2261-3-5.txt:        correlations difficult. Importantly, we cannot conclude
stringsearch-data/technical/biomed/gb-2002-3-5-research0024.txt:        fusion and fission are comparable. It cannot be ruled out
stringsearch-data/technical/biomed/gb-2002-3-5-research0025.txt:          [ 40]. Thus, low selection pressure cannot account for
stringsearch-data/technical/biomed/gb-2002-3-5-research0025.txt:        Although the origin of the GshA gene cannot be
stringsearch-data/technical/biomed/1471-2199-3-3.txt:          cannot be phosphorylated by Cdc5 should not allow release
stringsearch-data/technical/biomed/1471-2121-2-10.txt:        cannot be used before cells have been fixed, as non-ionic
stringsearch-data/technical/biomed/1471-2121-2-10.txt:          other methods cannot be stained with certain
stringsearch-data/technical/biomed/1471-2121-2-10.txt:          cannot be used as the sole criterion for cytoskeletal
stringsearch-data/technical/biomed/1471-2105-2-1.txt:          cannot be rejected with the given sequence data. As a
stringsearch-data/technical/biomed/1472-684X-2-2.txt:        sedation cannot compensate personal palliative support and
stringsearch-data/technical/biomed/1471-2180-1-26.txt:        involved for survival cannot be calculated. This approach
stringsearch-data/technical/biomed/1472-6963-3-13.txt:        of statin drugs in high-risk patients cannot rely solely on
stringsearch-data/technical/biomed/1475-9268-1-1.txt:          cannot enhance the fidelity appropriate MII segregation,
stringsearch-data/technical/biomed/cc2160.txt:        the acute phase of SAH [ 1 6 ] . However, one cannot refute
stringsearch-data/technical/biomed/1471-2164-3-32.txt:        database cannot be mapped to Incyte clones, and are
stringsearch-data/technical/biomed/1471-2180-3-4.txt:        planet, and conditions across its surface vary. We cannot
stringsearch-data/technical/biomed/1471-2180-3-4.txt:        results. They cannot prove the absence of life since there
stringsearch-data/technical/biomed/gb-2003-4-6-r39.txt:        the course of nematode evolution. Consequently, one cannot
stringsearch-data/technical/biomed/gb-2003-4-6-r39.txt:          ancestral species. Although it cannot be known if these
stringsearch-data/technical/biomed/1471-2458-2-25.txt:              parts of their body, you still cannot tell whether
stringsearch-data/technical/biomed/1471-2458-2-25.txt:        health care providers' and staff attitudes cannot be
stringsearch-data/technical/biomed/gb-2003-4-9-r57.txt:          contrast, we cannot exclude the possibility that some
stringsearch-data/technical/biomed/1472-6947-2-7.txt:          cannot readily communicate with each other. This lack of
stringsearch-data/technical/biomed/gb-2002-3-5-research0021.txt:        possibility cannot be ruled out at this time. The
stringsearch-data/technical/biomed/1471-2199-3-7.txt:          polyphosphates in Hnt2+ cultures cannot be attributed to
stringsearch-data/technical/biomed/1475-2867-3-2.txt:        Since the protein cannot be inactivated by phosphorylation
stringsearch-data/technical/biomed/1475-2867-3-2.txt:          mutated form of the protein which cannot be
stringsearch-data/technical/biomed/1475-925X-2-1.txt:        means that their results usually cannot be directly related
stringsearch-data/technical/biomed/1471-2105-3-34.txt:        finds portions of a network that cannot be connected using
stringsearch-data/technical/biomed/1471-2105-3-34.txt:        interactions cannot be "created" by the algorithm, but
stringsearch-data/technical/biomed/rr37.txt:        cannot be adequately examined [ 4, 5, 6, 7, 8, 15, 16, 17,
stringsearch-data/technical/biomed/gb-2001-3-1-research0001.txt:        some tissues and cells, has characteristics that cannot be
stringsearch-data/technical/biomed/gb-2001-3-1-research0001.txt:          glycerol facilitator [ 23], cannot be significant in
stringsearch-data/technical/biomed/gb-2001-3-1-research0001.txt:        still limited. One limitation is that we cannot yet
stringsearch-data/technical/biomed/1471-2172-2-9.txt:          peristaltic pump is that the pump rate cannot be changed
stringsearch-data/technical/biomed/1471-2172-2-9.txt:          in Fig. 1Dcannot be used to produce shear curves.
stringsearch-data/technical/biomed/1471-2180-3-5.txt:        cannot be isolated [ 25 ] .
stringsearch-data/technical/biomed/1471-2288-2-10.txt:          cannot be influenced by the results.
stringsearch-data/technical/biomed/1471-2288-2-10.txt:        before data analysis. Meta-analysis cannot be thought of as
stringsearch-data/technical/biomed/1471-2164-3-4.txt:          it cannot be decided to what extent these closer
stringsearch-data/technical/biomed/1471-2164-3-4.txt:        Many relationships among prokaryotes cannot be depicted
stringsearch-data/technical/biomed/1472-6793-3-3.txt:          in ser 16-HSP20 phosphorylation cannot be explained by
stringsearch-data/technical/biomed/1471-2202-3-4.txt:          from a covalent interaction, we cannot rule out other
stringsearch-data/technical/biomed/1472-6750-2-14.txt:          effect. Although we cannot completely account for the
stringsearch-data/technical/biomed/cc1495.txt:        compensation cannot be as effective and hypotension may
stringsearch-data/technical/biomed/1471-2091-3-17.txt:          2  SO-water mixtures cannot be ruled
stringsearch-data/technical/biomed/1471-2091-3-17.txt:        2  A, HA -and A =cannot be determined
stringsearch-data/technical/biomed/1471-2164-3-19.txt:        and 2 falling within the overlap region cannot easily be
stringsearch-data/technical/biomed/1471-2164-3-19.txt:            cannot be distinguished. A ROC curve representing a
stringsearch-data/technical/biomed/gb-2002-3-12-research0088.txt:        analysis cannot document this spatial information. One can
stringsearch-data/technical/biomed/1471-2164-3-31.txt:          While we cannot estimate Z and e directly, we can
stringsearch-data/technical/biomed/1472-6963-3-14.txt:          whole; we cannot simply test individual claims in
stringsearch-data/technical/biomed/1472-6963-3-14.txt:            RCTs cannot stand apart from basic science. Even when a
stringsearch-data/technical/biomed/1472-6963-3-14.txt:            event, we cannot simply accept that pure water (in the
stringsearch-data/technical/biomed/1472-6963-3-14.txt:            cannot simply say that they are complementary and that
stringsearch-data/technical/biomed/1475-2875-2-4.txt:        cannot be dismissed. It is likely, then, that the
stringsearch-data/technical/biomed/1475-2875-2-4.txt:        However, arbitrary designations cannot be considered
stringsearch-data/technical/biomed/ar612.txt:        these molecules, osteoclastogenesis cannot occur [ 9 ]
stringsearch-data/technical/biomed/ar612.txt:        demonstrate that RANKL-induced osteoclastogenesis cannot be
stringsearch-data/technical/biomed/1472-6793-2-19.txt:          The data available in this study cannot discern the
stringsearch-data/technical/biomed/gb-2002-3-5-research0022.txt:          replicates cannot detect a change as large as 
stringsearch-data/technical/biomed/1471-2288-3-9.txt:          between 2.25 and 2.35, but cannot be much more precise."
stringsearch-data/technical/biomed/1471-2288-3-9.txt:          cannot determine which values are better to use, they can
stringsearch-data/technical/biomed/bcr303.txt:        results suggest that NOM cannot modulate MRP gene
stringsearch-data/technical/biomed/bcr303.txt:        on MDR in MCF7/ADR cells cannot result from modulating the
stringsearch-data/technical/biomed/1471-2105-3-23.txt:        (e.g., t-tests) cannot be used to rate the statistical
stringsearch-data/technical/biomed/1471-2105-3-23.txt:          signal from the multiple probe pairs cannot be used to
stringsearch-data/technical/biomed/1471-2105-3-23.txt:        individual samples. We cannot guarantee that the same
stringsearch-data/technical/biomed/1471-2105-3-23.txt:        but cannot compensate for variance from other sources.
stringsearch-data/technical/biomed/bcr458.txt:        rates in Marin County because it is a county, we cannot
stringsearch-data/technical/biomed/1471-2156-2-17.txt:        improbable using these fragments because we cannot examine
stringsearch-data/technical/biomed/1471-2369-4-1.txt:        fibrillation in whom NSR cannot be established is based on
stringsearch-data/technical/biomed/gb-2002-3-6-research0029.txt:        genomic DNA cannot predict untranslated regions (UTRs), and
stringsearch-data/technical/biomed/gb-2002-3-6-research0029.txt:          site. Misannealing cannot explain the presence of
stringsearch-data/technical/biomed/gb-2002-3-6-research0029.txt:          mixed before library construction, we cannot determine
stringsearch-data/technical/biomed/gb-2002-3-6-research0029.txt:          to the genome. Some programs cannot efficiently handle a
stringsearch-data/technical/biomed/1471-2121-1-2.txt:        cannot bind the SRE autonomously, but require
stringsearch-data/technical/biomed/1471-2121-1-2.txt:          levels. We cannot determine if the increase in CAT
stringsearch-data/technical/biomed/1471-2180-1-34.txt:        the mutational phenotype cannot be switched on at
stringsearch-data/technical/biomed/1471-2180-1-34.txt:        the dsRNA approach cannot be used against 
stringsearch-data/technical/biomed/1471-2164-3-30.txt:        cannot rule out genetic heterogeneity for these genes and
stringsearch-data/technical/biomed/1471-2164-3-18.txt:          hexameric ring [ 14 ] . We cannot, at present, exclude an
stringsearch-data/technical/biomed/1471-213X-1-15.txt:          However, one cannot extrapolate from mRNA abundance to
stringsearch-data/technical/biomed/1471-213X-1-15.txt:          nuclei in TNF + SN50-treated explants, and (3) one cannot
stringsearch-data/technical/biomed/1471-213X-1-15.txt:        This is so because we cannot extrapolate from transcriptome
stringsearch-data/technical/biomed/1468-6708-3-4.txt:          data cannot be dependent on either the observed or the
stringsearch-data/technical/biomed/1468-6708-3-4.txt:        cannot provide statistical tests to select the missing data
stringsearch-data/technical/biomed/1471-2121-3-25.txt:          factors or docking proteins, but cannot cycle on and off
stringsearch-data/technical/biomed/1471-2121-3-25.txt:        investigation, we cannot rule out the alternative
stringsearch-data/technical/biomed/1471-2121-3-25.txt:        consist of misfolded endogenous proteins that cannot be
stringsearch-data/technical/biomed/1472-6882-1-10.txt:          of smell and cannot be afraid to dive into hollow logs or
stringsearch-data/technical/biomed/1471-2121-3-19.txt:        appropriate thick filament array it cannot function to
stringsearch-data/technical/biomed/1471-2334-1-17.txt:        interactions discernable, such interactions cannot be ruled
stringsearch-data/technical/biomed/1471-2326-2-4.txt:        this may have caused cannot be ascertained. Finally, as
stringsearch-data/technical/biomed/1471-2180-2-16.txt:          LcrV, but cannot block secretion of Yops in 
stringsearch-data/technical/biomed/1471-2121-4-1.txt:        integrity cannot exclude PI, which emits a red fluorescence
stringsearch-data/technical/biomed/1471-2121-4-1.txt:          that have lost membrane integrity cannot exclude PI,
stringsearch-data/technical/biomed/1471-213X-2-8.txt:          means that we cannot use cycloheximide sensitivity as a
stringsearch-data/technical/biomed/1471-213X-2-8.txt:        induction cannot be controlled easily.
stringsearch-data/technical/biomed/1471-2199-4-5.txt:        nuclease action. Of course, we cannot exclude the
stringsearch-data/technical/biomed/1471-2199-4-5.txt:        straightforward way. These null mutant enzymes cannot
stringsearch-data/technical/biomed/1471-2199-4-5.txt:        recombination [ 6 ] . We assume that they cannot repair the
stringsearch-data/technical/biomed/1471-2199-4-5.txt:        that they cannot degrade them into smaller pieces. The 
stringsearch-data/technical/biomed/1471-2202-2-1.txt:        staining which, however, cannot easily be assigned to
stringsearch-data/technical/biomed/1471-2202-2-1.txt:          From our results we cannot eliminate T5 cells as
stringsearch-data/technical/biomed/1472-6882-1-11.txt:        world's population cannot afford the therapy, and further
stringsearch-data/technical/biomed/1471-2121-3-30.txt:          cannot rule out the possibility that a second set of
stringsearch-data/technical/biomed/1471-2199-2-3.txt:        Table 2). Although we cannot rule out a marginal effect of
stringsearch-data/technical/biomed/1471-2199-2-3.txt:        this possibility cannot be explored further for the time
stringsearch-data/technical/biomed/1471-2199-2-3.txt:        Although the nature of these interactions cannot be deduced
stringsearch-data/technical/biomed/1471-2121-2-6.txt:        between these two possibilities cannot be conducted until a
stringsearch-data/technical/biomed/1475-2891-1-2.txt:          shown in Figure 3A, as compared to Figure 3B, cannot be
stringsearch-data/technical/biomed/1471-2105-1-1.txt:        biological processes cannot be analyzed or predicted based
stringsearch-data/technical/biomed/gb-2002-3-10-research0052.txt:        cannot be determined computationally in the absence of the
stringsearch-data/technical/biomed/gb-2002-3-10-research0052.txt:        model which cannot explain multiply inverted elements. The
stringsearch-data/technical/biomed/gb-2001-2-12-research0055.txt:        they cannot be log-transformed, a manipulation that is a
stringsearch-data/technical/biomed/1471-2210-1-4.txt:          antimuscarinic effects alone cannot account for all of
stringsearch-data/technical/biomed/1471-2210-1-4.txt:        Therefore, peripheral anti-muscarinic effects alone cannot
stringsearch-data/technical/biomed/1476-511X-2-3.txt:        groups. The present study cannot provide causal inference
stringsearch-data/technical/biomed/1476-511X-2-3.txt:        Our study is a cross section survey. Thus, we cannot
stringsearch-data/technical/biomed/1476-511X-2-3.txt:        addition, the influence of diet and genetic factors cannot
stringsearch-data/technical/biomed/1476-4598-2-28.txt:        SMAD pathway, but also because they cannot complete the
stringsearch-data/technical/biomed/1471-2121-4-3.txt:          removal from PP5 [ 19 20 ] . Although we cannot rule out
stringsearch-data/technical/biomed/1471-2105-3-2.txt:            sequences contain subsequences that cannot be aligned
stringsearch-data/technical/biomed/1471-2105-3-2.txt:            we do have sequence information but cannot fully
stringsearch-data/technical/biomed/1471-2105-3-2.txt:            cannot be subclassified as IB1, IB2, IB3, or IB4. Those
stringsearch-data/technical/biomed/1471-2229-2-11.txt:          allele, because we cannot distinguish between the L91'
stringsearch-data/technical/biomed/1472-6882-1-12.txt:        criteria we cannot be sure that other validity scoring were
stringsearch-data/technical/biomed/gb-2002-3-10-research0053.txt:          be computed for rice, we cannot presently equate %LNI
stringsearch-data/technical/biomed/1471-2148-3-3.txt:        function cannot be destroyed twice. In effect, one mutation
stringsearch-data/technical/biomed/1471-2148-3-3.txt:        mutations cannot be ignored if their frequency varies
stringsearch-data/technical/biomed/1472-6807-2-9.txt:        certain tripeptides. At the outset, we cannot make any
stringsearch-data/technical/biomed/1477-7827-1-36.txt:        approach cannot demonstrate coexpression of the ERs in a
stringsearch-data/technical/biomed/1477-7827-1-36.txt:        trophoblast cells in vivo cannot be achieved in vitro,
stringsearch-data/technical/biomed/1471-213X-1-13.txt:          isl1 [ 46]. Currently, we cannot
stringsearch-data/technical/biomed/1471-2199-2-4.txt:          per se , although we cannot exclude
stringsearch-data/technical/biomed/gb-2000-1-2-research0003.txt:        single reordering of the samples for all genes, cannot find
stringsearch-data/technical/biomed/gb-2000-1-2-research0003.txt:        aspects are important and cannot be captured by simple
stringsearch-data/technical/biomed/1472-6955-2-1.txt:          body within and between site agreement cannot be assumed.
stringsearch-data/technical/biomed/1472-6955-2-1.txt:          assessment. This conclusion, however, cannot be made
stringsearch-data/technical/biomed/1472-6947-1-6.txt:        Fifth, this study cannot assess the independence of
stringsearch-data/technical/biomed/1472-6947-1-6.txt:        diagnostic accuracy. Thus, the findings cannot be related
stringsearch-data/technical/biomed/1472-6947-1-6.txt:        with high specificity. Thus, physical signs cannot be used
stringsearch-data/technical/biomed/1472-6874-2-8.txt:        sequence of the c-KIT protein. However, we cannot exclude
stringsearch-data/technical/biomed/1471-2180-2-7.txt:          one cannot readily divide strains into those which form
stringsearch-data/technical/biomed/1472-6793-1-15.txt:          domain in the EC cannot be ruled-out.
stringsearch-data/technical/biomed/1471-2164-2-7.txt:          acceptor in the other. We cannot explain this finding,
stringsearch-data/technical/biomed/1471-2164-2-7.txt:        cannot demonstrate the co-existence of these intergenic
stringsearch-data/technical/biomed/gb-2001-2-12-research0051.txt:          cannot be predicted at present. However, these proteins
stringsearch-data/technical/biomed/gb-2001-2-12-research0051.txt:        cannot be proved by the success of the experiments they
stringsearch-data/technical/biomed/gb-2002-3-8-research0038.txt:        Antp ) gene cannot grow normal
stringsearch-data/technical/biomed/gb-2002-3-8-research0038.txt:        developmental phenotypes is large, we cannot assume that
stringsearch-data/technical/biomed/gb-2002-3-8-research0038.txt:        effects of the isolation procedure cannot be easily
stringsearch-data/technical/biomed/gb-2002-3-8-research0038.txt:            glec further and cannot therefore
stringsearch-data/technical/biomed/1468-6708-3-3.txt:        cannot be ignored given the wide confidence intervals (and
stringsearch-data/technical/biomed/1472-6947-3-5.txt:        Description, etc.) cannot be sensibly indexed or shared.
stringsearch-data/technical/biomed/1476-4598-1-5.txt:        contribute but cannot be simply and directly linked.
stringsearch-data/technical/biomed/1471-2458-3-11.txt:        indicate that clinically important findings cannot be
stringsearch-data/technical/biomed/1477-7827-1-31.txt:          actions cannot be dismissed as non-specific, because 4-AP
stringsearch-data/technical/biomed/1477-7827-1-31.txt:          resting membrane potential cannot be explained easily by
stringsearch-data/technical/biomed/gb-2002-3-3-research0011.txt:          experiment vectors cannot be visualized, the
stringsearch-data/technical/biomed/gb-2002-3-3-research0011.txt:          matrix and cannot adequately be constructed by other
stringsearch-data/technical/biomed/gb-2002-3-10-research0054.txt:        C. elegans cannot see or hear but
stringsearch-data/technical/biomed/1476-9433-1-2.txt:        other cytokines cannot compensate for IL-2 in the IL-2
stringsearch-data/technical/biomed/1478-1336-1-2.txt:        such differences cannot account for the results with
stringsearch-data/technical/biomed/1478-1336-1-2.txt:        cannot directly activate CAR targets. More complex
stringsearch-data/technical/biomed/1471-2202-3-16.txt:        studies cannot yet be performed at a high throughput level
stringsearch-data/technical/biomed/1471-2121-4-4.txt:          against both receptors cannot be readily interpreted,
stringsearch-data/technical/biomed/1471-2121-4-4.txt:          proteins directly in transfected cells, we cannot
stringsearch-data/technical/biomed/1471-2121-4-4.txt:          events. In contrast, LRP6ΔN cannot effectively substitute
stringsearch-data/technical/biomed/1477-5956-1-1.txt:        separated from KcF12, KcF6 and KcC7. While we cannot rule
stringsearch-data/technical/biomed/1471-2431-2-12.txt:          cannot be ruled out, as normal RC activities have been
stringsearch-data/technical/biomed/1471-2431-2-12.txt:          inborn error of metabolism cannot be excluded completely.
stringsearch-data/technical/biomed/1471-2431-2-12.txt:        and we cannot completely exclude the possibility of an
stringsearch-data/technical/biomed/ar328.txt:        P = 0.001) [ 33]. We cannot explain
stringsearch-data/technical/biomed/1471-2121-4-5.txt:        cannot determine the causal relationship between loss of
stringsearch-data/technical/biomed/1471-2407-1-13.txt:        cannot compare our results directly because of difference
stringsearch-data/technical/biomed/bcr605.txt:        physical activity in the interview, we cannot assess the
stringsearch-data/technical/biomed/bcr605.txt:        (but cannot completely rule out) the hypothesis that there
stringsearch-data/technical/biomed/1478-1336-1-3.txt:        7 ] . We cannot rule out, however, that Stat3 is affecting
stringsearch-data/technical/biomed/1471-2202-4-2.txt:          (P0, P8, P10). Thus the factor(s) cannot be released by
stringsearch-data/technical/biomed/1471-2172-3-9.txt:        cytotoxicity cannot be overlooked.
stringsearch-data/technical/biomed/gb-2002-3-10-research0055.txt:          meaningful groups of genes cannot be attributed to a
stringsearch-data/technical/biomed/gb-2002-3-10-research0055.txt:          previously published, our technique cannot be expected to
`
    2.  The following example searches for and returns all lines which contain the word *cannot* in all files under and the given directory and its subdirectories:<br>
        input: `grep -r "fruit" stringsearch-data/technical/government` <br>
        output: ```stringsearch-data/technical/government/About_LSC/Strategic_report.txt:also witnessed the fruition of prior efforts.
stringsearch-data/technical/government/About_LSC/commission_report.txt:of fruits and vegetables of every kind and other perishable
stringsearch-data/technical/government/About_LSC/commission_report.txt:apples (4,428), vegetable harvesting (4,822), and fruit harvesting
stringsearch-data/technical/government/Env_Prot_Agen/final.txt:recently borne fruit, particularly recent agreements with Japan and
stringsearch-data/technical/government/Alcohol_Problems/DraftRecom-PDF.txt:screening were not as fruitful topics for research as how to screen
stringsearch-data/technical/government/Gen_Account_Office/July11-2001_gg00172r.txt:fruition.
stringsearch-data/technical/government/Media/Unusual_Woodburn.txt:lettuce and chile harvests from the Central Valley to the fruit and
stringsearch-data/technical/government/Media/Farm_workers.txt:tending and harvesting fruits and vegetables.``` 
