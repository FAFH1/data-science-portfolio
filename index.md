---
layout: default
title: Kejia He | Data Science Portfolio
---

<section class="hero">
  <div>
    <p class="eyebrow">Data science portfolio</p>
    <h1>Turning data into <span>clear evidence.</span></h1>
    <p class="lede">I am Kejia He, a data science learner interested in exploratory analysis, reproducible workflows, and visual storytelling. This portfolio shows how I move from a research question to validated results that another person can rerun.</p>
    <div class="button-row">
      <a class="button" href="#project">View the project</a>
      <a class="button secondary" href="https://github.com/FAFH1/data-science-project">Open the repository</a>
    </div>
  </div>
  <aside class="hero-card" aria-label="Featured project summary">
    <span class="status">Project completed</span>
    <strong>Iris species classification</strong>
    <p>A transparent baseline combining exploratory data analysis with a reproducible hold-out evaluation.</p>
    <div class="metric">80%</div>
    <div class="metric-label">hold-out accuracy across three species</div>
  </aside>
</section>

<section class="about" id="about">
  <div class="about-grid">
    <div>
      <p class="eyebrow">About me</p>
      <h2>Curious about the story behind the numbers.</h2>
    </div>
    <div class="about-copy">
      <p>My approach is simple: ask a focused question, inspect the data before modelling it, communicate findings visually, and document every step so the result can be checked.</p>
      <p>This project demonstrates the full workflow — data validation, descriptive analysis, classification, evaluation, visualization, and public documentation. I am continuing to strengthen my skills in statistical reasoning, machine learning, and accessible data communication.</p>
    </div>
  </div>
</section>

<section id="skills">
  <p class="eyebrow">Technical skills</p>
  <div class="skill-grid">
    <article class="skill-card">
      <h3>Python analysis</h3>
      <p>pandas, NumPy, reusable scripts, data validation, and deterministic workflows.</p>
    </article>
    <article class="skill-card">
      <h3>Visual communication</h3>
      <p>Exploratory charts, labeled comparisons, result interpretation, and accessible layouts.</p>
    </article>
    <article class="skill-card">
      <h3>Reproducible practice</h3>
      <p>Git, GitHub, requirements files, documented setup steps, and versioned results.</p>
    </article>
  </div>
</section>

<section id="project">
  <div class="project-layout">
    <aside class="project-meta">
      <span class="project-tag">Featured project</span>
      <h2>Iris species: measurement patterns and classification</h2>
      <p><strong>Research question:</strong> How do flower measurements differ among Iris species, and how well can a simple distance-based model classify unseen flowers?</p>
      <ul class="facts">
        <li><span>Dataset</span><strong>150 Iris flowers</strong></li>
        <li><span>Methods</span><strong>Exploratory analysis + nearest centroid</strong></li>
        <li><span>Result</span><strong>80% hold-out accuracy</strong></li>
        <li><span>Status</span><strong>Completed</strong></li>
      </ul>
      <div class="button-row">
        <a class="button" href="https://github.com/FAFH1/data-science-project">Project repository</a>
      </div>
    </aside>

    <div class="project-content">
      <figure class="figure-card">
        <img src="{{ '/images/project-petal-scatter.png' | relative_url }}" alt="Scatter plot showing petal length and width for three Iris species">
        <figcaption>Setosa forms a clear cluster, while versicolor and virginica overlap in petal measurements.</figcaption>
      </figure>

      <div class="finding-grid">
        <div class="finding">
          <strong>Petal length separates species</strong>
          <p>Mean petal length rises from 1.46 cm for setosa to 4.26 cm for versicolor and 5.55 cm for virginica.</p>
        </div>
        <div class="finding">
          <strong>Two measurements move together</strong>
          <p>Petal length and petal width have a strong positive correlation of 0.963.</p>
        </div>
        <div class="finding">
          <strong>Classification is useful but imperfect</strong>
          <p>The baseline classifies every test setosa correctly but confuses some versicolor and virginica flowers.</p>
        </div>
        <div class="finding">
          <strong>Visual evidence supports the model result</strong>
          <p>The confusion matrix agrees with the overlap visible in the scatter plot.</p>
        </div>
      </div>

      <figure class="figure-card">
        <img src="{{ '/images/project-species-means.png' | relative_url }}" alt="Bar chart of mean petal length by Iris species">
        <figcaption>Mean petal length by species with one standard deviation shown by the whiskers.</figcaption>
      </figure>

      <figure class="figure-card">
        <img src="{{ '/images/project-confusion-matrix.png' | relative_url }}" alt="Confusion matrix for the nearest-centroid classifier">
        <figcaption>The hold-out confusion matrix makes the type and scale of classification errors explicit.</figcaption>
      </figure>

      <div class="callout">
        <h3>What I would improve next</h3>
        <p>I would test repeated cross-validation and compare the baseline with logistic regression and tree-based models. I would also add a small uncertainty analysis so the accuracy estimate is not based on a single train/test split.</p>
      </div>
    </div>
  </div>
</section>
