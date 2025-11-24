# Response to Reviewers - AK_statics

## Review of Statics_Lesson1.ipynb

### Reviewer Comment (Issue/Weakness): Minor typos
**Issue:** "Sutdents" → Students, "analyize" → analyze.

**Our Response:**
Thank you for this catch; we have updated the text.

---

### Reviewer Comment (Issue/Weakness): Video placeholder
**Issue:** The code block for IPython.display.HTML does not contain a working link (currently just `video_html = """ """`). Replace with actual embedded video or remove.

**Our Response:**
It worked when I had downloaded the notebook but not when it was just accessible on the web interface. Since I am not sure why and could not fix this, I have removed the video in favor of an image.

---

### Reviewer Comment (Issue/Weakness): Units
**Issue:** Constants use PSI and inches, while students should also be familiar with SI (MPa, meters). At least provide dual-unit examples.

**Our Response:**
After talking with our corresponding high school teacher, we decided that adding both units throughout might be a bit much for an introductory lesson. To still address this though, we added a separate cell that explains how a teacher can perform the unit conversions if they want to introduce that concept.

---

### Reviewer Comment (Issue/Weakness): Code readability
**Issue:** Some explanations are verbose. Students may benefit from concise comments plus a short "summary cell" that shows the complete workflow at once.

**Our Response:**
The comments were written in collaboration with the teacher who would be using the lesson. They are intended to provide comprehensive information, which teachers can then condense as needed. Therefore, we will retain the full comments but have also incorporated a summary cell, as suggested. We appreciate this valuable idea!

---

### Reviewer Comment (Issue/Weakness): Learning Objectives
**Issue:** Reframe as measurable outcomes (e.g., "Students will be able to calculate safe ice loads using Python functions").

**Our Response:**
I have revised the "Learning Objectives" to reflect more measurable outcomes. This includes adding a point about students' ability to calculate safe ice loads using Python code.

---

### Reviewer Comment (Issue/Weakness): Code clarity - compact version
**Issue:** Show a single-cell compact version after the step-by-step walkthrough, so students see the "full solution" cleanly.

**Our Response:**
Great idea! This is now included.

---

### Reviewer Comment (Issue/Weakness): Code clarity - f-strings
**Issue:** Use f-strings consistently for output (e.g., `print(f"Ice Thickness: {h} in, Safe Load: {safe_load} lbs")`).

**Our Response:**
Good catch! Done!

---

### Reviewer Comment (Issue/Weakness): Plot improvements
**Issue:** Add grid lines, units on axes, and compare safe vs. theoretical load.

**Our Response:**
I've updated the plot to include grid lines, units on the axes, and a comparison between the safe and theoretical load capacities.

---

### Reviewer Comment (Issue/Weakness): Assessment prompts
**Issue:** Add quick tasks at the end ("What happens if thickness = 8 inches?" or "Modify safety factor to 3, what changes?").

**Our Response:**
Great idea! Done!

---

### Reviewer Comment (Issue/Weakness): Context connection
**Issue:** After calculations, explicitly ask students to reflect: "How might climate change affect the assumptions in our model?"

**Our Response:**
That's a great way to connect the technical calculations back to the broader context of climate change! I added a reflection prompt after the coding and plotting sections to encourage students to think about how climate change might affect the assumptions made in our model. Thanks!

---

## Review of Statics_Lesson2 (1).ipynb

### Reviewer Comment (Issue/Weakness): Notation & Math Presentation
**Issue:** Symbols for forces are inconsistent: sometimes FN1/FN2, sometimes S1/S2. Stick to one.

**Our Response:**
Thank you for catching this inconsistency. We have standardized the notation throughout the notebook to use FN1/FN2 consistently for support forces, ensuring clarity and reducing student confusion.

---

### Reviewer Comment (Issue/Weakness): Stability check logic
**Issue:** The stability check `if FN1 < P_capacity:` only tests one support force, not the total. A case where each foot load < capacity but combined > capacity is not flagged. This should be clarified or modified.

