<!--
author: {{AUTHOR_NAME}}
email: {{AUTHOR_EMAIL}}
version: {{VERSION_NUMBER}}
language: {{LANGUAGE_CODE}}
narrator: {{NARRATOR_VOICE}}
comment: {{COURSE_DESCRIPTION}}

link: https://raw.githubusercontent.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/refs/heads/main/ASSET_basic.css

@style
.welcome-container {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 3rem;
    margin: 2rem 0;
    border-radius: 20px;
    box-shadow: 0 12px 40px rgba(0,0,0,0.3);
}

.orientation-page {
    background: #f8f9fa;
    border: 3px solid #007bff;
    border-radius: 15px;
    padding: 2rem;
    margin: 2rem 0;
    text-align: center;
}

.nugget-header {
    background: linear-gradient(45deg, #ff6b6b, #ffa726);
    color: white;
    padding: 1.5rem;
    border-radius: 15px;
    margin: 1rem 0;
    text-align: center;
}

.funding-acknowledgment {
    background: #e3f2fd;
    border-left: 5px solid #2196f3;
    padding: 1rem;
    margin: 1rem 0;
}

.inclusivity-notice {
    background: #f1f8e9;
    border: 2px solid #8bc34a;
    border-radius: 10px;
    padding: 1rem;
    margin: 1rem 0;
}

.competency-framework {
    text-align: center;
    margin: 2rem 0;
    padding: 1rem;
    background: white;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}

.motivational-statement {
    font-size: 1.5rem;
    font-weight: bold;
    color: #2196f3;
    text-align: center;
    margin: 1.5rem 0;
    padding: 1rem;
    background: linear-gradient(45deg, #e3f2fd, #f3e5f5);
    border-radius: 10px;
}

.contact-info {
    background: #fff3e0;
    border: 1px solid #ff9800;
    padding: 1rem;
    border-radius: 8px;
    margin: 1rem 0;
}

.audio-control {
    background: #e8f5e8;
    padding: 0.5rem;
    border-radius: 5px;
    margin: 0.5rem 0;
}

.reflection-section {
    background: #fafafa;
    border-left: 4px solid #9c27b0;
    padding: 1.5rem;
    margin: 2rem 0;
}

{{ADDITIONAL_CUSTOM_CSS}}
@end

@customQuiz
[[...]]
<script>
"@0" == btoa( "@input".trim().toLowerCase() )
</script>
@end

@h5p: <div class="h5p-element"><iframe src="@0" width="100%" height="@1" frameborder="0"></iframe></div>

@aiDemo: <div class="ai-tool-demo">**AI Demo:** @0<br>**Tool:** @1<br>**Try it:** [Click here](@2)</div>

@competencyHighlight: <div class="competency-framework"><img src="@0" alt="AI Competency Framework" style="max-width: 100%; height: auto;"><br><p style="color: #2196f3; font-weight: bold;">@1</p></div>

@motivationalStatement: <div class="motivational-statement">@0 @1</div>

@resourceLink: <a href="@1" class="resource-link" target="_blank">@0</a>

@highlightCell: <span style="background-color: #e3f2fd; border: 2px solid #2196f3; padding: 0.5rem; border-radius: 5px; font-weight: bold;">@0</span>

@normalCell: <span style="padding: 0.5rem;">@0</span>

-->


# .

<svg xmlns='http://www.w3.org/2000/svg' width='1100' height='400' viewBox='0 0 800 450'>
  <!-- Background -->
  <rect width='800' height='450' fill='{{PRIMARY_COLOR}}' />
  
  <!-- White rounded rectangle container -->
  <rect x='50' y='50' width='700' height='350' rx='20' fill='white' />
  
  <!-- Title -->
  <text x='400' y='130' font-family='Segoe UI, Arial, sans-serif' font-size='50' font-weight='bold' text-anchor='middle' fill='{{PRIMARY_COLOR}}'>
    {{COURSE_TITLE}}
  </text>
  
  <!-- Subtitle -->
  <text x='400' y='180' font-family='Segoe UI, Arial, sans-serif' font-size='24' font-weight='bold' text-anchor='middle' fill='{{SECONDARY_COLOR}}'>
    Virtual Training Nugget {{NUGGET_NUMBER}}
  </text>

  <!-- Framework Reference -->
  <text x='400' y='210' font-family='Segoe UI, Arial, sans-serif' font-size='16' font-weight='bold' text-anchor='middle' fill='{{SECONDARY_COLOR}}'>
    Based on the UNESCO AI Competency Framework for Teachers
  </text>

  <!-- Collaboration info -->
  <text x='400' y='235' font-family='Segoe UI, Arial, sans-serif' font-size='16' font-weight='bold' text-anchor='middle' fill='{{SECONDARY_COLOR}}'>
    A collaboration of the UNEVOC Network - ASSET Project
  </text>

  <!-- Academic reference -->
  <text x='400' y='260' font-family='Segoe UI, Arial, sans-serif' font-size='14' font-weight='bold' text-anchor='middle' fill='{{SECONDARY_COLOR}}'>
    {{ACADEMIC_REFERENCE}}
  </text>
</svg>

<!-- License info -->
<div style="position: fixed; bottom: 10px; right: 10px; font-size: 12px; opacity: 0.7;">
  <img src="media/CC_BY-SA_icon.png" alt="CC BY-SA" style="height: 20px; vertical-align: middle;">
  <a href="https://creativecommons.org/licenses/by-sa/4.0/" style="margin-left: 5px; text-decoration: none;">CC BY-SA 4.0</a>
</div>


<!-- UNEVOC -->
<div style="position: fixed; bottom: 20px; left: 20px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UNESCO-UNEVOC_logo.png?raw=true" alt="UNEVOC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UNEVOC</div>
</div>

<!-- ASSET -->
<div style="position: fixed; bottom: 20px; left: 180px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/ASSET_icon.png?raw=true" alt="ASSET Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">ASSET</div>
</div>

<!-- HWK Blume -->
<div style="position: fixed; bottom: 20px; left: 340px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/HWK_Blume.png?raw=true" alt="HWK Blume Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 7px;">HWK Blume</div>
</div>

<!-- GIZ -->
<div style="position: fixed; bottom: 20px; left: 500px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/giz-logo.gif?raw=true" alt="GIZ Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">GIZ</div>
</div>

<!-- UoVT -->
<div style="position: fixed; bottom: 20px; left: 660px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UoVT_Logo.png?raw=true" alt="UoVT Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UoVT</div>
</div>

<!-- OVGU -->
<div style="position: fixed; bottom: 20px; left: 820px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/Masub27/Intro/blob/main/ovgu.png?raw=true" alt="OVGU Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">OVGU</div>
</div>

<!-- HRDC -->
<div style="position: fixed; bottom: 20px; left: 980px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/hrdc_logo.png?raw=true" alt="HRDC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">HRDC</div>
</div>

<!-- MITD -->
<div style="position: fixed; bottom: 20px; left: 1140px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/mitd_logo.png?raw=true" alt="MITD Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">MITD</div>
</div>

---



## Welcome Page

<div class="welcome-container">

**{{WELCOME_TITLE}}**

Dear Learner,

Welcome to our comprehensive course on {{MAIN_TOPIC}}! We are excited to guide you through this learning journey.

> **Course Intention**

{{COURSE_INTENTION_TEXT}}

> **Funding & Partnership Acknowledgment**

<div class="funding-acknowledgment">
This course is made possible through the generous support of:

• **{{MAIN_FUNDER}}** ({{MAIN_FUNDER_ACRONYM}})
• **UNESCO** - United Nations Educational, Scientific and Cultural Organization
• **{{ADDITIONAL_FUNDERS}}**

This project is part of the {{PROJECT_NAME}} initiative, fostering international collaboration in {{FIELD_OF_STUDY}}.
</div>



## Course Overview

@@@

Structure: Course - Module - Nugget
We talk about the Course 

Course:
Module: Hoorziontal (Aspects such as Human Mindset, Ethics etc.)
Nugget: Specific Learning objective (LO. #.#.#.)

{{COURSE}} = Whole course for this example which comprises the 5 Competencies and the Aimed for {{COMPETENCY_LEVELS}}

{{Course_Description}} The {{COURSE}} aims to tackle the first Learning Objective of the first {{COMPETENCY_LEVELS}} to teach teachers a basic introduction of AI Skills based on the UNESCO Framework

{{COURSE_DURATION}} = number of overall {{NUMBER_OF_NUGGETS}} based on {{Course_Description}}

@@@


> **📊 Course Structure:**

- **Duration:** {{COURSE_DURATION}}
- **Number of Nuggets:** {{NUMBER_OF_NUGGETS}}
- **Learning Levels:** {{COMPETENCY_LEVELS}}
- **Time Investment:** {{TIME_INVESTMENT}} per nugget

**🔄 Processing Modes:**
{{#PROCESSING_MODES}}
- **{{MODE_NAME}}:** {{MODE_DESCRIPTION}}
{{/PROCESSING_MODES}}




## Nugget {{NUGGET_NUMBER}} Orientation

> **Current Focus: {{COMPETENCY_LEVELS}}**

| Competency | Acquire | Deepen | Create |
|------------|---------|--------|--------|
| **Human-centred Mindset** | @highlightCell(Develop understanding of AI's impact on human learning and well-being) | @normalCell(Apply human-centered principles in AI tool selection) | @normalCell(Design AI-enhanced learning experiences prioritizing human agency) |
| **Ethics of AI** | @normalCell(Understand basic AI ethical principles) | @normalCell(Analyze ethical implications of AI in education) | @normalCell(Develop ethical guidelines for AI use in teaching) |
| **AI Foundations & Applications** | @normalCell(Learn basic AI concepts and educational tools) | @normalCell(Integrate AI tools into teaching practice) | @normalCell(Create innovative AI-enhanced learning solutions) |
| **AI Pedagogy** | @normalCell(Understand AI's role in pedagogy) | @normalCell(Adapt teaching methods with AI support) | @normalCell(Design AI-integrated pedagogical approaches) |
| **AI for Professional Learning** | @normalCell(Use AI for personal professional development) | @normalCell(Collaborate with AI for continuous learning) | @normalCell(Lead professional development in AI literacy) |

---

<div class="orientation-page">

@competencyHighlight({{COMPETENCY_FRAMEWORK_IMAGE_URL}}, You are here: {{CURRENT_LEARNING_AREA}})

@motivationalStatement({{MOTIVATIONAL_STATEMENT}}, {{MOTIVATIONAL_EMOJI}})

<div class="contact-info">
📧 **Need Help?** Contact us at: {{CONTACT_EMAIL}}
</div>

</div>

---


#### Why LiaScript?

We chose LiaScript as our platform because:
{{#LIASCRIPT_BENEFITS}}
• {{BENEFIT}}
{{/LIASCRIPT_BENEFITS}}

This enables us to provide you with an interactive, accessible, and engaging learning experience that works across all devices and platforms.

</div>


#### Commitment to Inclusivity

<div class="inclusivity-notice">
🌍 **Our Commitment:** This course is designed to be accessible and inclusive for all learners, regardless of background, location, or learning preferences. We provide multiple formats, language options, and accessibility features to ensure everyone can participate effectively.

{{SPECIFIC_INCLUSIVITY_MEASURES}}
</div>
@@ add picture (same)

![Inclusiveity Picture](https://github.com/OVGU-VET-TechEd/ASSET_AI_Learning_Nuggets/blob/main/media/Inclusion_picture.jpg)

# {{NUGGET_TITLE}}

<div class="nugget-header">
**Virtual Training Nugget {{NUGGET_NUMBER}}:** {{NUGGET_SUBTITLE}}
<br>
**Competency Level:** {{COMPETENCY_LEVEL}} | **Duration:** {{NUGGET_DURATION}}
</div>

<div class="audio-control">
🎵 **Audio Narration Available** - Click the speaker icon to listen to this content
</div>

## Learning Objectives

By the end of this nugget, you will be able to:

{{#LEARNING_OBJECTIVES}}
{{OBJECTIVE_NUMBER}}. **{{ACTION_VERB}}** {{LEARNING_OUTCOME}}
{{/LEARNING_OBJECTIVES}}

> **Module {{MODULE_NUMBER}}: {{MODULE_TITLE}}**

> **{{SECTION_TITLE}}**

> **{{KEY_CONCEPT}}** {{CONCEPT_DEFINITION}}

<div class="framework-card">
**Core Elements:**
</div>


{{#CORE_ELEMENTS}}
{{ELEMENT_NUMBER}}. **{{ELEMENT_TITLE}}** - {{ELEMENT_DESCRIPTION}}
{{/CORE_ELEMENTS}}


## Real-World Examples

**Scenario:** {{SCENARIO_DESCRIPTION}}

**{{CHARACTER_NAME}}**, a {{PROFESSION}} in {{CONTEXT}}, faces {{CHALLENGE_DESCRIPTION}}.

**Key Question:** {{SCENARIO_QUESTION}}



## Hands-On Activity

> **Activity {{ACTIVITY_NUMBER}}: {{ACTIVITY_TITLE}}**

**Instructions:** {{ACTIVITY_INSTRUCTIONS}}

> **Step {{STEP_NUMBER}}: {{STEP_TITLE}}**

{{STEP_INSTRUCTIONS}}

    [[___]]
    **{{INPUT_FIELD_LABEL}}:** {{INPUT_FIELD_HINT}}



## Interactive Quiz Section

> **Knowledge Check {{QUIZ_NUMBER}}: {{QUIZ_TOPIC}}**

{{QUIZ_INSTRUCTION}}

> **Question {{QUESTION_NUMBER}}: {{QUESTION_TOPIC}}**

{{QUESTION_TEXT}}

    [[ ]] {{OPTION_1}}
    [[ ]] {{OPTION_2}}
    [[ ]] {{OPTION_3}}
    [[ ]] {{OPTION_4}}
    [[?]] {{SELECTION_INSTRUCTION}}
    <script>
      let correct = [{{CORRECT_ANSWERS}}];
      let selected = @input;
      
      let isCorrect = correct.every(i => selected.includes(i)) && 
                     selected.every(i => correct.includes(i));
      
      if (isCorrect) {
        send.lia("✅ **Excellent!** {{CORRECT_FEEDBACK}}");
      } else {
        send.lia("❌ **Not quite right.** {{INCORRECT_FEEDBACK}}");
      }
    </script>

> **Single Choice Question {{QUESTION_NUMBER}}: {{QUESTION_TOPIC}}**

{{QUESTION_TEXT}}

    [( )] {{OPTION_1}}
    [(X)] {{OPTION_2}}
    [( )] {{OPTION_3}}
    [[?]] {{SELECTION_INSTRUCTION}}
    <script>
      if (@input === 2) {
        send.lia("✅ **Perfect!** {{CORRECT_FEEDBACK}}");
      } else {
        send.lia("❌ **Try again.** {{INCORRECT_FEEDBACK}}");
      }
    </script>

---


#### Evaluation Framework

> **Criterion {{CRITERION_NUMBER}}: {{CRITERION_NAME}}**

    [( )] {{CRITERION_OPTION_1}}
    [( )] {{CRITERION_OPTION_2}}
    [( )] {{CRITERION_OPTION_3}}
    [( )] {{CRITERION_OPTION_4}}
    [[?]] {{CRITERION_QUESTION}}

---



## Reflection Section

<div class="reflection-section">

> **🤔 Personal Reflection**

Take a moment to reflect on your learning:

    [[___]]
    **{{REFLECTION_PROMPT_1}}**

    [[___]]
    **{{REFLECTION_PROMPT_2}}**

    [[___]]
    **{{REFLECTION_PROMPT_3}}**

### 💡 Key Insights

What are your main takeaways from this nugget?

    [[___]]
    **{{INSIGHT_PROMPT}}**

</div>



## Further Reading & Resources

<div class="audio-control">
🎵 **Audio Summary Available** - Listen to key points from this section
</div>

> **Essential Resources**

{{#ESSENTIAL_RESOURCES}}
@resourceLink({{RESOURCE_TITLE}}, {{RESOURCE_URL}})
{{/ESSENTIAL_RESOURCES}}

> **Extended Learning**

{{#EXTENDED_RESOURCES}}
• [{{RESOURCE_TITLE}}]({{RESOURCE_URL}}) - {{RESOURCE_DESCRIPTION}}
{{/EXTENDED_RESOURCES}}

> **Tools for Practice**

{{#PRACTICE_TOOLS}}
@aiDemo({{TOOL_DESCRIPTION}}, {{TOOL_NAME}}, {{TOOL_URL}})
{{/PRACTICE_TOOLS}}




## Next Steps & Module Progression

### ✅ Completion Checklist

Before moving to the next nugget, ensure you have:

{{#COMPLETION_CRITERIA}}
- [ ] {{COMPLETION_ITEM}}
{{/COMPLETION_CRITERIA}}

### 🎯 Preparation for Next Nugget

**Coming Up:** {{NEXT_NUGGET_TITLE}}

**Preview:** {{NEXT_NUGGET_PREVIEW}}

**Recommended Preparation:**
{{#PREPARATION_ITEMS}}
• {{PREPARATION_ITEM}}
{{/PREPARATION_ITEMS}}

---

## Course Navigation

> **📚 All Course Nuggets**

{{#COURSE_NUGGETS}}
{{NUGGET_NUMBER}}. [{{NUGGET_TITLE}}]({{NUGGET_URL}}) - {{NUGGET_STATUS}}
{{/COURSE_NUGGETS}}

---

**🎉 Congratulations on completing Virtual Training Nugget {{NUGGET_NUMBER}}!**

<div class="contact-info">
**Support & Feedback:**
📧 Email: {{CONTACT_EMAIL}}
🌐 Course Portal: {{COURSE_PORTAL_URL}}
📋 Feedback Form: {{FEEDBACK_FORM_URL}}
</div>

> *{{CLOSING_INSPIRATION_MESSAGE}}*

