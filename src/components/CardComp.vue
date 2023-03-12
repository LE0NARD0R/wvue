<template>
  <div class="container-fluid">
    <div class="barra container-fluid" v-for="(job, index) in joblist" :key="index">
      <div class="tittle">{{ job.name }}</div>
      <div class="col">{{ job.companie }}</div>
      <div class="col">{{ job.salary }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComp",
  props: {
    lists: Number,
  },
  data() {
    return {
      joblist: [
        {
          name: "Ingeniero de software",
          companie: "Importante Empresa Del Sector",
          salary: "$3.000.000",
        },
        {
          name: "Gerente de proyectos",
          companie: "METALES Y MADERAS DEL RISARALDA",
          salary: "$5.000.000",
        },
        {
          name: "Practicante de seguridad y salud en el trabajo",
          companie: "Eficacia",
          salary: "$1.500.000",
        },
        {
          name: "Analista financiero",
          companie: "Alentti | Portal de Empleo",
          salary: "$4.000.000",
        },
        {
          name: "Practicante en mercading",
          companie: "Eficacia",
          salary: "$1.000.000",
        },
        {
          name: "Analista financiero",
          companie: "Alentti | Portal de Empleo",
          salary: "$3.500.000",
        },
        {
          name: "Gerente de proyectos",
          companie: "METALES Y MADERAS DEL RISARALDA",
          salary: "$5.000.000",
        },
        {
          name: "Ingeniero de software",
          companie: "Importante Empresa Del Sector",
          salary: "$4.000.000",
        },
      ],
    };
  },
};
</script>

<style scoped>
.container-fluid {
  width: 100%;
  height: auto;
  padding-right: var(--bs-gutter-x, 0.75rem);
  padding-left: var(--bs-gutter-x, 0.75rem);
  margin-right: auto;
  margin-left: auto;
}

.barra {
  width: 86vw;
  height: 12vh;
  background-color: rgb(179, 168, 207);
  border-radius: 7px;
  box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.5);
  margin: 20px;
}
.tittle {
  position: relative;
  height: auto;
  top: 5px;
  left: 5px;
  margin: 2px;
  padding: 5px;
  text-align: left;
  font-size: 1.5em;
}

.col {
  float: left;
  padding: 5px;
  width: 45%;
  font-size: 0.9em;
}
</style>
