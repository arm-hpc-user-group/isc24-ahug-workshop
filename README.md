# Arm HPC User Group Workshop @ ISC24

The 2024 Arm HPC User Group (AHUG) Workshop is held in conjunction with [**ISC High Performance 2024**](https://www.isc-hpc.com/) in Hamburg, Germany. 

**Date & Time**: May 16th, 2024 @ 9:00am - 1:00pm <br>
**Location**: Hall Y10 - 2nd floor, Congress Center Hamburg (CCH), Germany

[**Join the AHUG Slack channel!**](https://join.slack.com/t/a-hug/shared_invite/zt-25r69qm2u-hhEkbN7terYpw7K3W2k6Eg)

## Timetable and agenda 

<table>
<colgroup>
<col width="10%" />
<col width="10%" />
<col width="40%" />
<col width="23%" />
<col width="17%" />
</colgroup>
<thead>
<tr class="header">
<th>Time</th>
<th>Duration</th>
<th>Title</th>
<th>Speaker</th>
<th>Affiliation</th>
</tr>
</thead>
<tbody>
<tr>
<td markdown="span">09:00-09:10</td>
<td markdown="span">10m</td>
<td markdown="span">**Welcome Remarks & Plenary Address to the AHUG Community**</td>
<td markdown="span">Filippo Spiga</td>
<td markdown="span">AHUG</td>
</tr>
<tr>
<td markdown="span">09:10-09:45</td>
<td markdown="span">35m</td>
<td markdown="span"><font size="-1">Invited Talk</font><br>
**Isambard-3 and Isambard-AI**</td>
<td markdown="span">Simon McIntosh-Smith</td>
<td markdown="span">University of Bristol / GW4</td>
</tr>
<tr>
<td markdown="span">09:45-10:10</td>
<td markdown="span">25m</td>
<td markdown="span">**Performance analyses of benchmark applications on different A64FX architectures**</td>
<td markdown="span">Seydou Ba</td>
<td markdown="span">RIKEN R-CCS</td>
</tr>
<tr>
<td markdown="span">10:10-10:35</td>
<td markdown="span">25m</td>
<td markdown="span">**NVIDIA Grace Superchip Early Evaluation for HPC Applications**</td>
<td markdown="span">Fabio Banchelli</td>
<td markdown="span">BSC</td>
</tr>
<tr>
<td markdown="span">10:35-11:00</td>
<td markdown="span">25m</td>
<td markdown="span">**Accelerating Hierarchical Collective Communication on next-gen ARM architectures**</td>
<td markdown="span">Alon Zameret</td>
<td markdown="span">Toga Networks - Huawe</td>
</tr>
<tr>
<td markdown="span">11:00-11:30</td>
<td markdown="span">30m</td>
<td colspan="3" markdown="span">_Coffee break_</td>
</tr>
<tr>
<td markdown="span">11:30-11:55</td>
<td markdown="span">25m</td>
<td markdown="span">**Running Arm Accelerated Solutions for Engineering Workflows in the Cloud with Rescale**</td>
<td markdown="span">Sam Zakrzewski</td>
<td markdown="span">Rescale</td>
</tr>
<tr>
<td markdown="span">11:55-12:20</td>
<td markdown="span">25m</td>
<td markdown="span">**Extending Arm's Reach by Going EESSI**</td>
<td markdown="span">Kenneth Hoste</td>
<td markdown="span">Ghent University</td>
</tr>
<tr>
<td markdown="span">12:20-12:40</td>
<td markdown="span">20m</td>
<td markdown="span"><font size="-2">Silicon Update</font><br>
**NVIDIA Grace Superchip**</td>
<td markdown="span">Filippo Spiga</td>
<td markdown="span">NVIDIA</td>
</tr>
<tr>
<td markdown="span">12:40-13:00</td>
<td markdown="span">20m</td>
<td markdown="span"><font size="-2">Silicon Update</font><br>
**AWS Graviton 3/3E/4**</td>
<td markdown="span">TBD</td>
<td markdown="span">AWS</td>
</tr>
</tbody>
</table>

## Abstracts

### Performance analyses of benchmark applications on different A64FX architectures
**Speaker**: Seydou Ba (RIKEN R-CCS)

_Modern supercomputers are increasingly complex and are utilizing faster and denser core count processors per node. This work focuses on the performance comparison of different node architectures of Fujitsu's A64FX, namely the FX1000 (Fugaku) and two versions of the FX700. The architectures differ mainly in that, the FX1000 has 48cores per node and uses the TofuD interconnect, while the FX700s use Infiniband and one version has 48cores per node and the other has 24cores per node at a higher frequency.  We are monitoring performance with profilers and analysis tools to conduct detailed performance studies with key benchmark applications.  Furthermore, we aim to expend this study with the purpose of  analyzing hardware option for interconnections leaning toward photonics design for next-gen supercomputers._

### NVIDIA Grace Superchip Early Evaluation for HPC Applications 
**Speaker**: Fabio Banchelli (BSC)

_Arm-based system in HPC are a reality since more than a decade. However, when a new chip enters the market always implies challenges, not only at ISA level, but also with regards to the SoC integration, the memory subsystem, the board integration, the node interconnection, and finally the OS and all layers of the system software (compiler and libraries). Guided by the procurement of an NVIDIA Grace HPC cluster within the deployment of MareNostrum 5, and emulating the approach of a scientist who needs to migrate its scientific research to a new HPC system, we evaluated five complex scientific applications on engineering sample nodes of NVIDIA Grace CPU Superchip and NVIDIA Grace Hopper Superchip (CPU-only). We report intra-node and inter-node scalability and early performance results showing a speed-up between 1.3x and 4.28x for all codes when compared to the current generation of MareNostrum 4 powered by Intel Skylake CPUs._

### Accelerating Hierarchical Collective Communication on next-gen ARM architectures
**Speaker**: Alon Zameret (Toga Networks - Huawei)

_In large-scale distributed computing, collective communication often poses a bottleneck due to the latency and bandwidth limitations of modern networks. In this work we propose an innovative hierarchical approach to accelerate collective communication, based on multiple levels of communication aggregation (intra-node, inter-node, inter-rack). Assigning multiple representatives at each level enables communication and data partitioning for alleviating latency/bandwidth bounds in HPC and AI applications. Leveraging the SIMD extensions (e.g. SVE) offered in next-generation ARM architectures further improves performance by optimizing memory copy and reduction operations. The resulting communication component, MLMR, demonstrates up to 5x reduction of AllReduce collective communication on an ARM cluster with more than 12k cores. Further work is underway to introduce payload pipelining in order to overlap inter-level communication, and enhance performance._


### Running Arm Accelerated Solutions for Engineering Workflows in the Cloud with Rescale
**Speaker**: Sam Zakrzewski (Rescale)

_As computational demands in engineering continue to rise, leveraging cloud computing resources becomes increasingly imperative. This presentation delves into the optimization and efficiency gains achieved by running engineering workflows in the cloud on Arm-based hardware through Rescale's platform. Case studies and demonstrations illustrate how Rescale's platform enables seamless migration of engineering workflows to Arm-based cloud instances, unlocking unparalleled performance and cost-effectiveness. Key topics covered include the technical considerations of transitioning to Arm architecture, performance benchmarks and cost comparisons illustrating the economic benefits of cloud-based Arm computing. Attendees will gain a comprehensive understanding of how adopting Arm accelerated solutions for engineering workflows on Rescale's platform empowers organizations to tackle complex simulations with unprecedented efficiency, driving innovation and competitiveness._

### Extending Arm's Reach by Going EESSI
**Speaker**: Kenneth Hoste (University of Genth)

_In the European Environment for Scientific Software Installation (EESSI) community project (https://eessi.io), we provide a stack of optimized scientific software installations that work on any Linux system, regardless of whether it is powered by Intel, AMD, or Arm CPUs (soon also RISC-V). This effort is currently funded through the EuroHPC Centre-of-Excellence MultiXscale (https://multixscale.eu). In this talk, we will share our experiences with building a wide range of scientific applications, libraries, and required dependencies for different Arm microarchitectures. We encountered (and fixed) various problems along the way, especially when targetting Arm Neoverse V1, and when running software test suites. Additionally, we will demonstrate how you can get access in a matter of minutes to a rich set of optimized software installations for Arm systems, including Raspberry PI's, cloud instances powered by an Arm CPU, and Arm-based EuroHPC supercomputers like Deucalion and JUPITER._