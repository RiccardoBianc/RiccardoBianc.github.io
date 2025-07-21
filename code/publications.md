---
title: Publications
layout: home
nav_order: 2
last_modified_date: July 21 2025 at 09:20 AM
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
 Resource-awareness for Java-like languages and beyond </a>\\
supervised by Elena Zucca (Unige), Francesco Dagnino (Unige) and Paola Giannini (UniUpo)\\
DIBRIS - Università di Genova\\
PhD Program in Computer Science and System Engineering, Cycle XXXVI\\
Thesis defended in April 23, 2024

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