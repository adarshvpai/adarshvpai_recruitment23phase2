## Automotive
## Car Hacking Handbook
Chapter-1 Understanding Threat Models
1. Attack Surfaces: The chapter begins by explaining the concept of an attack surface, which refers to all the possible ways to attack a target, 
from vulnerabilities in individual components to those that affect the entire vehicle. It emphasizes that when discussing the attack surface,
the focus is on entry points into the target rather than how to exploit it.
2. Evaluating Attack Surfaces: To find weaknesses in a vehicle's security, the chapter suggests thinking like an attacker and evaluating the vehicle's 
perimeter. This involves considering all the ways data can enter a vehicle, such as through radio waves, key fobs, sensors, diagnostic ports, and more.
3. Threat Modeling: Threat modeling is introduced as a crucial process for identifying potential risks and vulnerabilities in a target system. It involves
creating diagrams to illustrate how parts of the car communicate, identifying higher-risk inputs, and maintaining a checklist of things to audit. Threat
models are dynamic documents that change as the target system evolves.
4. Threat Model Levels: Threat models can have different levels of complexity. The chapter introduces three levels: Bird's-Eye View (Level 0), Receivers 
(Level 1), and Receiver Breakdown (Level 2). These levels allow for increasingly detailed analysis of the system's communication and vulnerabilities.
5. DREAD Rating System: The chapter presents the DREAD rating system, which stands for Damage potential, Reproducibility, Exploitability, Affected users,
and Discoverability. Each category is assigned a score to assess the risk level of a specific threat.
6. Working with Threat Model Results: Depending on whether you're on the attacker (red team) or defender (blue team) side, the chapter explains how to use 
the threat model results. The red team would prioritize attacking high-risk areas, while the blue team would implement countermeasures to mitigate the 
identified risks.
7. Summary: The chapter concludes by summarizing the importance of threat modeling in identifying and addressing security vulnerabilities, emphasizing that
 threat models are dynamic documents that require regular updates.