**Our Response:**
Excellent point! We have revised the stability check to compare the total weight against the total capacity (both feet combined). The updated code now checks `if total_weight <= 2 * P_capacity:` and provides clearer feedback about whether the system is stable. We've also added a note explaining why we check the total load rather than individual support forces.

---

### Reviewer Comment (Issue/Weakness): Code comments
**Issue:** Redundant explanations in comments (how loops work) make code cells long; suggest a concise "annotated" version plus a clean minimal version for clarity.

**Our Response:**
We've restructured the code presentation to include both a detailed annotated version for learning and a clean, minimal version that students can reference as a complete solution. This allows teachers to choose the level of detail appropriate for their students while keeping the workflow clear.

---

### Reviewer Comment (Issue/Weakness): Output formatting
**Issue:** Use f-strings consistently for readable output instead of mixed formats.

**Our Response:**
All print statements have been updated to use f-strings consistently throughout the notebook for improved readability and modern Python best practices.

---

### Reviewer Comment (Pedagogical Issue): Simple example
**Issue:** Example is simple (equal load distribution). For more substantial conceptual value, show a non-symmetric case where forces differ.

**Our Response:**
We've added a second example demonstrating a non-symmetric case where a person is carrying a heavy backpack, shifting their center of mass and creating unequal force distribution between their feet. This helps students understand how asymmetric loading affects support forces and provides a more realistic application of the equilibrium concepts.

---

### Reviewer Comment (Pedagogical Issue): Concept check
**Issue:** The concept check section is good but could include a direct student coding task ("Modify the weights list to include 600 lb and discuss stability").

**Our Response:**
Great suggestion! We've added an interactive coding task where students modify the weight values and analyze the resulting stability. The task includes prompts for discussion about what happens when the total load exceeds capacity and how this relates to real-world safety considerations.

---

### Reviewer Comment (Pedagogical Issue): Text-heavy explanation
**Issue:** The note on solving for unknowns is text-heavy. Could be condensed with one symbolic worked example (system of equations with substitution).

**Our Response:**
We've condensed the explanation and added a clear worked example showing the system of equations with step-by-step substitution. This provides a concrete demonstration while reducing the amount of text students need to read through.

---

### Reviewer Comment (Suggestion): Standardize variable naming
**Issue:** Standardize variable naming (use FN1, FN2 throughout).

**Our Response:**
Completed as part of addressing the notation consistency issue above.

---

### Reviewer Comment (Suggestion): Revise stability check
**Issue:** Revise stability check: compare total weight vs. capacity, not only one support force.

**Our Response:**
Completed as part of addressing the stability check logic issue above.

---

### Reviewer Comment (Suggestion): Non-symmetric example
**Issue:** Add at least one non-symmetric example (person carrying a load more on one foot).

**Our Response:**
Completed as part of addressing the pedagogical issue about simple examples above.

---

### Reviewer Comment (Suggestion): Clean solution cell
**Issue:** Provide a clean solution cell at the end of each example to reinforce the workflow.

**Our Response:**
We've added clean solution cells at the end of each major example, presenting the complete workflow without extensive comments. This allows students to see the entire solution process in one place and serves as a reference for their own work.

---

## Review of Statics_Lesson3.ipynb

### Reviewer Comment (Area for Improvement): Clarity and Grammar
**Issue:** Multiple typos (e.g., calcualte, undersand, equilbrium, intereseted, direciton, raotate). These may distract students.

**Our Response:**
Thank you for the thorough proofreading. We have corrected all identified typos throughout the notebook to ensure a professional presentation that won't distract students from the learning content.

---

### Reviewer Comment (Area for Improvement): Mathematical Rigor
**Issue:** In Example 1, the explanation of why the torque is not zero could be more formal: explicitly show that the moment connection introduces an unknown reaction torque, leading to equilibrium equation.

