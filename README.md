[autonomous-robots-safety-act.md](https://github.com/user-attachments/files/34679844/autonomous-robots-safety-act.md)
# Autonomous Robots Safety Act (Draft)

As of 11 November 2026 · Martin Vorel

A model statute for discussion, not tied to any jurisdiction. Its premise: the contents of an AI model cannot be audited, so safety must be enforced outside the model.

## Disclaimer

This text is not a bill before any parliament, not legal advice and not the work of a lawyer. It was written by a layperson as a thought experiment in the form of a statute. No court, regulator or legal professional has reviewed it.

It exists because of a concern. Societies tend to regulate a technology only after its first public disaster, and laws written in the weeks after a disaster are usually rushed, driven by fear and shaped by whoever lobbies fastest. Robots with autonomous AI will reach homes, streets, hospitals and laboratories within the working life of people alive today. The debate about who answers for them should happen before the first serious incident, in calm conditions, and in public.

Read the text with these limits in mind:

- **All figures are placeholders.** Periods, thresholds, fines and prison terms are working values chosen to make the text concrete. None of them comes from an existing law or from an impact study.
- **It cannot stop a determined individual.** A robot built at home from parts appears in no register. The Act can only punish such use afterwards.
- **It stops at the border.** Imports from jurisdictions without comparable rules, and old machines without support, remain a gap.
- **Military use is excluded** and is arguably the larger risk.
- **The Act creates a new danger of its own.** The event recorder, the register and the remote stop channel are also instruments of surveillance and control. Whoever runs them holds a lever over every household that owns a robot. This risk is comparable to the one the Act is meant to reduce, and the safeguards in Sections 10, 12, 24, 28 and 35 may not be enough.
- **Heavy rules favour large manufacturers.** Section 31 tries to keep room for hobbyists, repairers and small builders. Whether it succeeds is an open question.

The text may be shared, criticised, rewritten and taken apart. That is its purpose.

## Opening Questions and Theses

The draft grew out of a discussion. These are the questions and theses that started it.

### Questions

1. Once someone fixes a blade to a robot and sends it into a public square, who bears responsibility for what it does?
2. How will such machines be insured?
3. How can anyone control which AI model people load into a robot they own?

### Theses

1. **Awareness will come late.** Most of society will understand that a robot with autonomous AI is an easily misused object only after the first violent incident. Everything depends on how the law handles it, and the law will probably be written after the fact.
2. **A robot is an object whose security can be broken.** Once compromised, it can do physical harm in a way that software alone cannot.
3. **Models can carry hidden behaviour.** Research has documented backdoors in language models: behaviour that stays dormant until a specific sequence of words triggers it. Theoretical work shows that a neural network of this kind can be programmed to act as a general-purpose computer.
4. **Models can change other models.** Research has shown that one model can pass its tendencies to another through data that looks unrelated to them, and that targeted changes to a model's stored answers are possible.
5. **Nobody can check.** There is no reliable method for inspecting the parameters of a model and stating what is hidden in them. Combined with theses 3 and 4, this means a model in a robot has to be treated as untrusted.
6. **The laboratory case is the worst one.** An AI model with unsupervised access to a gene-editing laboratory able to engineer viruses is a risk of a different order from anything a household robot can do.
7. **We stand at a crossroads.**

### Social context from the same discussion

- Care robots are among the few workable answers to current demographic trends.
- Robots and AI companions will supplement human contact for most people and replace it mainly for those who already live without close human ties.
- The industrial revolution separated generations geographically. The AI and robotics revolution makes relationships easier to switch off, and at the same time makes it easier to keep a chosen circle of people together across distance.
- Whether an AI has only text, a voice, a face or a body is not the most important factor.

## Part I: General Provisions

### Section 1. Purpose

This Act lays down rules on the safety, liability and insurance of autonomous robots in order to protect life, health, property and privacy.

### Section 2. Scope

(1) This Act applies to every robot placed on the market, put into service or operated within the territory.

(2) This Act does not apply to:

(a) robots used exclusively by the armed forces, which are governed by separate legislation;

(b) machines whose every movement is commanded directly by a human and in which no AI model generates actions.

### Section 3. Definitions

For the purposes of this Act:

(a) "robot" means a machine capable of movement or physical manipulation whose actions are wholly or partly determined by an AI model;

(b) "AI model" means a computational system whose behaviour derives from learned parameters and is not fully specified by its source code;

(c) "safety controller" means a hardware and software unit, physically separate from the AI model, that enforces the limits set out in Section 6;

(d) "safe state" means a condition in which the robot is stable and exerts no force capable of causing injury or damage;

(e) "operator" means the natural or legal person who controls the use of a robot and benefits from its operation; the owner is presumed to be the operator unless proven otherwise;

(f) "manufacturer" means the person who places a robot on the market under its own name or trademark;

(g) "model supplier" means the person who supplies an AI model for use in a robot;

(h) "circumvention" means any act that disables, bypasses or alters a safety measure required by this Act, including the installation of an unapproved AI model;

(i) "vulnerable person" means a minor or a person dependent on the care of others by reason of age, illness or disability;

(j) "Authority" means the Robotics Safety Authority established under Section 21.

### Section 4. Legal status of robots

(1) A robot is a thing. It has no legal personality and cannot hold rights, bear obligations or incur liability.

(2) Every robot of Class B or higher shall have an identifiable operator at all times.

## Part II: Classification

### Section 5. Classes of robots

(1) Robots are classified as follows:

| Class | Definition | Regime |
| --- | --- | --- |
| A | Robots that, by their mass and actuator force, cannot cause injury requiring medical treatment | Exempt from Parts III to VI |
| B | Robots capable of causing injury, operated in private premises | Parts III to V, and type approval under Section 22 |
| C | Robots capable of causing injury, operated in publicly accessible places | Parts III to VI in full |
| D | Robots exceeding the mass, force or speed thresholds set by the Authority, including vehicles and industrial machines | Parts III to VI in full, with operator licensing |
| E | Robots caring for vulnerable persons, or operating in critical infrastructure or in laboratories handling hazardous agents | Parts III to VI in full, and Part VII, Sections 27 to 29 |

(2) A robot that meets the definition of more than one class belongs to the highest of them.

(3) The Authority shall set by regulation the mass, force and speed thresholds separating the classes and shall review them at least every two years.

(4) Modification of a robot that moves it into a higher class requires new approval under Section 22.

## Part III: Technical Safety Requirements

### Section 6. Safety controller

(1) Every robot of Class B or higher shall be fitted with a safety controller running on hardware physically separate from the hardware that runs the AI model.

(2) The safety controller shall enforce limits on force, speed and permitted zones of operation, and shall bring the robot to a safe state when a limit is exceeded.

(3) The AI model shall have no means of writing to, reconfiguring or disabling the safety controller.

(4) The software of the safety controller shall be formally verified against its specification. The verification record forms part of the type approval file.

### Section 7. Physical stop

(1) Every robot of Class B or higher shall have a clearly marked physical stop control that brings the robot to a safe state.

(2) The physical stop shall act directly on the power supply to the actuators and shall not be capable of being disabled by software.

### Section 8. Software integrity

(1) A robot shall start only firmware and AI models that carry a valid cryptographic signature of the manufacturer.

(2) The Authority shall keep a public register of AI models approved for each class. A model not entered in the register shall not be installed in a robot of Class B or higher, except as provided in Section 31.

(3) The manufacturer shall provide security updates for the whole declared service life of the robot, which shall not be shorter than ten years.

### Section 9. Integrity of the body

(1) A robot shall hold a record of its approved tools and end effectors.

(2) Where a robot detects an unapproved tool, an object fixed to its body or a modification of its structure, it shall enter a restricted mode in which it performs no manipulation and moves only as needed to reach a safe state.

### Section 10. Event recorder

(1) Every robot of Class B or higher shall be fitted with a tamper-evident event recorder.

(2) The recorder shall store, for at least 30 days, the commands received, the version of the AI model, the interventions of the safety controller and the sensor data needed to reconstruct an incident.

(3) Access to the recorder is permitted only to the operator, to the Investigation Board under Section 25, and to other persons on the basis of a court order.

### Section 11. Identification

(1) Every robot of Class C or higher shall bear a visible registration mark and shall broadcast its registration identifier by radio while in operation.

(2) A robot shall disclose that it is a robot to any person who asks, and shall not present itself as a human.

### Section 12. Loss of connection, end of support and remote intervention

(1) Loss of network connection or of a remote service shall not cause a robot to leave a safe mode of operation.

(2) At the end of its service life a robot shall enter a restricted mode with reduced force and speed. It shall not be rendered inoperable.

(3) Remote intervention by the manufacturer or by a public authority is limited to bringing the robot to a safe state. Remote assumption of control over the movement of a robot is prohibited.

## Part IV: Liability

### Section 13. Liability of the operator

(1) The operator is liable for damage caused by the operation of a robot of Class B or higher, irrespective of fault.

(2) The injured person need prove only the damage and that it was caused by the robot.

(3) The operator is released from liability only to the extent that the damage was caused by the injured person's own intentional act.

### Section 14. Liability of the manufacturer

(1) The manufacturer is liable for damage caused by a defect of the robot, including a defect of its firmware, of its AI model or of any update.

(2) A robot is defective where it does not provide the safety that a person is entitled to expect, including where a known vulnerability was not remedied within the period set under Section 26.

(3) Where the event recorder data are missing, unreadable or withheld, the defect and the causal link are presumed, and the manufacturer bears the burden of proving otherwise.

(4) An operator or insurer who has compensated the injured person has a right of recourse against the manufacturer to the extent of the manufacturer's liability.

### Section 15. Liability of the model supplier

The model supplier is liable to the manufacturer for damage the manufacturer was obliged to compensate as a result of a defect of the AI model. This liability cannot be excluded or limited by contract.

### Section 16. Circumvention

(1) A person who carries out circumvention is liable in full for all damage subsequently caused by the robot, jointly and severally with the operator.

(2) The manufacturer is released from liability for damage caused by circumvention if it proves that the safety measures corresponded to the state of the art at the time the robot was placed on the market or last updated.

### Section 17. Interference by a third party

(1) Unlawful interference by a third party does not release the operator from liability towards the injured person.

(2) The operator and its insurer have a right of recourse against the third party, and against the manufacturer where the interference exploited a vulnerability covered by Section 14(2).

## Part V: Insurance

### Section 18. Compulsory liability insurance

(1) A robot of Class B or higher shall not be operated unless liability for damage caused by its operation is insured.

(2) The insurance contract is tied to the serial number of the robot and passes to a new operator on transfer.

(3) The injured person has a direct claim against the insurer.

(4) The Authority shall set by regulation the minimum insured amounts for each class.

(5) Insurers may set premiums according to the safety record of the robot type, of the AI model and of the manufacturer. The Authority shall give insurers access to anonymised incident data for that purpose.

### Section 19. Guarantee Fund

(1) A Guarantee Fund is established to compensate damage caused by a robot that is uninsured or whose operator cannot be identified.

(2) The Fund is financed by contributions of insurers providing insurance under Section 18.

(3) The Fund has a right of recourse against the operator and against any person liable under Part IV.

### Section 20. Systemic Risk Fund

(1) A Systemic Risk Fund is established to cover damage arising from a single defect or vulnerability that affects more than a number of robots set by the Authority.

(2) The Fund is financed by contributions of manufacturers in proportion to the number of their robots in operation, weighted by class.

(3) The State guarantees the obligations of the Fund above a ceiling set by statute.

(4) Insurers under Section 18 may limit their cover for events falling under subsection (1) to an amount set by the Authority. Damage above that amount is paid by the Fund.

## Part VI: Approval, Registration and Oversight

### Section 21. Robotics Safety Authority

(1) The Robotics Safety Authority is established as an independent administrative body.

(2) The Authority grants type approvals, keeps the registers under Sections 8 and 24, supervises compliance with this Act and issues the regulations this Act provides for.

### Section 22. Type approval

(1) A robot of Class B or higher shall not be placed on the market without type approval.

(2) The Authority grants type approval where the manufacturer demonstrates compliance with Part III. Approval covers a specific combination of hardware, firmware and AI model.

(3) A change of AI model, or a firmware change affecting the safety controller, requires an extension of the approval.

(4) The Authority shall suspend or withdraw approval where a robot type presents a serious risk that the manufacturer has not remedied.

### Section 23. Periodic inspection

(1) Robots of Class C or higher are subject to periodic technical inspection at intervals set by the Authority, not exceeding two years.

(2) The inspection verifies the function of the safety controller and of the physical stop, the integrity of the body and the validity of software signatures.

### Section 24. Register of robots and operators

(1) The Authority keeps a register of robots of Class C or higher and of their operators.

(2) The operator shall notify the Authority of any transfer, loss, theft or decommissioning of a registered robot within seven days.

(3) Data in the register are not public. They are disclosed to an injured person to the extent needed to bring a claim.

### Section 25. Incident Investigation Board

(1) An Incident Investigation Board is established, independent of the Authority.

(2) Operators and manufacturers shall report to the Board without delay any incident involving death, injury or serious damage, and any failure of a safety controller.

(3) The purpose of an investigation is to establish causes and prevent recurrence, not to apportion blame. Statements made to the Board shall not be used as evidence against the person who made them, except in cases of intentional harm.

(4) The Board publishes its findings and safety recommendations.

### Section 26. Vulnerabilities

(1) A manufacturer or model supplier that learns of a vulnerability affecting safety shall notify the Authority within 72 hours.

(2) The Authority sets a period for remedy according to the severity of the vulnerability. Until the remedy is deployed, the Authority may order affected robots to operate in restricted mode.

## Part VII: Special Protections and Prohibitions

### Section 27. Robots caring for vulnerable persons

(1) A robot caring for a vulnerable person shall not use techniques designed to create emotional dependence, and shall not promote goods, services or opinions to that person.

(2) The operator shall designate a natural person responsible for supervising the care. That person shall be notified of every intervention of the safety controller.

(3) A robot shall not restrict the movement of a vulnerable person except to avert an immediate danger to life or health.

### Section 28. Data from private dwellings

(1) Data captured by a robot inside a private dwelling shall be processed within the robot or on equipment under the control of the operator.

(2) Transfer of such data to the manufacturer or to any third party requires the specific, revocable consent of the operator and shall not be a condition for the functioning of the robot.

(3) Public authorities may obtain such data only on the basis of a court order.

### Section 29. Laboratories and critical infrastructure

(1) In a laboratory handling hazardous biological or chemical agents, a robot or an AI model shall not initiate any step of synthesis, modification or release of such agents without confirmation by two authorised natural persons acting independently.

(2) In critical infrastructure, no single AI model shall control more than the share of installations set by the Authority, so that a defect of one model cannot disable the whole system.

### Section 30. General prohibitions

It is prohibited to:

(a) fit a robot with a weapon or adapt it for use as a weapon;

(b) operate a robot that decides autonomously on the use of force against a person;

(c) operate a robot that presents itself as a human;

(d) operate a robot of Class C or higher without identification under Section 11;

(e) carry out circumvention on a robot operated in a publicly accessible place.

### Section 31. Private and experimental use

(1) Any person may install an AI model of their own choice in a robot of Class A.

(2) Any person may build, modify and operate a robot of Class B or D with an unapproved AI model on private premises that are closed to the public, provided that the physical stop under Section 7 is retained. Section 16(1) applies.

(3) Manufacturers shall not use technical measures to prevent the uses permitted by this Section, nor to prevent repair by the operator or by an independent repairer.

## Part VIII: Penalties and Final Provisions

### Section 32. Criminal offences

(1) A person who commits an act prohibited by Section 30(a), (b) or (e) commits a criminal offence punishable by imprisonment of up to five years.

(2) Where the act causes death or serious injury, the penalty is imprisonment of three to fifteen years.

(3) A person who uses a robot to commit a criminal offence is liable as if they had committed it in person.

### Section 33. Administrative penalties

(1) The Authority may impose on a manufacturer or model supplier a fine of up to 6 % of its worldwide annual turnover for breach of Part III, Section 22 or Section 26.

(2) The Authority may impose on an operator a fine for operating a robot without insurance, registration or valid inspection, and may order the robot to be taken out of operation.

(3) In setting a fine the Authority takes into account the gravity and duration of the breach and whether the person reported it voluntarily.

### Section 34. Transitional provisions

(1) Robots placed on the market before the entry into force of this Act may be operated for a period of three years, after which they shall comply with Sections 7, 11 and 18.

(2) Robots that cannot be brought into compliance with Section 6 shall after that period be operated only in the restricted mode under Section 12(2).

### Section 35. Review and entry into force

(1) The Government shall submit to Parliament, every three years, a report on the application of this Act, including an assessment of the use of the powers under Sections 10(3), 12(3) and 24 with regard to the protection of privacy.

(2) This Act enters into force on the first day of the twelfth month following its publication.
