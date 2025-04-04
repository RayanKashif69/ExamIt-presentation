---
layout: default
title: Development Experience
---

<section class="info-card focus-card">
  <h2>Development Process & Reflections</h2>
  <p>Here is a summary of our retrospectives and lessons learned during the development of ExamIt, including what went well, what challenges we faced, and what we would improve if starting again.</p>
</section>

<section class="reflection-cards">

  <div class="reflection-card">
    <h3> What Went Right</h3>
    <p>Splitting the project into separate source files and developing independently worked out great. Each person could work on different files, which prevented conflicts and made branch merging much easier.</p>
  </div>

  <div class="reflection-card">
    <h3> What Went Wrong</h3>
    <p>This strategy also had a downside — coordination between branches became very difficult. Since members didn’t interact with each other's branches until merging, it was hard to know what others were working on or what would be required. This issue became more noticeable in Iteration 3 when distant branches had to be merged into <code>develop</code>.</p>
  </div>

  <div class="reflection-card">
    <h3> What Could've Solved It</h3>
    <p>Before diving into branching, we should’ve designed the structure together and agreed on interfaces for key classes. This way, everyone could expect consistent behavior without needing to see the implementation. We began trying this approach during the last week — and it worked well for aligning expectations.</p>
  </div>

  <div class="reflection-card">
    <h3> Change of Vision</h3>
    <p>Over time, some planned features were removed from the scope, such as the teacher role, achievement system, timers for mock tests, notes, and content sharing.</p>
  </div>

  <div class="reflection-card">
    <h3> What Took the Most Time?</h3>
    <p>The FlashCard feature took the most time. Our team decided to refactor after it was implemented and simultaneously tidy up parts of the logic layer — this resulted in it taking more time than expected.</p>
  </div>

  <div class="reflection-card">
    <h3> What We’d Do Differently</h3>
    <p>If we had the chance to start over, we would create a mermaid diagram for each iteration. This would help teammates understand the flow and reduce repetition. We’d also divide team responsibilities into layers — 1 person on the display layer, 2 on the business layer, and 2 on the data layer — allowing focused, parallel development and fewer merge issues.</p>
  </div>

</section>

<section class="info-card wide-reflection-card">
  <h2>Reflection on Vision, Challenges, and Lessons Learned</h2>
  <p>
    Since iteration 0, the scale of the project changed significantly as we discovered development constraints. While we implemented the core structure of the app, many initially planned features were removed due to complexity or time constraints — including user interaction and teacher accounts.
  </p>

  <p>
    Our strategy to divide the system into independent files worked well and minimized conflicts during merging. It allowed each team member to focus on their part of the project with minimal interruption or overlap.
  </p>

  <p>
    However, this separation also introduced challenges. Members often implemented similar logic independently in their own branches, leading to duplicated code in the final `develop` branch. This happened because we lacked a shared interface or upfront agreement on how components should interact.
  </p>

  <p>
    Moving forward, we learned that defining common interfaces early in development is essential. It helps ensure consistency across different parts of the system and reduces redundant work. In our final iteration, we successfully tried this by specifying expected interfaces in advance, which allowed teammates to implement their components independently — while still staying aligned.
  </p>
</section>