**Our Response:**
We've enhanced the explanation to explicitly show how the moment connection at the support introduces an unknown reaction torque (M_reaction). The revised text now includes the complete equilibrium equation: ΣM = M_reaction + M_fish = 0, making it clear why we need to account for this reaction moment and how it maintains equilibrium.

---

### Reviewer Comment (Area for Improvement): Coding Pedagogy - linking code to theory
**Issue:** Current Python code is correct but lacks comments linking to equations. Students might struggle to connect code with theory.

**Our Response:**
We've added detailed comments throughout the code cells that explicitly reference the corresponding equations and theoretical concepts. For example, comments now indicate "# Calculate torque using τ = F × d (Equation 3.1)" to help students connect the code implementation directly to the mathematical theory.

---

### Reviewer Comment (Area for Improvement): Coding Pedagogy - intermediate outputs
**Issue:** Suggestion: add intermediate print statements (e.g., lever arm in ft, fish torque in lb·ft).

**Our Response:**
Excellent suggestion! We've added intermediate print statements that display calculated values at each step (lever arm, individual torques, etc.). This helps students verify their understanding at each stage and makes debugging easier if they modify the code.

---

### Reviewer Comment (Area for Improvement): Safety and Design Context
**Issue:** The note about the crane's actual load rating (220 lb vs 807 lb theoretical) is excellent, but it could be tied more explicitly to factor of safety concepts.

**Our Response:**
We've expanded this section to explicitly calculate and discuss the factor of safety (FoS = 807/220 ≈ 3.67). The revised text explains what this factor of safety means in practice and why manufacturers use such conservative ratings to account for dynamic loads, material variability, and long-term reliability.

---

### Reviewer Comment (Recommendation): Enhance Coding Cells - step-by-step outlines
**Issue:** Provide step-by-step code outlines more explicitly tied to equations.

**Our Response:**
We've restructured the coding cells to include explicit step-by-step outlines before the code. Each step is numbered and references the corresponding equation or concept, creating a clear bridge between theory and implementation.

---

### Reviewer Comment (Recommendation): Enhance Coding Cells - example format
**Issue:** Example: `#Step 1: Define known quantities...`

**Our Response:**
Implemented as part of the step-by-step outline enhancement above. All code cells now follow this clear format with numbered steps.

---

### Reviewer Comment (Recommendation): Link Back to Engineering Practice
**Issue:** When introducing manufacturer limits, explicitly define factor of safety (FoS) and ask students to compute it.

**Our Response:**
We've added a dedicated section that defines factor of safety, provides the formula (FoS = Ultimate Load / Working Load), and includes a coding task where students calculate the FoS for the crane example. This reinforces the connection between theoretical calculations and real-world engineering practice.

---

## Review of Statics_Lesson4.ipynb

### Reviewer Comment (Issue/Weakness): Vocabulary section
**Issue:** The vocabulary section says "no new vocabulary" but the lesson still has terms like pivot point and support force that could use a short definition.

**Our Response:**
You're absolutely right. We've updated the vocabulary section to include concise definitions of key terms used in this lesson (pivot point, support force, torque) even though they were introduced in earlier lessons. This reinforces important concepts and helps students who may need a refresher.

---

### Reviewer Comment (Issue/Weakness): Pivot point explanation
**Issue:** The pivot point explanation is correct but too abstract; many students may not see why A is chosen beyond "to simplify."

**Our Response:**
We've enhanced the explanation to show the concrete benefit of choosing point A as the pivot: it eliminates the unknown force at A from the torque equation because its lever arm is zero. We now include a comparison showing what the equation would look like with a different pivot point to demonstrate why choosing A makes the problem significantly easier to solve.

---

### Reviewer Comment (Issue/Weakness): Code completion level
**Issue:** Code is too complete. Students mostly just "run" instead of reasoning. Little space for discovery.

