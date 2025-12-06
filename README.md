<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1"/>
<title>DyanVa Family Services Ltd. — Website</title>

<!-- ============ ALL CSS COMBINED ============ -->
<style>
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:Arial,Helvetica,sans-serif;background:#f7f8fb;color:#1a1a1a;line-height:1.45;}

.header{background:#fff;box-shadow:0 2px 8px rgba(0,0,0,.06);position:sticky;top:0;z-index:30;}
.header .inner{display:flex;align-items:center;justify-content:space-between;padding:12px 0;width:94%;max-width:1100px;margin:0 auto;}
.brand{display:flex;align-items:center;gap:12px;text-decoration:none;color:#000;}
.logo-img{width:56px;height:56px;border-radius:8px;object-fit:cover;display:block;}

/* nav */
.nav{display:flex;gap:14px;}
.nav a{text-decoration:none;padding:8px 10px;border-radius:8px;color:#111827;font-weight:700;font-size:14px;}
.nav a:hover,.nav a.active{background:#eef2ff;color:#0033ff;}

/* hamburger */
.hamburger{display:none;border:0;background:transparent;font-size:22px;cursor:pointer;}

/* container and layout */
.container{width:94%;max-width:1100px;margin:0 auto;padding:32px 0;}

.hero{
  padding:64px 0;
  color:#fff;
  text-align:left;
  background-image:linear-gradient(rgba(3,19,102,0.48), rgba(3,19,102,0.48)), url('https://i.ibb.co/2YC1sBD8/hero.jpg');
  background-size:cover;
  background-position:center;
}
.hero h1{font-size:34px;margin-bottom:8px;letter-spacing:0.2px;}
.hero p{color:rgba(255,255,255,0.95);margin-top:10px;margin-bottom:18px;max-width:760px;}
.cta-row{display:flex;gap:12px;margin-top:12px;}
.btn{padding:10px 16px;border-radius:10px;font-weight:700;text-decoration:none;display:inline-block;}
.btn-primary{background:#0033ff;color:#fff;box-shadow:0 6px 18px rgba(0,51,255,.12);}
.btn-outline{border:1px solid #dbeafe;color:#0033ff;background:transparent;}

/* cards */
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:16px;margin-top:20px;}
.card{background:#fff;padding:16px;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,.05);}
.card h3{margin-bottom:6px;}
.card p{color:#475569;font-size:14px;}

/* forms */
.input,textarea,select{width:100%;padding:10px;border-radius:8px;border:1px solid #ddd;margin-bottom:10px;font-size:14px;}
textarea{min-height:120px;resize:vertical;}

/* modal styling */
.team-modal{
  display:none;
  position:fixed;
  z-index:999;
  left:0;top:0;
  width:100%;height:100%;
  background:rgba(0,0,0,0.65);
  padding-top:60px;
}
.team-modal-content{
  background:#fff;
  margin:auto;
  padding:20px;
  border-radius:10px;
  max-width:520px;
  color:#003366;
}
.team-close{
  float:right;
  font-size:28px;
  cursor:pointer;
  color:#003366;
}

/* footer */
.footer{background:#0b1220;color:#cbd5e1;padding:28px 0;text-align:center;margin-top:40px;}
.footer a{color:#cbd5e1;text-decoration:none;font-weight:600;}

.small-muted{color:#6b7280;font-size:13px;}
.section-title{font-size:20px;margin-bottom:12px;color:#0b1220;font-weight:800;padding-top:6px;}
.address-row{margin-top:12px;color:#eef2ff;opacity:0.95;font-weight:600;}

/* responsive */
@media(max-width:900px){
  .nav{display:none;}
  .hamburger{display:block;}
  .hero{padding:40px 0;}
  .hero h1{font-size:26px;}
}
/* Policies expand/collapse */
.policy-details {
  display: none;
  margin-top: 10px;
  color: #374151;
  font-size: 14px;
}

.card:hover {
  cursor: pointer;
}
</style>

</head>
<body>

<!-- ============ HEADER ============ -->
<header class="header">
  <div class="inner">
    <a href="#home" class="brand" aria-label="DyanVa Family Services Ltd. Home">
      <img src="assets/logo.jpg">
      <div>
        <div style="font-weight:800;color:#0b1220;">DyanVa Family Services Ltd.</div>
        <div style="font-size:12px;color:#666;font-weight:600;">Empowering lives, One Step at a Time</div>
      </div>
    </a>

    <nav class="nav" aria-label="Main navigation">
      <a href="#home" class="active">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#policies">Policies</a>
      <a href="#careers">Careers</a>
      <a href="#resources">Resources</a>
      <a href="#contact">Contact</a>
      <a href="javascript:void(0)" onclick="openAdmin()" class="btn btn-outline">Admin</a>
    </nav>

    <button class="hamburger" aria-label="Toggle menu">☰</button>
  </div>
</header>

<!-- ============ HOME ============ -->
<section id="home" class="hero">
  <div class="container">
    <h1>Person-centred care that empowers lives</h1>
    <p>At DyanVa Family Services Ltd., we provide supportive living, group care, and community integration services for youth and adults.</p>

    <div class="cta-row">
      <a href="javascript:void(0)" onclick="openBooking()" class="btn btn-primary">Book Appointment</a>
      <a href="#policies" class="btn btn-outline">View Policies</a>
    </div>

    <div class="address-row" style="margin-top:14px;">
      📍 17911 – 60 Street NW, Edmonton, Alberta T5Y 3W9 • 📞 (587) 712-2323 • ✉️ dyanvafamilyser1525@outlook.com
    </div>

    <div class="cards" style="margin-top:20px;">
      <div class="card"><h3>Supportive Living</h3><p>Independence-building programs for adults.</p></div>
      <div class="card"><h3>Group Care (Youth)</h3><p>Safe, structured environments for youth.</p></div>
      <div class="card"><h3>Community Integration</h3><p>Life skills programs fostering inclusion.</p></div>
      <div class="card"><h3>Transitional Support</h3><p>Planning for independent living pathways.</p></div>
    </div>
  </div>
</section>

<!-- ============ ABOUT ============ -->
<section id="about" class="container">
  <h2 class="section-title">About Us</h2>

  <div class="card">
    <h3>Organizational Overview</h3>
    <p class="small-muted">DyanVa Family Services Ltd. delivers person-centred services to youth and adults with developmental, emotional, and behavioural needs.</p>
  </div>

  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:12px;">
    <div class="card"><h3>Mission</h3><p>To deliver compassionate, person-centred care that uplifts and empowers lives.</p></div>
    <div class="card"><h3>Vision</h3><p>To be recognized as a leading Alberta care organisation.</p></div>
    <div class="card"><h3>Core Values</h3>
      <ul style="margin-top:8px;color:#374151;">
        <li>Respect & Dignity</li>
        <li>Integrity & Accountability</li>
        <li>Compassion & Empathy</li>
        <li>Teamwork & Collaboration</li>
        <li>Safety & Compliance</li>
      </ul>
    </div>
  </div>
</section>

<!-- ============ TEAM ============ -->
<section id="team" class="container" style="padding:60px 20px;">
  <h2 class="section-title" style="text-align:center;font-size:32px;color:#004aad;">Meet Our Leadership Team</h2>

  <div class="cards" style="display:flex;gap:25px;justify-content:center;flex-wrap:wrap;">

    <div class="card" style="text-align:center;border:2px solid #bfdcff;">
      <img src="assets/founder.jpg" alt="Prince Flowers — Executive Director" style="max-width:140px;border-radius:8px;">
      <h3 style="color:#004aad;">Prince Flowers</h3>
      <p class="small-muted">Executive Director</p>
      <button class="btn btn-outline" onclick="openModal('m1')">Read More</button>
    </div>

    <div class="card" style="text-align:center;border:2px solid #bfdcff;">
      <img src="assets/co-founder.jpg" alt="Nancee Daniels — Co-Director" style="width:120px;height:120px;border-radius:50%;">
      <h3 style="color:#004aad;">Nancee Daniels</h3>
      <p class="small-muted">Co-Director</p>
      <button class="btn btn-outline" onclick="openModal('m2')">Read More</button>
    </div>

    <div class="card" style="text-align:center;border:2px solid #bfdcff;">
      <img src="assets/chairman.jpg" alt="Chris Miller — Chairman" style="width:120px;height:120px;border-radius:50%;">
      <h3 style="color:#004aad;">Chris Miller</h3>
      <p class="small-muted">Chairman</p>
      <button class="btn btn-outline" onclick="openModal('m3')">Read More</button>
    </div>

  </div>
</section>

<!-- TEAM MODALS -->
<div id="m1" class="team-modal" role="dialog" aria-modal="true" aria-labelledby="m1-title">
  <div class="team-modal-content">
    <span class="team-close" onclick="closeModal('m1')">&times;</span>
    <h2 id="m1-title" style="color:#004aad;">Prince Flowers — Executive Director</h2>
    <p>Provides strategic leadership and oversight for DyanVa Family Services Ltd. Ensures that all programs, staff operations, and client care services meet the organization’s quality, safety, and compliance standards. Guides policy implementation, partnership development, and service expansion while upholding the company’s mission of providing compassionate, person-centered support to individuals and families.</p>
  </div>
</div>

<div id="m2" class="team-modal" role="dialog" aria-modal="true" aria-labelledby="m2-title">
  <div class="team-modal-content">
    <span class="team-close" onclick="closeModal('m2')">&times;</span>
    <h2 id="m2-title" style="color:#004aad;">Nancee Daniels — Co-Director</h2>
    <p>Oversees daily operations across all DyanVa programs and services. Ensures that staffing, scheduling, and program delivery align with organisational standards and regulatory compliance. Supports the Executive Director in strategic planning, resource management, and continuous improvement of service quality.</p>
  </div>
</div>

<div id="m3" class="team-modal" role="dialog" aria-modal="true" aria-labelledby="m3-title">
  <div class="team-modal-content">
    <span class="team-close" onclick="closeModal('m3')">&times;</span>
    <h2 id="m3-title" style="color:#004aad;">Chris Miller — Chairman</h2>
    <p>Provides strategic leadership and governance oversight for DyanVa Family Services Ltd. Ensures that the organization’s mission, vision, and values are upheld, guiding long-term planning, risk management, and stakeholder engagement. Works closely with the Executive Director and Co-Directors to maintain excellence in service delivery, compliance, and organizational growth.</p>
  </div>
</div>

<!-- ============ SERVICES ============ -->
<section id="services" class="container">
  <h2 class="section-title">Our Services</h2>
  <div class="cards">
    <div class="card"><h3>Supportive Living</h3><p>24/7 adult support services.</p></div>
    <div class="card"><h3>Group Care (Youth)</h3><p>Residential and behavioural support.</p></div>
    <div class="card"><h3>Community Integration</h3><p>Life skills training.</p></div>
    <div class="card"><h3>Transitional Support</h3><p>Personal development planning.</p></div>
    <div class="card"><h3>Crisis Response</h3><p>Short-term stabilization.</p></div>
  </div>
</section>

<!-- ============ POLICIES ============ -->
<section id="policies" class="container">
  <h2 class="section-title">Policies & Standards</h2>

<div class="card" onclick="togglePolicy(this)">
  <h3>Resident Rights</h3>
  <p>Protection of dignity, privacy, and autonomy.</p>
  <div class="policy-details">
    <p>Our goal is to maintain an environment where residents feel heard, respected, and supported in reaching their full potential.
Resident Rights
All residents have the right to:
1. Respect & Dignity – To be treated with kindness, courtesy, and compassion.
2. Safety – To live in a secure, clean, and healthy environment.
3. Privacy – To personal space, confidential communication, and the protection of personal information.
4. Participation – To contribute to personal care planning and make choices about daily living.
5. Communication – To express opinions, feelings, and preferences without fear of retaliation.
6. Cultural Identity – To observe personal religious or cultural practices.
7. Personal Property – To own, use, and enjoy personal belongings within reasonable safety limits.
8. Access to Information – To review personal records in accordance with privacy regulations.
9. Freedom from Abuse & Neglect – To live free from verbal, physical, emotional, sexual, or financial abuse.
10. Grievance & Appeal – To raise concerns or complaints through a fair and transparent process.

Resident Responsibilities
Residents also share in maintaining a respectful, safe, and cooperative living environment.
They are expected to:
1. Treat others (staff and peers) with respect and kindness.
2. Follow established home guidelines and safety rules.
3. Respect the property and privacy of others.
4. Participate in programming and personal growth activities.
5. Communicate openly with staff about concerns or needs.
6. Refrain from behaviour that endangers themselves or others.
7. Take responsibility, as able, for personal care and hygiene.
8. Contribute positively to household routines and community life.</p>
  </div>
</div>

<div class="card" onclick="togglePolicy(this)">
  <h3>Health & Safety</h3>
  <p>OHS, emergency, and infection control policies.</p>
  <div class="policy-details">
    <p>DyanVa Family Services Ltd. is committed to ensuring that every person within its facilities is protected from injury or illness. To promote and maintain a safe, healthy, and hazard-free environment for residents, staff, and visitors, we adhere to Alberta’s Occupational Health and Safety (OHS) regulations and supportive living standards. Safety is a shared responsibility, and all staff, residents, and management work together to identify risks, report hazards, and uphold safe practices. Our ultimate goal is to prevent accidents before they occur and to ensure that all emergencies are managed calmly, confidently, and efficiently.
Health & Safety Objectives
The primary objective of our health and safety program is to protect the well-being of residents, staff, and visitors. We aim to maintain full compliance with all municipal and provincial health and safety standards. Workplace injuries are prevented through proactive training and awareness, while ongoing reporting and hazard identification are strongly encouraged. Additionally, we ensure that emergency procedures are well understood and practiced by all members of the organization.
Staff Responsibilities
All staff are required to follow health, safety, and infection-control procedures at all times. Hazards, unsafe conditions, or incidents must be reported immediately to a supervisor. Staff are expected to attend mandatory safety and emergency preparedness training and use protective equipment (PPE) as required. Accurate incident and injury reports must be maintained, and staff are encouraged to model safe practices for both residents and coworkers.
Management Responsibilities
Management is responsible for providing a safe physical environment, including cleanliness, adequate lighting, fire safety, and secure exits. Regular safety inspections and audits must be conducted, and any safety incidents investigated and resolved promptly. Management is also tasked with supplying the necessary training, PPE, and first aid materials. It is essential that all staff have access to emergency protocols and contact numbers to ensure a quick and effective response in any situation.    Resident Involvement
Residents are encouraged to:
Participate in safety drills.
Report unsafe conditions to staff.
Follow guidance during emergencies.
Maintain personal hygiene and report illness promptly.

Safety is everyone’s responsibility — when we care for each other, we protect each other.💙</p>
  </div>
</div>

<div class="card" onclick="togglePolicy(this)">
  <h3>Confidentiality</h3>
  <p>FOIP / PIPA / HIA-compliant data handling.</p>
  <div class="policy-details">
    <p>Medication information is considered private health information and is protected under applicable privacy legislation.
All medication records are stored in secure files with restricted access.</p>
  </div>
</div>

<div class="card" onclick="togglePolicy(this)">
  <h3>Admission & Discharge</h3>
  <p>Clear and person-centred processes.</p>
  <div class="policy-details">
    <p>Purpose
The purpose of this policy is to ensure that the admission and discharge of residents at DyanVa Family Services Ltd. are conducted in a fair, transparent, and person-centred manner, consistent with Alberta’s licensing and care standards.
Policy Statement
DyanVa Family Services Ltd. accepts residents whose needs align with our program’s purpose, staffing qualifications, and available resources. All admissions and discharges are handled with sensitivity, professionalism, and respect for the rights and dignity of the resident.
Admission Criteria
Admission decisions are based on a thorough assessment of the resident’s developmental, behavioural, and emotional needs. Compatibility with existing residents and program capacity is considered, alongside safety considerations for both the individual and others in care. Referrals and documentation from authorized agencies, such as Alberta Health Services, PDD, or Children’s Services, are required. Admission is confirmed through a signed Service Agreement that outlines program expectations, resident rights, and responsibilities.
Admission Procedures
The admission process begins with a review of referral documents, assessments, and recommendations by management. A pre-admission interview is conducted with the resident, and, where applicable, their family or caseworker, to discuss care goals and program expectations. The team then evaluates the resident’s potential impact on current residents and program resources. Once approved by the Director, all intake forms, medical records, and consents are completed. Finally, new residents receive an orientation, including a friendly introduction to the home, daily routines, staff, and peer community.
Resident Rights During Admission
Residents have the right to be treated with respect and dignity, to be informed about program rules, expectations, and routines, and to receive clear information about grievance procedures and privacy rights. They also have access to personal belongings and family contact, unless restrictions are necessary for safety reasons.
Discharge Criteria
A resident may be discharged when program goals have been achieved and they are ready to transition to a lower level of support, when the resident, guardian, or placing agency requests discharge, when the resident’s needs exceed the program’s capacity or resources, or when safety risks require alternate placement. All discharges are planned collaboratively whenever possible.
Discharge Procedures
The discharge process begins with a case review in consultation with the resident, guardian, and referral agency. Transition planning ensures support for the next placement, including proper documentation and continuity of care. A discharge summary and exit report are completed and signed, and all personal belongings are returned to the resident or guardian. Where appropriate, staff may conduct a follow-up call or report to ensure a successful transition.
Emergency Discharge
In rare cases where immediate removal is necessary for safety reasons, the Director will notify the placing agency immediately, document the incident and rationale in detail, and ensure the resident’s safety and dignity throughout the transition.</p>
  </div>
</div>

  <a href="https://wp.me/agXV2H-7" class="btn btn-primary">Download Full Policy Manual (PDF)</a>
</section>

<!-- ============ CAREERS ============ -->
<section id="careers" class="container">
  <h2 class="section-title">Careers</h2>
  <div class="card"><h3>Join Our Team</h3><p>We are always looking for talented and compassionate individuals. Submit your application below.</p></div>

  <div class="card">
    <h3>Apply Now</h3>
    <form id="careerForm" action="send-application.php" method="post" enctype="multipart/form-data" style="margin-top:20px; display:grid; gap:12px; max-width:500px;">
      <label class="sr-only" for="name">Full name</label>
      <input type="text" id="name" name="name" class="input" placeholder="Full Name*" required>
      <label class="sr-only" for="email">Email</label>
      <input type="email" id="email" name="email" class="input" placeholder="Email*" required>
      <label class="sr-only" for="phone">Phone</label>
      <input type="tel" id="phone" name="phone" class="input" placeholder="Phone Number*" required>
      <input type="text" id="position" name="position" class="input" placeholder="Position Applying For*" required>
      <textarea id="message" name="message" placeholder="Message / Cover Letter (Optional)"></textarea>

      <!-- Drag & Drop -->
      <div id="drop-area" style="border:2px dashed #0033ff; border-radius:10px; padding:20px; text-align:center; cursor:pointer;">
        <p id="drop-text">Drag & Drop CV here or click to browse</p>
        <input type="file" id="cv" name="cv" accept=".pdf,.doc,.docx" required style="display:none;">
      </div>
      <p id="file-name" style="font-size:14px;color:#0b1220;font-weight:600;"></p>

      <button type="submit" class="btn btn-primary">Submit Application</button>
    </form>
  </div>
</section>

<style>
#drop-area.hover {background-color:#eef2ff;}
.sr-only { position: absolute !important; height: 1px; width: 1px; overflow: hidden; clip: rect(1px, 1px, 1px, 1px); white-space: nowrap; }
</style>

<!-- ============ RESOURCES ============ -->
<section id="resources" class="container">
  <h2 class="section-title">Resources</h2>
  <div class="card">
    <h3>Downloads</h3>
    <ul>
      <li><a href="policy-manual.pdf" download>Policy Manual (PDF)</a></li>
    </ul>
  </div>
</section>

<!-- ============ CONTACT ============ -->
<section id="contact" class="container">
  <h2 class="section-title">Contact Us</h2>

  <div class="card">
    <h3>Office</h3>
    <p><strong>Address:</strong> 17911 – 60 Street NW, Edmonton, Alberta T5Y 3W9</p>
    <p><strong>Phone:</strong> (587) 712-2323</p>
    <p><strong>Email:</strong> <a href="mailto:dyanvafamilyser1525@outlook.com">dyanvafamilyser1525@outlook.com</a></p>
  </div>

  <div class="card">
    <h3>Send a Message</h3>
    <form action="send-message.php" method="post">
      <input class="input" name="name" placeholder="Your Name" required>
      <input class="input" name="email" type="email" placeholder="Your Email" required>
      <input class="input" name="phone" placeholder="Phone Number (optional)">
      <textarea class="input" name="message" placeholder="Message" required></textarea>
      <button class="btn btn-primary">Send</button>
    </form>
  </div>

  <div class="card">
    <h3>Location Map</h3>
    <iframe width="100%" height="300" loading="lazy" style="border:0"
      src="https://www.google.com/maps?q=17911+60+Street+NW+Edmonton+AB&output=embed" title="Map to DyanVa Family Services">
    </iframe>
  </div>
</section>

<!-- ============ FOOTER ============ -->
<footer class="footer">
  <div style="max-width:1100px;margin:0 auto;">
    <div style="display:flex;flex-direction:column;gap:8px;align-items:center;">
      <div style="font-weight:700;">DyanVa Family Services Ltd.</div>
      <div class="small-muted">17911 – 60 Street NW, Edmonton, Alberta T5Y 3W9 • (587) 712-2323</div>
      <div style="margin-top:8px;">© 2025 DyanVa Family Services Ltd. All rights reserved.</div>
    </div>
  </div>
</footer>

<!-- ============ MODALS: BOOKING & ADMIN ============ -->
<div id="bookingModal" class="team-modal" role="dialog" aria-modal="true" aria-labelledby="booking-title">
  <div class="team-modal-content" style="max-width:600px;">
    <span class="team-close" onclick="closeBooking()">&times;</span>
    <h2 id="booking-title" style="color:#004aad;margin-bottom:10px;">Book an Appointment</h2>

    <form id="bookingForm" method="POST" action="send-booking.php" style="display:grid;gap:12px;">
      <input class="input" name="name" required placeholder="Full Name*">
      <input class="input" name="email" type="email" required placeholder="Email*">
      <input class="input" name="phone" required placeholder="Phone Number*">

      <select class="input" name="service" required>
        <option value="">Select Service</option>
        <option>Supportive Living</option>
        <option>Group Care (Youth)</option>
        <option>Community Integration</option>
        <option>Transitional Support</option>
        <option>Crisis Response</option>
      </select>

      <input class="input" name="date" type="date" required>
      <input class="input" name="time" type="time" required>

      <textarea class="input" name="notes" placeholder="Additional Notes (optional)"></textarea>

      <button class="btn btn-primary" type="submit">Submit Booking</button>
    </form>
  </div>
</div>

<div id="adminModal" class="team-modal" role="dialog" aria-modal="true" aria-labelledby="admin-title">
  <div class="team-modal-content" style="max-width:400px;">
    <span class="team-close" onclick="closeAdmin()">&times;</span>
    <h2 id="admin-title" style="color:#004aad;margin-bottom:15px;text-align:center;">Admin Login</h2>

    <!-- Login Form: POSTs to server for secure authentication -->
    <form id="adminForm" action="admin-login.php" method="post" style="display:grid;gap:12px;">
      <input class="input" name="email" type="email" placeholder="Outlook Email*" required>
      <input class="input" name="password" type="password" placeholder="Password*" required>
      <button class="btn btn-primary" type="submit">Login</button>
      <p class="error" id="adminError" style="display:none;color:red;text-align:center;">Invalid email or password</p>
      <p style="text-align:center;font-size:12px;color:#555;">
        Forgot password? <a href="#" id="showChangePass">Click here</a>
      </p>
    </form>

    <!-- Password Change Form (hidden by default) - posts to server to handle securely -->
    <form id="changePassForm" action="change-password.php" method="post" style="display:none;grid-gap:12px;margin-top:10px;">
      <input class="input" name="email" type="email" placeholder="Admin Email*" required>
      <input class="input" name="newPassword" type="password" placeholder="New Password*" required>
      <input class="input" name="confirmPassword" type="password" placeholder="Confirm Password*" required>
      <button class="btn btn-primary" type="submit" id="changePassBtn">Change Password</button>
      <p class="success" id="changeSuccess" style="display:none;color:green;text-align:center;">Password updated successfully!</p>
      <p class="error" id="changeError" style="display:none;color:red;text-align:center;">Passwords do not match</p>
      <p style="text-align:center;font-size:12px;color:#555;">
        <a href="#" id="backToLogin">Back to Login</a>
      </p>
    </form>

  </div>
</div>

<!-- ============ CONSOLIDATED JS (place just before closing body) ============ -->
<script>
/* Consolidated JS: fixes duplicated scripts and stray tags; ensures element checks before use */

// NAV hamburger
(function(){
  const nav = document.querySelector(".nav");
  const burger = document.querySelector(".hamburger");
  if (!burger || !nav) return;
  burger.addEventListener("click", () => {
    const isVisible = getComputedStyle(nav).display === "flex";
    if (isVisible) {
      nav.style.display = "none";
    } else {
      nav.style.display = "flex";
      nav.style.flexDirection = "column";
      nav.style.background = "#fff";
      nav.style.position = "absolute";
      nav.style.right = "20px";
      nav.style.top = "64px";
      nav.style.padding = "12px";
      nav.style.borderRadius = "10px";
      nav.style.boxShadow = "0 6px 20px rgba(0,0,0,.10)";
    }
  });
})();

// Drag & Drop CV upload (guards for missing elements)
(function(){
  const dropArea = document.getElementById("drop-area");
  const fileInput = document.getElementById("cv");
  const fileNameDisplay = document.getElementById("file-name");
  if (!dropArea || !fileInput) return;

  // click to open file dialog
  dropArea.addEventListener("click", ()=> fileInput.click());

  // handle file selection
  fileInput.addEventListener("change", ()=>{
      if(fileInput.files.length > 0 && fileNameDisplay){
          fileNameDisplay.textContent = "Selected file: " + fileInput.files[0].name;
      }
  });

  // drag over
  dropArea.addEventListener("dragover", (e)=>{
      e.preventDefault();
      dropArea.classList.add("hover");
  });

  // drag leave
  dropArea.addEventListener("dragleave", ()=>{
      dropArea.classList.remove("hover");
  });

  // drop file
  dropArea.addEventListener("drop", (e)=>{
      e.preventDefault();
      dropArea.classList.remove("hover");
      const files = e.dataTransfer.files;
      if(files.length > 0){
          fileInput.files = files;
          if(fileNameDisplay) fileNameDisplay.textContent = "Selected file: " + files[0].name;
      }
  });
})();

// Modal helpers and policy toggle
(function(){
  function showModal(id){ const el = document.getElementById(id); if(el) el.style.display = "block"; }
  function hideModal(id){ const el = document.getElementById(id); if(el) el.style.display = "none"; }

  // expose functions for inline onclick attributes
  window.openBooking = function(){ showModal("bookingModal"); };
  window.closeBooking = function(){ hideModal("bookingModal"); };
  window.openAdmin = function(){ showModal("adminModal"); };
  window.closeAdmin = function(){ hideModal("adminModal"); };
  window.openModal = function(id){ showModal(id); };
  window.closeModal = function(id){ hideModal(id); };

  window.togglePolicy = function(card){
    if(!card) return;
    const details = card.querySelector('.policy-details');
    if(!details) return;
    details.style.display = (details.style.display === 'block') ? 'none' : 'block';
  };

  // Close any open modal when clicking outside content
  window.addEventListener("click", function(event){
    document.querySelectorAll(".team-modal").forEach(m => {
      if (event.target === m) m.style.display = "none";
    });
  });

  // Close when pressing Escape
  window.addEventListener("keydown", function(e){
    if(e.key === "Escape"){
      document.querySelectorAll(".team-modal").forEach(m => { m.style.display = "none"; });
    }
  });

  // Close buttons (delegated)
  document.addEventListener("click", function(e){
    if (e.target && e.target.classList.contains("team-close")) {
      const modal = e.target.closest(".team-modal");
      if(modal) modal.style.display = "none";
    }
  });
})();

// Admin modal: UI-only toggles; server endpoints handle auth/change-password
(function(){
  const adminForm = document.getElementById("adminForm");
  const changePassForm = document.getElementById("changePassForm");
  const adminError = document.getElementById("adminError");
  const changeError = document.getElementById("changeError");
  const changeSuccess = document.getElementById("changeSuccess");

  const showChangePass = document.getElementById("showChangePass");
  const backToLogin = document.getElementById("backToLogin");

  if (showChangePass && adminForm && changePassForm) {
    showChangePass.addEventListener("click", function(e){
      e.preventDefault();
      adminForm.style.display = "none";
      changePassForm.style.display = "grid";
      if (adminError) adminError.style.display = "none";
      if (changeError) changeError.style.display = "none";
      if (changeSuccess) changeSuccess.style.display = "none";
    });
  }

  if (backToLogin && adminForm && changePassForm) {
    backToLogin.addEventListener("click", function(e){
      e.preventDefault();
      changePassForm.style.display = "none";
      adminForm.style.display = "grid";
      if (changeError) changeError.style.display = "none";
      if (changeSuccess) changeSuccess.style.display = "none";
      if (adminError) adminError.style.display = "none";
    });
  }

  // Prevent showing client-side "invalid" indicators — rely on server to return messages.
  if (adminForm) {
    // If server returns an error, ensure adminError can be shown by server or JS after response.
    adminForm.addEventListener("submit", function(){
      if (adminError) adminError.style.display = "none";
      // The form posts to admin-login.php (server should handle validation and redirect).
    });
  }

  if (changePassForm) {
    changePassForm.addEventListener("submit", function(e){
      // Basic client-side check to avoid unnecessary server roundtrip
      const newPass = changePassForm.newPassword ? changePassForm.newPassword.value : "";
      const confirmPass = changePassForm.confirmPassword ? changePassForm.confirmPassword.value : "";
      if (newPass !== confirmPass) {
        e.preventDefault();
        if (changeError) { changeError.style.display = "block"; changeSuccess.style.display = "none"; }
        return;
      }
      // let the form submit to change-password.php to securely handle the update server-side
    });
  }
})();

// Accessibility tip: ensure forms have server-side validation and responses are surfaced to the user.
</script>

</body>
</html>
