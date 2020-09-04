# Requirement Prioritization Brainstorm

The design team is tasked with answering “What are the requirements for solutions to compressing segment routing information for use over IPv6?”. This can result in a very broad set of requirements covering many aspects of compression, SR and IPv6.

Requirements for a solution to compress segment routing information for use over IPv6 can be divided into three mutually exclusive groups:

1. Requirements specific to a compression solution
1. Requirements specific to SRv6 and any other instantiation of SR for IPv6
1. Requirements specific to any protocol design

The first group of requirements is the primary objective for the design team to identify and are likely of key interest to SPRING. These requirements should be considered to be the main driver of selecting a solution. In other words, if they are not met, there is no need to select the solution.

Requirements associated with the second group will help to make the functionality of the final solution more complete. These requirements while still important for SPRING to consider, are much broader and likely better understood already within the SPRING working group.

Requirements associated with the third group aim to make the final solution more mature and practical, some of them are like design principle to some extent.

It therefore makes sense for the design team to prioritize its efforts on group 1, then 2, then 3 and document them in this order in the final documentation. The order is important for SPRING since early requirements can act as gates during the evaluation of a proposal. I.e., if a proposal does not compress well it can be identified quickly and improved or discarded.


Below is a list of requirements sorted into priority groups, this is an initial suggestion and not yet complete since requirement review is ongoing.

# Requirements Specific To Compression

Does a proposal compress well, does it do so efficiently, and can an operator migrate to it from existing SRv6 networks?

Example Candidates:

* REQ-7-27-COMPRESS
* REQ-7-28-LOSSLESS-COMPRESSION
* REQ-8-17-FWD-EFFICIENCY
* REQ-8-17-STATE-EFFICIENCY
* REQ-8-20-SRv6-to-CompSRv6-00
* REQ-8-26-SPRING-SRV6-MIGRATION-01

# Requirements Specific To SRv6 And Any Other Instantiation Of SR For IPv6

SRv6 is the current instantiation of SR for the IPv6 data plane and there are many solutions built around it and SR MPLS. Does a proposal support existing SR solutions and is it a good instantiation of SR for IPv6?

Example Candidates:

* REQ-7-27-ARCH
* REQ-7-27-SPRING-FRAMEWORK
* REQ-8-19-FLEX-ALGO
* REQ-7-31-Convergence-TILFA
* REQ-8-26-SUMM
* Scale (various)
  * REQ-9-1-LINKNODE-SCALE
  * REQ-9-1-SERVICE-SCALE
  * REQ-7-27-SVC-SCALE-00
  * REQ-8-14-GLOBAL-SIGNIFICANT-SVC-SCALE-00
  * REQ-8-14-LOCAL-SIGNIFICANT-SVC-SCALE-00
  * REQ-8-26-NETWORK-SCALE
  * REQ-7-27-SR-PATH-LENGTH-00
  * REQ-8-20-IPv6-to-CompSRv6-00
* REQ-7-28-FLEX-ADDRESS-PLANNING-00
* “Interworking Across SR Domain Boundaries”

# Requirements Specific To Any Protocol Design

How does a proposal support general best practices?

Example Candidates:

* REQ-8-26-IPV6-SECURITY-COMPLIANCE-00
* REQ-08-19-SEGMENT-LINK--LOCAL-00
* REQ-08-07-DEBUGGING-00