**Our Response:**
We've restructured the notebook to provide three levels of coding tasks: (1) a fully worked example with complete code and explanations, (2) partially completed code with strategic gaps for students to fill in (marked with `# YOUR CODE HERE`), and (3) blank scaffolds with only comments outlining the required steps. This allows teachers to choose the appropriate level of challenge for their students.

---

### Reviewer Comment (Issue/Weakness): Hard-coded values
**Issue:** Heavy reliance on hard-coded numbers (1500, 2, 5, etc.), no user input or variability.

**Our Response:**
We've converted the main calculations into functions that accept parameters (e.g., `def calculate_support_forces(weight, distance_to_load, total_length):`). This allows students to easily explore different scenarios by changing input values. We've also added prompts encouraging students to experiment with different values and observe how the results change.

---

### Reviewer Comment (Issue/Weakness): Error checking
**Issue:** No error checks (e.g., negative weights, unrealistic values).

**Our Response:**
We've added input validation to the functions, including checks for negative weights, distances outside the beam length, and other unrealistic values. When invalid inputs are detected, the code provides helpful error messages explaining what went wrong. This teaches students about defensive programming while preventing confusing results.

---

### Reviewer Comment (Issue/Weakness): Plot quality
**Issue:** Plotting is done but lacks labels, gridlines, or legend clarity for real interpretability.

**Our Response:**
All plots have been updated to include clear axis labels with units, gridlines for easier reading of values, descriptive legends, and titles that explain what the plot shows. We've also added annotations to highlight key points (e.g., the location of the load, support forces).

---

### Reviewer Comment (Issue/Weakness): Incremental coding tasks
**Issue:** Incremental coding tasks ("delete or keep") are confusing; students may not know which version to use.

**Our Response:**
We've removed the confusing "delete or keep" instructions and instead provide clear, separate sections for each approach: one complete reference solution and separate scaffolded exercises with clear instructions about what students should do. This eliminates ambiguity about which code to use.

---

### Reviewer Comment (Suggestion): Term definitions
**Issue:** Add short definitions for recurring terms (pivot, support force, torque) even if they were introduced earlier.

**Our Response:**
Completed as part of addressing the vocabulary section issue above.

---

### Reviewer Comment (Suggestion): Coding scaffolds
**Issue:** Provide optional coding scaffolds: one full example, one partial outline, and one blank cell for different skill levels.

**Our Response:**
Completed as part of addressing the code completion level issue above.

---

### Reviewer Comment (Suggestion): Emphasize reasoning
**Issue:** Emphasize why each step matters (choosing the pivot point simplifies solving, not just "because it's natural").

**Our Response:**
Completed as part of addressing the pivot point explanation issue above.

---

### Reviewer Comment (Suggestion): Real-world connection
**Issue:** In the results section, tie the numbers back to real-world meaning (what failure would look like on the ice).

**Our Response:**
We've added a discussion section after the calculations that explains what the calculated forces mean in physical terms. For example, we discuss what would happen if the ice couldn't support the calculated force at point B (cracking, vehicle sinking) and how this relates to the safety considerations discussed in earlier lessons.

---

### Reviewer Comment (Suggestion): Encourage experimentation
**Issue:** Encourage experimentation: e.g., "Change trailer weight or ice thickness and see what happens."

**Our Response:**
We've added an "Exploration Tasks" section at the end with specific prompts for experimentation, such as: "What happens to the support forces if you double the trailer weight?" and "How does moving the trailer closer to point A affect the force at point B?" These tasks encourage students to develop intuition by exploring different scenarios.

---

## Review of Statics_Lesson5.ipynb

### Reviewer Comment (Issue/Weakness - Pedagogical): Abstract jump
**Issue:** The concept of "infinitely close cut" for internal forces is introduced abruptly with little intuitive explanation. Students may struggle to understand why we "cut" the structure and what that reveals.

**Our Response:**
We've added an intuitive introduction using a physical analogy: imagine sawing through a wooden plank and examining what forces you'd need to apply to keep each piece in place. This helps students visualize why the "cut section" method works and what it reveals about internal forces. We've also included a simple diagram showing the cut and the exposed internal forces.

