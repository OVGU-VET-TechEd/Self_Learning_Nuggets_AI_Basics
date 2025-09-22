<!--
author: UNESCO ASSET Team
email: hannes.tegelbeckers@ovgu.de
version: 1.0.0
language: en
narrator: UK English Female
comment: Self-Learning Nugget - Human-centered mindset: Human agency in AI for TVET education

link: https://raw.githubusercontent.com/OVGU-VET-TechEd/Integrating_AI_in_TVET_UNESCO/refs/heads/main/VorlageUN.css

@style
.unesco-header {
    background: linear-gradient(135deg, #0072CE 0%, #00A1DE 100%);
    color: white;
    padding: 2rem;
    margin: 1rem 0;
    border-radius: 15px;
    text-align: center;
    box-shadow: 0 8px 32px rgba(0,114,206,0.3);
}

.framework-card {
    background: #f8f9fa;
    border-left: 5px solid #0072CE;
    padding: 1.5rem;
    margin: 1rem 0;
    border-radius: 0 10px 10px 0;
}

.challenge-box {
    background: linear-gradient(45deg, #ff6b6b, #ffa726);
    color: white;
    padding: 1rem;
    border-radius: 10px;
    margin: 1rem 0;
    text-align: center;
}

.opportunity-box {
    background: linear-gradient(45deg, #4CAF50, #8BC34A);
    color: white;
    padding: 1rem;
    border-radius: 10px;
    margin: 1rem 0;
    text-align: center;
}

.case-study {
    background: #e3f2fd;
    border: 2px solid #0072CE;
    border-radius: 15px;
    padding: 1.5rem;
    margin: 1rem 0;
}

.policy-highlight {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 1rem;
    border-radius: 10px;
    margin: 0.5rem 0;
}

.interactive-element {
    background: #fff3e0;
    border: 2px dashed #ff9800;
    border-radius: 10px;
    padding: 1rem;
    margin: 1rem 0;
}

@end

@SpeechRecognition.support
<script modify="false" run-once>
// Vendor prefix
const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
if (!SpeechRecognition) {
  "LIASCRIPT: > 'Speech Recognition' not supported in this browser. Try Chrome, Opera, or Edge.";
} else {
  "LIASCRIPT: > Your browser does support 'Speech Recognition' ..."
}
</script>
@end

@SpeechRecognition
<script>
// Vendor prefix
const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
if (!SpeechRecognition) {
  alert('SpeechRecognition not supported. Try Chrome, Opera, or Edge.');
} else {
  const recognition = new SpeechRecognition();
  recognition.lang = '@0';
  recognition.interimResults = false;
  recognition.continuous = false;

  const solution = "@1".toLowerCase()
    .replace(/(\.|\?|\!|\,|\-|\;)/g," ")
    .replace(/[ ]+/g," ")
    .trim();

  recognition.onresult = ev => {
    let t = ev.results[0][0].transcript?.toLowerCase().trim() || '';
    if (t === solution) {
      send.lia("true");
    } else {
      send.lia("Please try again â€¦",[],false);
    }
  };
  recognition.onerror = ev => send.lia("Error: "+ev.error,[],false);
  recognition.onend   = () => console.log('Speech recognition ended.');
  recognition.start();
}
"LIA: wait"
</script>
@end

@SpeechRecognition.withFeedback
<script>
// Vendor prefix
const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
if (!SpeechRecognition) {
  alert('SpeechRecognition not supported. Try Chrome, Opera, or Edge.');
} else {
  const recognition = new SpeechRecognition();
  recognition.lang = '@0';
  recognition.interimResults = false;
  recognition.continuous = false;

  const solution = "@1".toLowerCase()
    .replace(/(\.|\?|\!|\,|\-|\;)/g," ")
    .replace(/[ ]+/g," ")
    .trim();

  recognition.onresult = ev => {
    let t = ev.results[0][0].transcript?.toLowerCase().trim() || '';
    if (t === solution) {
      send.lia("true");
    } else {
      send.lia(t,[],false);
    }
  };
  recognition.onerror = ev => send.lia("Error: "+ev.error,[],false);
  recognition.onend   = () => console.log('Speech recognition ended.');
  recognition.start();
}
"LIA: wait"
</script>
@end
-->

# 🚀 Mastering AI for TVET Education

--{{0}}--
Welcome to this comprehensive learning experience on AI prompting techniques specifically designed for Technical and Vocational Education and Training educators. This interactive module will transform your understanding of how to effectively communicate with AI systems to enhance your teaching, learning, and assessment practices.

<svg xmlns="http://www.w3.org/2000/svg" width="960" height="540" viewBox="0 0 960 540">
  <!-- Background gradient -->
  <defs>
    <linearGradient id="grad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#667eea"/>
      <stop offset="100%" stop-color="#764ba2"/>
    </linearGradient>
  </defs>
  <rect width="960" height="540" fill="url(#grad)" rx="15" ry="15"/>

  <!-- Title -->
  <text x="480" y="80" text-anchor="middle" font-family="Arial, Helvetica, sans-serif" font-size="32" font-weight="bold" fill="#ffffff">
    🌟 Welcome to Your AI Learning Journey
  </text>

  <!-- Greeting -->
  <text x="480" y="130" text-anchor="middle" font-family="Arial, Helvetica, sans-serif" font-size="20" font-weight="600" fill="#ffffff">
    Dear TVET Educator,
  </text>

  <!-- Intro paragraph -->
  <text x="480" y="170" text-anchor="middle" font-family="Arial, Helvetica, sans-serif" font-size="16" fill="#e0e0ff">
    <tspan x="480" dy="0">Transform your teaching with cutting-edge AI prompting techniques!</tspan>
    <tspan x="480" dy="22">This immersive 15-minute experience will revolutionize how</tspan>
    <tspan x="480" dy="22">you leverage AI systems in your educational practice.</tspan>
  </text>

  <!-- Learning intention -->
  <text x="480" y="250" text-anchor="middle" font-family="Arial, Helvetica, sans-serif" font-size="18" font-weight="700" fill="#ffffff">
    🎯 Learning Intention
  </text>
  <text x="480" y="280" text-anchor="middle" font-family="Arial, Helvetica, sans-serif" font-size="16" fill="#e0e0ff">
    <tspan x="480" dy="0">Master practical AI prompting strategies that enhance your TVET teaching effectiveness.</tspan>
    <tspan x="480" dy="20">Discover how to identify AI potential, understand limitations,</tspan>
    <tspan x="480" dy="20">and craft powerful prompts for your specific educational context.</tspan>
  </text>
</svg>

<!-- UNEVOC -->
<div style="position: fixed; bottom: 1px; left: 20px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UNESCO-UNEVOC_logo.png?raw=true" alt="UNEVOC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UNEVOC</div>
</div>

<!-- ASSET -->
<div style="position: fixed; bottom: 1px; left: 180px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/ASSET_icon.png?raw=true" alt="ASSET Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">ASSET</div>
</div>

<!-- HWK Blume -->
<div style="position: fixed; bottom: 1px; left: 340px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/HWK_Blume.png?raw=true" alt="HWK Blume Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 7px;">HWK Blume</div>
</div>

<!-- GIZ -->
<div style="position: fixed; bottom: 1px; left: 500px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/giz-logo.gif?raw=true" alt="GIZ Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">GIZ</div>
</div>

<!-- UoVT -->
<div style="position: fixed; bottom: 1px; left: 660px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UoVT_Logo.png?raw=true" alt="UoVT Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UoVT</div>
</div>

<!-- OVGU -->
<div style="position: fixed; bottom: 1px; left: 820px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/Masub27/Intro/blob/main/ovgu.png?raw=true" alt="OVGU Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">OVGU</div>
</div>

<!-- HRDC -->
<div style="position: fixed; bottom: 1px; left: 980px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/hrdc_logo.png?raw=true" alt="HRDC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">HRDC</div>
</div>

<!-- MITD -->
<div style="position: fixed; bottom: 1px; left: 1140px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/mitd_logo.png?raw=true" alt="MITD Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">MITD</div>
</div>

# 📚 Critical Reflection on AI Benefits, Limitations and Risks in TVET Education

--{{0}}--
This learning experience is carefully structured to maximize your understanding and practical application of AI prompting techniques. You'll progress through interactive scenarios, hands-on activities, and real-world applications specific to TVET education.**Course Intention**. This nugget aims to develop your ability to critically evaluate AI tools for your specific TVET subject area, understand their pedagogical limitations, and make informed decisions about their appropriate use while maintaining human agency in education. 

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; margin: 30px 0;">

<div style="background: linear-gradient(45deg, #ff6b6b, #ffa500); color: white; padding: 25px; border-radius: 20px; box-shadow: 0 8px 25px rgba(0,0,0,0.1);">

### ⏱️ **Duration & Structure**
- **Time Investment:** 15 minutes
- **Learning Objective:** Using AI while maintaining human agency  
- **Format:** Interactive self-learning
- **Mode:** Self-paced with guided checkpoints

</div>

<div style="background: linear-gradient(45deg, #4ecdc4, #44a08d); color: white; padding: 25px; border-radius: 20px; box-shadow: 0 8px 25px rgba(0,0,0,0.1);">

### 🎯 **Why This Format?**
- **🔄 Immediate Application** - Practice as you learn
- **🗃️ Real-World Scenarios** - Actual TVET contexts
- **✅ Self-Assessment** - Check understanding instantly
- **🛠️ Practical Focus** - Skills for immediate use

</div>

</div>

## 🎯 Learning Objectives

<div style="background: linear-gradient(135deg, #e3f2fd, #bbdefb); padding: 30px; border-radius: 20px; margin: 30px 0; border-left: 8px solid #2196f3;">

### 🏆 **By the end of this nugget, you will master:**

<div style="display: grid; grid-template-columns: 1fr; gap: 15px; margin: 20px 0;">

<div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-left: 5px solid #ff6b6b;">
<strong>1. 🔍 IDENTIFY</strong> opportunities and risks of using AI tools for your subject area and teaching context
</div>

<div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-left: 5px solid #ffa500;">
<strong>2. 💡 Reflect</strong> regularly on technical and pedagogical limitations of AI tools regarding your learning group
</div>

<div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-left: 5px solid #4ecdc4;">
<strong>3. 🛠️ Explain</strong> the educational added value of AI tools for your specific educational context
</div>

<div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-left: 5px solid #9b59b6;">
<strong>4. ⚖️ Make informed decisions</strong> about when AI tool use is appropriate in teaching â€" and when it is not
</div>

<div style="background: white; padding: 20px; border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-left: 5px solid #2ecc71;">
<strong>5. ✅ Consider</strong> ethical and data protection aspects when using AI tools with your learning group
</div>

</div>

</div>

## 🎥 Module 1: Introduction Video & Context Setting

--{{0}}--
This introductory video explores the fundamental principle of maintaining human agency when integrating AI tools in technical and vocational education. It emphasizes the educator's central role in guiding, evaluating, and contextualizing AI-generated content for meaningful learning experiences.

<div class="audio-control">
🎵 **Video Narration:** Understanding Human Agency in AI-Enhanced TVET Education
</div>

!?[Understanding Human Agency in AI-Enhanced TVET Education] (https://www.youtube.com/watch?v=YLe8XQTsarM)

**Video Summary:** This video introduces the principle of preserving human agency in the use of AI for technical and vocational education. It shows that while AI can support learning, educators remain central in guiding, evaluating, and contextualizing its outputs for meaningful learning experiences.

<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 30px; border-radius: 20px; margin: 30px 0;">

### 🔑 **Key Concept**

**Human Agency in AI Education** = The educator's ability to make informed, critical decisions about when, how, and why to use AI tools while maintaining control over the learning process and outcomes.

</div>

---

## 🗃️ Module 2: TVET-Specific AI Applications & Scenarios

--{{0}}--
 **Work context:**
 
Let's explore how AI applications work in authentic TVET contexts. These detailed scenarios will help you understand the practical applications and critical considerations when using AI systems in your specific teaching environment.

---

### 🔨 **Scenario 1: Construction Technology Training**

<div style="background: linear-gradient(135deg, #ff9a56, #ff6b6b); color: white; padding: 25px; border-radius: 20px; margin: 25px 0; box-shadow: 0 10px 30px rgba(0,0,0,0.2);">

**👩‍🏫 Marina** teaches **Construction Technology** at a vocational college. She's considering using AI tools to help students design sustainable building layouts and generate technical documentation. Her students range from complete beginners to those with some industry experience.

</div>

**Key Questions for Marina:**

- How can AI enhance hands-on learning without replacing practical skills?
- What are the risks of students becoming overly dependent on AI for design thinking?
- How can she ensure AI-generated designs meet actual building codes and safety standards?

**Your Reflection:** What opportunities do you see for AI in construction education?

    [[___]]

**Your Reflection:** What concerns would you have about AI accuracy in this safety-critical field?

    [[___]]

---

### 🚗 **Scenario 2: Automotive Service Technology**

--{{0}}--
Now let's examine how another TVET instructor faces challenges with AI diagnostic tools and the balance between technology assistance and fundamental skill development.

<div style="background: linear-gradient(135deg, #4ecdc4, #44a08d); color: white; padding: 25px; border-radius: 20px; margin: 25px 0; box-shadow: 0 10px 30px rgba(0,0,0,0.2);">

**👨‍🔧 James** instructs **Automotive Service Technology** and is exploring AI diagnostic tools that can help students identify vehicle problems. He worries about students losing fundamental diagnostic thinking skills and becoming too reliant on AI recommendations.

</div>

**Critical Considerations:**

- AI diagnostic tools may provide quick answers but skip the reasoning process
- Students need to understand the *why* behind diagnoses, not just the *what*
- Real-world scenarios often involve variables AI hasn't encountered

> **Activity 1: Critical Analysis Framework**

**Instructions:** Use the framework below to analyze the automotive scenario.

> **Step 1: Identify Benefits**

List potential benefits of AI diagnostic tools in automotive education:

**Educational Benefits:** How could AI enhance learning?

    [[___]]

**Practical Benefits:** What real-world advantages exist?

    [[___]]

> **Step 2: Assess Limitations**

**Technical Limitations:** What can AI diagnostic tools NOT do?

    [[___]]

**Pedagogical Limitations:** How might AI hinder deep learning?

    [[___]]

> **Step 3: Risk Evaluation**

[( )] Low Risk - Minimal impact on student learning
[( )] Medium Risk - Some concerns but manageable
[(X)] High Risk - Significant potential for skill degradation
[[?]] Consider dependency, accuracy, and learning depth

---

## 📊 Module 3: Critical Evaluation Framework for AI Tools

--{{0}}--
Developing a systematic approach to evaluate AI tools is essential for TVET educators. This framework helps you make informed decisions about AI integration while maintaining educational quality and safety standards.

### 🎯 **The TVET AI Evaluation Matrix**

| **Evaluation Criterion** | **Questions to Ask** | **Red Flags** |
|---------------------------|----------------------|---------------|
| **Subject Relevance** | Does the AI tool align with industry standards? | Outdated information, non-standard practices |
| **Skill Development** | Does it enhance or replace critical thinking? | Students bypass problem-solving steps |
| **Safety & Accuracy** | Are AI outputs verified for safety compliance? | Unverified technical specifications |
| **Learning Depth** | Does it promote understanding or just answers? | Surface-level engagement |
| **Ethical Considerations** | Are data privacy and bias addressed? | Student data misuse, biased outputs |

### 🧠 **Interactive Quiz: AI Tool Evaluation**

> **Knowledge Check 1: Benefits vs. Risks**

You're teaching **Electrical Installation** and considering an AI tool that generates wiring diagrams based on room descriptions. What's your primary concern?

[( )] The tool might be too slow for classroom use
[(X)] Students might not learn electrical safety principles
[( )] The tool costs too much for the budget
[( )] Students might find it too difficult to use
[[?]] Focus on learning outcomes and safety implications

> **Knowledge Check 2: Appropriate Use Cases**

Which scenario represents the MOST appropriate use of AI in TVET education?

[( )] AI completely replaces hands-on practice sessions
[( )] Students use AI to write all their technical reports
[(X)] AI provides multiple practice scenarios for diagnostic training
[( )] AI makes all assessment decisions about student competence
[[?]] Consider which option enhances rather than replaces learning

## Further Reading & Resources

Expand your knowledge with these carefully curated resources for TVET AI integration.

> **Essential Resources**

* [UNESCO AI Competency Framework for Educators](https://unesdoc.unesco.org/ark:/48223/pf0000391104) - Comprehensive framework for AI literacy in education
* [EU Ethics Guidelines for Trustworthy AI](https://ec.europa.eu/digital-single-market/en/news/ethics-guidelines-trustworthy-ai) - Ethical principles for AI development and deployment
* [TVET AI Integration Best Practices Guide](https://www.unevoc.unesco.org/go.php?q=page_ai_tvet) - UNESCO-UNEVOC guidelines for technical education
* [Partnership on AI - Education Working Group](https://partnershiponai.org/program/education/) - Collaborative AI research for educational applications
* [MIT's Moral Machine Experiment - AI Ethics](http://moralmachine.mit.edu/) - Explore ethical decision-making in AI systems

> **Extended Learning**

* [AI in Vocational Education: Opportunities and Challenges](https://www.cedefop.europa.eu/en/publications/ai-vocational-education) - Comprehensive CEDEFOP analysis
* [Ethical AI for Education](https://www.edtechpolicy.org/ethical-ai) - Policy framework for responsible AI use
* [Human-Centered AI Design Principles](https://hai.stanford.edu/about) - Stanford HAI research and guidelines
* [TVET Digital Transformation Guide](https://www.ilo.org/skills/areas/skills-training-for-poverty-reduction/WCMS_740847/lang--en/index.htm) - ILO perspective on skills development
* [Critical Thinking in Digital Age Education](https://www.brookings.edu/research/critical-thinking-digital-age/) - Maintaining analytical skills with technology

## Course Navigation

> **📚 All Course Nuggets**

1. [AI Orientation for TVET Educators](https://liascript.github.io/course/?https://github.com/OVGU-VET-TechEd/Self_Learning_Nuggets_AI_Basics/blob/main/01_Orientation-V3.md) - Current
2. **[AI Basics](https://raw.githubusercontent.com/OVGU-VET-TechEd/Self_Learning_Nuggets_AI_Basics/refs/heads/main/02_AI_Basics-V3.md) - Next**
3. [AI Tools Presentation](https://raw.githubusercontent.com/OVGU-VET-TechEd/Self_Learning_Nuggets_AI_Basics/refs/heads/main/03_Tool_Presentations-V3.md) - Upcoming
4. [Prompting](https://raw.githubusercontent.com/OVGU-VET-TechEd/Self_Learning_Nuggets_AI_Basics/refs/heads/main/04_Prompting_V2.md) - Upcoming
5. [Assessment and Evaluation with AI](https://raw.githubusercontent.com/OVGU-VET-TechEd/Self_Learning_Nuggets_AI_Basics/refs/heads/main/05_Quality_%26_Ethics_V2.md) - Upcoming

---

**🎉 Congratulations on completing Virtual Training Nugget 2.1!**

You've developed a critical framework for evaluating AI tools in TVET education while maintaining human agency and educational quality. Your thoughtful approach to balancing innovation with pedagogical soundness will serve your students well.

<div class="contact-info">
**Support & Feedback:**
📧 Email: asset-project@unesco.org
🌐 Course Portal: https://unesco-asset-portal.example.com
📋 Feedback Form: https://feedback.unesco-asset.example.com
</div>

> *"The best AI integration in TVET education amplifies human expertise rather than replacing it. Your critical evaluation skills ensure that technology serves learning, not the other way around."*

# END

<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="650" viewBox="0 0 1280 720" role="img" aria-labelledby="title desc">
  <title id="title">End Slide – Technical Accuracy Motivation</title>
  <desc id="desc">Thank you slide emphasising technical accuracy in TVET AI content.</desc>

  <!-- Background -->
  <defs>
    <linearGradient id="bgGrad" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#0f172a"/>
      <stop offset="100%" stop-color="#0b2447"/>
    </linearGradient>

    <filter id="softShadow" x="-50%" y="-50%" width="200%" height="200%">
      <feDropShadow dx="0" dy="8" stdDeviation="20" flood-color="#000" flood-opacity="0.4"/>
    </filter>
  </defs>

  <rect width="1280" height="720" fill="url(#bgGrad)"/>

  <!-- Big rounded panel -->
  <rect x="80" y="80" rx="24" ry="24" width="1120" height="560" fill="rgba(255,255,255,0.04)" stroke="rgba(255,255,255,0.06)" stroke-width="1" filter="url(#softShadow)"/>

  <!-- Left accent bar -->
  <rect x="100" y="120" width="16" height="480" rx="8" fill="#10b981" opacity="0.95"/>

  <!-- Headline -->
  <text x="180" y="210" font-family="Inter, Arial, Helvetica, sans-serif" font-size="48" font-weight="700" fill="#ffffff">
    Thank you and keep striving for accuracy
  </text>

  <!-- Divider line -->
  <line x1="180" y1="230" x2="1060" y2="230" stroke="rgba(255,255,255,0.06)" stroke-width="2"/>

  <!-- Motivational line (main) -->
  <text x="180" y="320" font-family="Inter, Arial, Helvetica, sans-serif" font-size="28" fill="#e6f0ff">
    Technical accuracy matters:
    * it empowers learning 
    * builds trust
    * and ensures safe, effective skills for the workplace
  </text>

  <!-- Secondary short CTA -->
  <text x="180" y="370" font-family="Inter, Arial, Helvetica, sans-serif" font-size="20" fill="#bfe6d9">
    Aim for rigor. Validate with experts. Iterate with learners.
  </text>

  <!-- Footer -->
  <g transform="translate(180,460)">
    <circle cx="0" cy="0" r="28" fill="#0ea5a3" opacity="0.95"/>
    <text x="48" y="8" font-family="Inter, Arial, Helvetica, sans-serif" font-size="16" fill="#dffcf6">
      TVET • AI • Quality
    </text>
  </g>

  <!-- Decorative icon (gears) top-right -->
  <g transform="translate(980,140) scale(1.2)" fill="none" stroke="#ffffff" stroke-opacity="0.08" stroke-width="2">
    <circle cx="40" cy="40" r="28"/>
    <path d="M40 16v6M40 64v6M24 40h6M56 40h6M30 24l4 4M50 24l-4 4M30 56l4-4M50 56l-4-4" stroke-linecap="round"/>
    <circle cx="100" cy="40" r="18" fill="none"/>
    <path d="M100 32v4M96 40h8" stroke-linecap="round"/>
  </g>

  <!-- Accessibility note (invisible to visual layout but readable) -->
  <rect x="0" y="0" width="1" height="1" fill="transparent" aria-hidden="false"/>
</svg>

<!-- UNEVOC -->
<div style="position: fixed; bottom: 1px; left: 20px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UNESCO-UNEVOC_logo.png?raw=true" alt="UNEVOC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UNEVOC</div>
</div>

<!-- ASSET -->
<div style="position: fixed; bottom: 1px; left: 180px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/ASSET_icon.png?raw=true" alt="ASSET Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">ASSET</div>
</div>

<!-- HWK Blume -->
<div style="position: fixed; bottom: 1px; left: 340px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/HWK_Blume.png?raw=true" alt="HWK Blume Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 7px;">HWK Blume</div>
</div>

<!-- GIZ -->
<div style="position: fixed; bottom: 1px; left: 500px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/giz-logo.gif?raw=true" alt="GIZ Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">GIZ</div>
</div>

<!-- UoVT -->
<div style="position: fixed; bottom: 1px; left: 660px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/UoVT_Logo.png?raw=true" alt="UoVT Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">UoVT</div>
</div>

<!-- OVGU -->
<div style="position: fixed; bottom: 1px; left: 820px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/Masub27/Intro/blob/main/ovgu.png?raw=true" alt="OVGU Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">OVGU</div>
</div>

<!-- HRDC -->
<div style="position: fixed; bottom: 1px; left: 980px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/hrdc_logo.png?raw=true" alt="HRDC Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">HRDC</div>
</div>

<!-- MITD -->
<div style="position: fixed; bottom: 1px; left: 1140px; opacity: 0.9; z-index: 1000; text-align: center; width: 100px;">
  <img src="https://github.com/OVGU-VET-TechEd/ASSET_UNESCO_Coinitiative/blob/main/media/mitd_logo.png?raw=true" alt="MITD Logo" style="height: 60px; width: auto; border-radius: 10px;" />
  <div style="font-size: 0.8em; color: #555; margin-top: 5px;">MITD</div>
</div>









