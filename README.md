# Uncertainty-aware Specification and Analysis for Hardware-in-the-Loop Testing of Cyber Physical Systems


## Contributors 
    
* Seung Yeob Shin (seungyeob.shin@uni.lu), SnT Centre, University of Luxembourg, Luxembourg  
* Karim Chaouch (karim.chaouch@uni.lu), SnT Centre, University of Luxembourg, Luxembourg  
* Shiva Nejati (snejati@uottawa.ca), University of Ottawa, Canada & SnT Centre, University of Luxembourg, Luxembourg  
* Mehrdad Sabetzadeh (m.sabetzadeh@uottawa.ca), University of Ottawa, Canada & SnT Centre, University of Luxembourg, Luxembourg  
* Lionel C. Briand (lionel.briand@uni.lu), SnT Centre, University of Luxembourg, Luxembourg & University of Ottawa, Canada
* Frank Zimmer (frank.zimmer@ses.com), SES Networks, Luxembourg  

## Project artifacts

This page contains the artifacts related to an article entitled "Uncertainty-aware Specification and Analysis for Hardware-in-the-Loop Testing of Cyber Physical Systems" submitted to the Journal of Systems and Software.

### HITECS language grammar
* ./grammar  
  We extend the UML Testing Profile (UTP), UML Uncertainty Profile (UUP), and UML action language (Alf) to define the HITECS language for hardware-in-the-loop (HiL) testing of cyber physical systems (CPS). The HITECS grammar is described in the Xtext grammar definition language and builds on the Alf grammar in the Xtext format used in Papyrus (see https://www.eclipse.org/papyrus/). The HITECS grammar file is fully described and is ready to be used for developing an Xtext-based HITECS editor (see https://www.eclipse.org/Xtext/).


### HITECS specifications
* ./specifications  
  We have evaluated HITECS by applying it to an industrial case study, in-orbit satellite testing. We note that the specifications are sanitized due to the confidentiality reasons of our industry partner.  
  This artifact contains the HITECS specifications of our industrial case study under the following directories:  
  - ./specifications/HITECS/Component:  
    Containing HiL component specifications. A HiL component is either the system under test or a (peripheral) test instrument required to execute a HiL test case.  
  - ./specifications/HITECS/PhysicalBehavior:  
    Containing physical behavior specifications. A physical behavior of a HiL component is specified as a mathematical function.
  - ./specifications/HITECS/TestCase:  
    Containing HiL test case specifications. A HiL test case specifies test properties (inputs, outputs, and HiL components), a set of test operations, assertions, simulation annotations, and a test oracle.  
  - ./specification/HITECS/Activity:  
    Containing activity specifications. An activity specifies operation calls over HiL components.  
  - ./specifications/HITECS/MeasurementFormula:  
    Containing measurement formula specifications. A measurement formula of a HiL test case is specified as a formular to measure a state value of test instruments, SUT, or test environments.
  - ./specification/HITECS/TestSuite:  
    Containing HiL test suite specifications. A HiL test suite is an ordered list of test cases.  
  - ./specification/HITECS/Scheduler:  
    Containing HiL test scheduler specifications. A HiL test scheduler is a procedure that defines the execution order of a test suite.


### Experiment results of RQ1 and RQ2
* ./experiments/RQ1_RQ2  
  RQ1 (assertion guidelines): Are our guidelines for defining well-behavedness assertions useful?  
  RQ2 (model checking): Can HITECS verify HiL test case assertions in practical time?  
  We used 609 non-equivalent mutants to answer RQ1 and RQ2. This directory contains all the experiment outputs (model_checking.xlsx) related to Table 9 and Figure 19.


### Experiment results of RQ3
* ./experiments/RQ3  
  RQ3 (uncertainty resolution): Can HITECS identify conditions on unknown parameters of HiL test cases under which HiL test cases are conclusively well-behaved?  
  We used 10000 samples and 10000 decision trees to answer RQ3. This directory contains all the experiment outputs related to Table 11 (see identified_conditions.xlsx) and Figure 20 (see J48.xlsx, SimpleCart.xlsx, and REPTree.xlsx).


### Experiment results of RQ4
* ./experiments/RQ4  
  RQ4 (simulation): Can HITECS accurately estimate the execution times of HiL test cases via simulation?
  We used 3000 simulation runs to answer RQ4. This directory contains all the simulated execution time estimates and the actual execution time values obtained from the historical data (see simulation.xlsx). Figure 21 visually compares the two sets of execution time values in the artifact.


## HITECS tool
* HITECS tool is available upon request.  
  Contact: Karim Chaouch (karim.chaouch@uni.lu) and Seung Yeob Shin (seungyeob.shin@uni.lu)

## Licensing
This software is © University of Luxembourg and is licensed under the GPLv3 license. See COPYING.txt.