---

### Reviewer Comment (Issue/Weakness - Pedagogical): Heavy reliance on equations
**Issue:** Long symbolic sections dominate before intuition is reinforced. Visuals help, but students may still lose track.

**Our Response:**
We've reorganized the content to lead with conceptual understanding and visual explanations before introducing equations. Each major equation is now preceded by a qualitative explanation of what it represents and why we need it. We've also broken long derivations into smaller, digestible steps with intermediate explanations.

---

### Reviewer Comment (Issue/Weakness - Pedagogical): Uneven treatment of vocabulary
**Issue:** Terms like shear, moment, and cut section are assumed to be known rather than reinforced with simple analogies.

**Our Response:**
We've added a comprehensive vocabulary section with clear definitions and physical analogies for each term. For example, shear is explained as "forces trying to slide one part of the structure past another, like scissors cutting paper," and moment is described as "the tendency of a force to cause rotation, like pushing on a door handle to open it."

---

### Reviewer Comment (Issue/Weakness - Pedagogical): Overloaded lesson
**Issue:** Covers abutments, piers, shear, moment, cuts, and environmental tradeoffs in a single notebook. Risk of cognitive overload.

**Our Response:**
We've split this content into two separate notebooks: Lesson 5A focuses on external equilibrium (reactions at abutments and piers, load distribution), while Lesson 5B addresses internal forces (shear and moment using the cut section method). Each notebook is now more focused and manageable, reducing cognitive load while maintaining the logical flow of concepts.

---

### Reviewer Comment (Issue/Weakness - Code): Too complete
**Issue:** Most code cells already provide full solutions, leaving little room for students to practice problem-solving.

**Our Response:**
Following the approach used in Lesson 4, we've restructured the code to provide scaffolded learning opportunities: complete worked examples for new concepts, partially completed code with strategic gaps for practice, and blank scaffolds for more advanced exercises. This gives students appropriate challenges while ensuring they have reference solutions available.

---

### Reviewer Comment (Issue/Weakness - Code): Hard-coded values
**Issue:** Constants like 600,000 lb and 300 ft are fixed; this discourages exploration of alternative scenarios.

**Our Response:**
We've converted the main calculations into parameterized functions (e.g., `def calculate_bridge_reactions(total_load, bridge_length, load_position):`). This allows students to easily explore different bridge configurations, load magnitudes, and load positions. We've also added exploration prompts encouraging students to investigate how changing these parameters affects the results.

---

### Reviewer Comment (Suggestion - Pedagogy): Physical analogy for cuts
**Issue:** Introduce "cut sections" with a physical analogy (like sawing a plank and holding one piece) to make the rationale intuitive.

**Our Response:**
Completed as part of addressing the "abstract jump" issue above.

---

### Reviewer Comment (Suggestion - Pedagogy): Split lesson
**Issue:** Split lesson into two notebooks: one on external equilibrium (abutments, piers) and one on internal forces (shear and moment).

**Our Response:**
Completed as part of addressing the "overloaded lesson" issue above. The content is now divided into Lesson 5A (external equilibrium) and Lesson 5B (internal forces).

---

### Reviewer Comment (Suggestion - Pedagogy): Recap glossary
**Issue:** Add a brief recap glossary for shear, moment, cut section, and equilibrium to avoid assumed knowledge.

**Our Response:**
Completed as part of addressing the "uneven treatment of vocabulary" issue above.

---

### Reviewer Comment (Suggestion - Pedagogy): Conceptual questions
**Issue:** Use more conceptual questions before equations: for instance: "If a truck parks closer to one abutment, which support feels more load?"

**Our Response:**
We've added conceptual questions throughout the notebook before introducing mathematical formulations. These questions help students develop intuition and make predictions before seeing the calculations. For example, we now ask students to predict which support will carry more load before calculating the actual distribution.

---

