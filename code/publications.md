---
title: Publications
layout: home
nav_order: 2
last_modified_date: July 29 2025 at 11:46 AM
---

# Publications

## Conference papers

{% bibliography --file conference --sort-by year%}

## Journal papers

{% bibliography --file journal --sort-by year%}

## Workshop papers

{% bibliography --file workshop --sort-by year%}

## Preprint papers

{% bibliography --file preprint --sort-by year%}


# PhD thesis
 <a href="https://iris.unige.it/retrieve/0491538c-536a-4994-86a8-e55c9535a110/phdunige_4231932.pdf" target="_blank"><i class="fa-solid fa-file"></i>
 Resource-awareness for Java-like languages and beyond </a>
  <i class="fas fa-search" style="font-size: 20px;" data-bs-toggle="modal" data-bs-target="#abstractModalPhDThesis"></i>\\
supervised by Elena Zucca (Unige), Francesco Dagnino (Unige) and Paola Giannini (UniUpo)\\
DIBRIS - Università di Genova\\
PhD Program in Computer Science and System Engineering, Cycle XXXVI\\
Thesis defended in April 23, 2024

<div class="modal fade" id="abstractModalPhDThesis{{ entry.key | slugify }}" tabindex="-1" aria-labelledby="modalLabelAbstractPhD{{ entry.key | slugify }}" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="modalLabelAbstractPhD{{ entry.key | slugify }}">Abstract</h5>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Chiudi"></button>
      </div>
      <div class="modal-body" id="contentAbstractPhD{{ entry.key | slugify }}">
          {% assign pair = site.data.abstracts.abstracts | where: "keyword", "PhDThesis" | first %}
          {{ pair.abstract }}
      </div>
    </div>
  </div>
</div>

# Software
 <a href="https://github.com/RiccardoBianc/QueryAGT" target="_blank"><i class="fa-brands fa-github"></i>
Query AGT: An implementation in co-logic programming of the asynchronous global type system with a simple query language to interact with it
</a>

<script>
document.addEventListener('DOMContentLoaded', function () {
  const copyButtons = document.querySelectorAll('.copy-btn');

  copyButtons.forEach(button => {
    button.addEventListener('click', function () {
      const targetId = this.getAttribute('data-target');
      const content = document.getElementById(targetId).textContent;

      navigator.clipboard.writeText(content).then(() => {
        this.textContent = "Copied!";
        setTimeout(() => this.textContent = "Copy in clipboard", 2000);
      }).catch(err => {
        console.error('Error in copying the content', err);
        this.textContent = "Error in copying the content";
      });
    });
  });
});
</script>