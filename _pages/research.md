---
permalink: /research/
title: "Research"
author_profile: true
---

<style>
/* ==== Research Page Custom Styling ==== */
.research-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 24px;
  justify-content: center;
  margin-top: 20px;
}

.research-card {
  background: #fff;
  border: 1px solid #ddd;
  border-radius: 12px;
  width: 320px;
  padding: 16px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.08);
  transition: all 0.2s ease-in-out;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 470px; /* Fixed height for consistent alignment */
  overflow: hidden;
}

.research-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 16px rgba(0,0,0,0.12);
}

.research-card img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  border-radius: 8px;
  margin-bottom: 12px;
}

.research-card h3 {
  margin-top: 0;
  font-size: 1.1rem;
  border-left: 4px solid #E87722;
  padding-left: 10px;
  font-weight: 700;
}

.research-card p {
  font-size: 0.95rem;
  color: #444;
  line-height: 1.4;
  margin-bottom: 10px;
  display: -webkit-box;
  -webkit-line-clamp: 4; /* show only 4 lines */
  -webkit-box-orient: vertical;
  overflow: hidden;
  transition: max-height 0.3s ease;
}

.research-card.expanded p {
  -webkit-line-clamp: unset;
  max-height: none;
}

.research-card .button {
  display: inline-block;
  padding: 6px 14px;
  background-color: #E87722;
  color: white;
  border-radius: 6px;
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 500;
  text-align: center;
  transition: all 0.2s ease;
}

.research-card .button:hover {
  background-color: #cf6b1e;
}

/* View More button for expanding */
.research-card .view-more {
  background: none;
  border: none;
  color: #E87722;
  font-size: 0.9rem;
  font-weight: 600;
  cursor: pointer;
  padding: 0;
  margin-top: 5px;
}
</style>

## Research Highlights

<div class="research-grid">

  <div class="research-card">
    <img src="/pr_makerspace_.jpeg" alt="people sitting at tables doing braille activities">
    <h3>Envisioning the Creation of A Culturally-Responsive and Accessible Makerspace</h3>
    <p>Exploring how communities in Puerto Rico imagine a makerspace that is accessible and reflects their culture. The project highlights participatory design methods that empower participants to shape the future of inclusive making spaces through co-design workshops, local engagement, and storytelling-based prototyping.</p>
    <button class="view-more" onclick="toggleDescription(this)">View More</button>
  </div>

  <div class="research-card">
    <img src="/blv_project.jpeg" alt="A laptop, a MakeyMakey kit, and conductive objects on a table">
    <h3>Community-engaged Partnership with Blind and Low-Vision Youth</h3>
    <p>Developing long-term relationships with a local organization to expose BLV youth to information and opportunities in technology and STEM. This work uses inclusive learning practices, hands-on workshops, and adaptive materials to support meaningful engagement and creative confidence among youth participants.</p>
    <button class="view-more" onclick="toggleDescription(this)">View More</button>
  </div>

  <div class="research-card">
    <img src="/assembly_line_project.jpeg" alt="assembly line work setting">
    <h3>Investigating the Work Practices of Assembly Line Workers with Visual Impairments</h3>
    <p>Studying experiences and challenges of assembly line garment workers, along with strategies and workarounds developed to support workflow and independence. The study centers workers’ voices and identifies design opportunities for more inclusive assistive technologies in manufacturing environments.</p>
    <button class="view-more" onclick="toggleDescription(this)">View More</button>
  </div>

</div>

<script>
function toggleDescription(button) {
  const card = button.closest(".research-card");
  const isExpanded = card.classList.toggle("expanded");
  button.textContent = isExpanded ? "View Less" : "View More";
}
</script>