### Reviewer Comment (Suggestion - Code): Scaffolded tasks
**Issue:** Provide scaffolded coding tasks: start with outlines, then let students complete missing steps instead of giving full solutions.

**Our Response:**
Completed as part of addressing the "too complete" code issue above.

---

### Reviewer Comment (Suggestion - Code): Use functions
**Issue:** Replace repeated hard-coded problems with functions (e.g., `def support_forces(length, load, position): ...`).

**Our Response:**
Completed as part of addressing the "hard-coded values" issue above.

---

### Reviewer Comment (Suggestion - Code): Interactive sliders
**Issue:** Add interactive sliders (via ipywidgets) for bridge length, weight, and load position to make the exploration more engaging and fun.

**Our Response:**
Excellent idea! We've added interactive widgets using ipywidgets that allow students to adjust bridge length, load magnitude, and load position with sliders. The results (support forces, shear, and moment) update in real-time, making it easy and engaging for students to explore how different parameters affect the structural behavior. This also makes the notebook more interactive and fun while reinforcing the underlying concepts.

---

### Reviewer Comment (Suggestion - Code): Clear expectations
**Issue:** Make expectations clear: consistently present each coding task as (a) full worked example, (b) partial outline, or (c) blank scaffold.

**Our Response:**
We've standardized the presentation of all coding tasks with clear headers indicating the type: "📘 Worked Example (Complete Code)", "✏️ Practice Task (Fill in the Blanks)", or "🎯 Challenge (Build from Scratch)". This makes it immediately clear what level of completion students should expect and what they need to do.

---

## Summary of Changes

### Statics_Lesson1.ipynb
- ✅ Fixed typos
- ✅ Replaced video with image
- ✅ Added unit conversion cell
- ✅ Added summary cell
- ✅ Revised learning objectives to be measurable
- ✅ Added compact solution version
- ✅ Standardized f-strings
- ✅ Enhanced plots with gridlines, units, and safe vs. theoretical comparison
- ✅ Added assessment prompts
- ✅ Added climate change reflection prompt

### Statics_Lesson2 (1).ipynb
- ✅ Standardized notation (FN1/FN2 throughout)
- ✅ Fixed stability check to compare total load vs. total capacity
- ✅ Restructured code with annotated and clean versions
- ✅ Standardized f-strings throughout
- ✅ Added non-symmetric example (person with backpack)
- ✅ Added interactive coding task in concept check
- ✅ Condensed text with worked example for system of equations
- ✅ Added clean solution cells for each example

### Statics_Lesson3.ipynb
- ✅ Corrected all typos
- ✅ Enhanced mathematical rigor in Example 1 (explicit reaction torque)
- ✅ Added comments linking code to equations
- ✅ Added intermediate print statements
- ✅ Expanded safety discussion with explicit FoS calculation
- ✅ Added step-by-step code outlines
- ✅ Added FoS definition and student calculation task

### Statics_Lesson4.ipynb
- ✅ Updated vocabulary section with key definitions
- ✅ Enhanced pivot point explanation with comparison
- ✅ Restructured with three levels of coding tasks
- ✅ Converted to parameterized functions
- ✅ Added input validation and error checking
- ✅ Improved plots with labels, gridlines, legends, and annotations
- ✅ Clarified coding task structure
- ✅ Added real-world failure discussion
- ✅ Added exploration tasks section

### Statics_Lesson5.ipynb
- ✅ Added physical analogy for cut sections
- ✅ Split into Lesson 5A (external equilibrium) and 5B (internal forces)
- ✅ Added comprehensive vocabulary section with analogies
- ✅ Reorganized to lead with concepts before equations
- ✅ Provided scaffolded coding tasks (worked/partial/blank)
- ✅ Converted to parameterized functions
- ✅ Added interactive widgets (ipywidgets) for exploration
- ✅ Added conceptual prediction questions
- ✅ Standardized coding task presentation with clear headers

---

*Document prepared: November 24, 2025*
