# Digital Vote Register – Digital System Design (Logisim Evolution)
 
A complete digital counting system designed using combinational and sequential logic in **Logisim Evolution**.  
The project implements voter eligibility verification, ambiguity-free candidate selection, and secure vote counting with multi-digit display.
---
## Overview
This Digital Vote Register was developed as part of Digital System Design practice.  
It simulates a real-world voting process using fundamental logic blocks such as flip-flops, decoders, encoders, and counters.
The system ensures:
- Only eligible voters can vote  
- Only one candidate can be selected  
- Votes are counted securely  
- Results remain hidden until explicitly requested  
---
##Features

### Voter Eligibility Verification
Three criteria must be satisfied.
- Green LED → Eligible  
- Red LED → Not Eligible  
- Invalid voters cannot submit votes.
---

### Ambiguity-Free Candidate Selection
- Four candidates supported.
- Multiple selections are detected and rejected.
---

### Confirm-Based Voting
Votes are registered only after pressing **Confirm VOTE**.
---

### 8-Bit Asynchronous Counters
Each candidate uses an 8-bit D Flip-Flop based asynchronous counter.
Maximum count per candidate: **4096**
Global reset provided.
---

### Binary to BCD to 7-Segment Display
Binary counter outputs are converted to BCD and decoded to drive:
- Units  
- Tens  
- Hundreds  
---

### Vote Privacy Mode
All displays remain zero during voting.
Actual counts appear only after pressing **View All Candidate Votes**.
---

## Concepts Implemented
- D Flip-Flops  
- Asynchronous Counters  
- Encoders / Decoders  
- Clock Gating  
- Ambiguity Detection  
- BCD Conversion  
- 7-Segment Interfacing  
- Sequential + Combinational Integration  
---

## Tools Used

-Logisim Evolution 
---

## How to Run
1. Install Logisim Evolution.
2. Clone repository:
```bash
git clone <your-repo-url>
3. Open Digital_Vote_Regiser.circ
4. Set eligibility criteria.
5. Select a candidate.
6. Press Confirm Vote.
7. Use View Results to display counts.
8. Reset All Votes if required.

## Future Improvements
-Replace asynchronous counters with synchronous counters
-Add voter lock after successful vote
-Include EEPROM-style memory
-Implement password or ID verification
-Extend to N candidates

## Learning Outcome
-Practical counter design
-Clock control
-Digital system integration
-Display interfacing
-Logic-level security mechanisms

👤 Author:
Dishan Panchigar
Electronics & Digital Systems Enthusiast

## License
This project is licensed under the MIT License.