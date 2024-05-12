<script></script>

<template>
  <div class="company">
    <h1 class="title">
      <span class="box"></span>Why Choose<span class="title2"> Us?</span>
    </h1>
    <div class="card-container">
      <div class="card">
        <img
          src="../assets/company-value1.svg"
          alt="card-image"
          class="card-image"
        />
        <h1 class="card-title">High Quality Intern</h1>
        <p class="card-body">
          Candidates will go through our Right KLIC Curation process to help
          identify their potential and competency.
        </p>
      </div>
      <div class="card">
        <img
          src="../assets/company-value2.svg"
          alt="card-image"
          class="card-image"
        />
        <h1 class="card-title">Experienced Coaches</h1>
        <p class="card-body">
          Candidates will go through our Right KLIC Curation process to help
          identify their potential and competency.
        </p>
      </div>
      <div class="card">
        <img
          src="../assets/company-value3.svg"
          alt="card-image"
          class="card-image"
        />
        <h1 class="card-title">Training and Coaching</h1>
        <p class="card-body">
          Candidates will go through our Right KLIC Curation process to help
          identify their potential and competency.
        </p>
      </div>
      <div class="card">
        <img
          src="../assets/company-value4.svg"
          alt="card-image"
          class="card-image"
        />
        <h1 class="card-title">Cost Efficient Solution</h1>
        <p class="card-body">
          Candidates will go through our Right KLIC Curation process to help
          identify their potential and competency.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.company {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.title {
  font-size: 36pt;
  font-weight: bold;
  color: #110f5e;
  margin-bottom: 24px;
}
.title2 {
  color: #fddc58;
}
.box {
  background-color: transparent;
  border: 5px solid #110f5e;
  margin-right: 24px;
}

.card-container {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
}

.card {
  flex-basis: 23%;
  height: auto;
  padding: 18px;
  display: flex;
  flex-direction: column;
  background-color: white;
  align-items: center;
  justify-content: center;
  border-radius: 32px;
  box-shadow: 0px 6px 10px 0px rgba(0, 0, 0, 0.2);
  margin-bottom: 20px;
}

.card > *:not(:last-child) {
  margin-bottom: 20px;
}

.card-image {
  width: 175px;
  height: 200px;
}

.card-title {
  text-align: center;
  font-weight: bold;
  font-size: 20pt;
}

.card-body {
  font-size: 12pt;
  font-weight: normal;
  text-align: center;
}

@media (max-width: 1024px) {
  .title {
    font-size: 36pt;
  }
  .card {
    flex-basis: 48%;
    border-radius: 24;
  }
  .card-title {
    font-size: 16pt;
  }

  .card-body {
    font-size: 11pt;
  }
}

@media (max-width: 768px) {
  .title {
    font-size: 24pt;
  }
  .card {
    flex-basis: 80%;
    border-radius: 16px;
  }
  .card-title {
    font-size: 14pt;
  }

  .card-body {
    font-size: 10pt;
  }
}

@media (max-width: 480px) {
  .title {
    font-size: 18pt;
  }
  .card {
    flex-basis: 80%;
    border-radius: 12px;
  }
  .card-title {
    font-size: 14pt;
  }

  .card-body {
    font-size: 10pt;
  }
}
</style>
